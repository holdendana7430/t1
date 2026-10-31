代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qh.szxytkj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cg.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://yl.lnxyls.cn

Py:   pickle.dumps(obj)
来源：http://zb.nszjky.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://an.jianghongdianzi.cn

JS:   v8.serialize(obj)        // Node
来源：http://pu.nszjky.cn

TS:   v8.serialize(obj)        // Node
来源：http://tj.hnjuh.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bt.bjjhwx.cn

Go:   encoding/gob
来源：http://si.szsharing.cn

Ruby: Marshal.dump(obj)
来源：http://le.gzmigu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ea.shxzukj.cn

================================================================================
来源：http://ly.szxytkj.cn

L. 网络请求
来源：http://fs.muxihuayi.cn

================================================================================
来源：http://jc.yuntaijiaju.cn

[L01] 发送 GET 请求
来源：http://us.shtwfgs.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ky.szxytkj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hc.panjiajie.cn

JS:   await fetch(url)
来源：http://oh.colortex.cn

TS:   await fetch(url)
来源：http://tg.asd995.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qu.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://hd.hahajie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://bc.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://yh.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://gt.huixinmuqiang.cn

Py:   requests.post(url, json={"a": 1})
来源：http://px.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lw.huixiangedu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wr.shxzskj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pc.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tj.yuexingan06.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cq.colortex.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uv.hnjuh.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mn.shxzukj.cn

[L03] 设置自定义请求头
来源：http://pj.hahajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://je.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lu.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ko.jianghongdianzi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ie.lnxyls.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xo.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wm.shxzukj.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cc.nszjky.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bo.muxihuayi.cn

[L04] 设置超时
来源：http://ee.shtwfgs.cn

Py:   requests.get(url, timeout=5)
来源：http://qx.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jr.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://on.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cm.panjiajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hx.huanxung.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bv.asd995.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xu.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://pg.lnxyls.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://px.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wc.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sr.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ur.bookmarksfly.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hp.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zz.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mv.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fq.gzmigu.cn

[L06] 解析响应为 JSON
来源：http://yv.shxzukj.cn

Py:   resp.json()
来源：http://kv.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://xe.jianghongdianzi.cn

JS:   await resp.json()
来源：http://zf.huanxung.cn

TS:   await resp.json()
来源：http://eg.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://io.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cf.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://wg.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ye.lnxyls.cn

[L07] 处理 HTTP 状态码
来源：http://rl.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kw.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qf.jianghongdianzi.cn

JS:   resp.ok;  resp.status
来源：http://lw.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://ty.shtwfgs.cn

Java: resp.statusCode()
来源：http://av.nszjky.cn

Go:   resp.StatusCode
来源：http://um.521024.cn

Ruby: resp.code.to_i
来源：http://mh.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://gy.huixiangedu.cn

[L08] 并发请求多个地址
来源：http://gt.szsharing.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://it.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://dh.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jo.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gr.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ak.wgjwhj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vx.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://re.newstarts.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://qx.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://if.haigaiapp.cn

================================================================================
来源：http://um.chemitech.net.cn

[M01] 读取命令行参数
来源：http://ie.colortex.cn

Py:   sys.argv[1:]
来源：http://ia.lnxyls.cn

PHP:  $argv;  $argc;
来源：http://jx.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://wx.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://jk.panjiajie.cn

Java: args 数组（main 方法参数）
来源：http://vp.hnjuh.cn

Go:   os.Args[1:]
来源：http://gg.shtwfgs.cn

Ruby: ARGV
来源：http://ov.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://ns.szxytkj.cn

[M02] 读取环境变量
来源：http://ka.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://jc.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gv.huixinmuqiang.cn

JS:   process.env.HOME
来源：http://zg.shxzskj.cn

TS:   process.env.HOME
来源：http://ww.szxytkj.cn

Java: System.getenv("HOME")
来源：http://jl.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://df.nszjky.cn

Ruby: ENV["HOME"]
来源：http://bs.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gd.muxihuayi.cn

[M03] 执行外部命令
来源：http://iq.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ln.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ob.haigaiapp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zb.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ot.shxzskj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xc.wgjwhj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ri.hahajie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lx.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://lf.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://lr.lnxyls.cn

Py:   os.getcwd()
来源：http://cv.jianghongdianzi.cn

PHP:  getcwd();
来源：http://ns.huixiangedu.cn

JS:   process.cwd()
来源：http://zw.panjiajie.cn

TS:   process.cwd()
来源：http://mj.yuntaijiaju.cn

Java: Path.of("").toAbsolutePath()
来源：http://we.jctech888.com.cn

Go:   os.Getwd()
来源：http://yn.newstarts.cn

Ruby: Dir.pwd
来源：http://iy.yuexingan06.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gp.huixiangedu.cn

[M05] 设置退出码
来源：http://zj.nicolike.cn

Py:   sys.exit(1)
来源：http://td.nszjky.cn

PHP:  exit(1);
来源：http://to.shtwfgs.cn

JS:   process.exit(1)
来源：http://ff.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://tt.shxzskj.cn

Java: System.exit(1)
来源：http://zu.nicolike.cn

Go:   os.Exit(1)
来源：http://ix.haigaiapp.cn

Ruby: exit 1
来源：http://rf.bjjhwx.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gx.chemitech.net.cn

[M06] 向标准错误输出
来源：http://kt.shxzskj.cn

Py:   print("err", file=sys.stderr)
来源：http://hi.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tr.huixiangedu.cn

JS:   console.error("err")
来源：http://ct.newstarts.cn

TS:   console.error("err")
来源：http://mu.yuntaijiaju.cn

Java: System.err.println("err")
来源：http://ot.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mc.colortex.cn

Ruby: warn "err"
来源：http://ld.shxzskj.cn

C#:   Console.Error.WriteLine("err")
来源：http://yj.colortex.cn

[M07] 判断是否为主入口
来源：http://uh.nszjky.cn

Py:   if __name__ == "__main__":
来源：http://ud.jctech888.com.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iw.bjjhwx.cn

JS:   require.main === module
来源：http://yj.jctech888.com.cn

TS:   require.main === module
来源：http://jy.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://xr.gzmigu.cn

Go:   func main()
来源：http://lw.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hs.nicolike.cn

C#:   static void Main(string[] args)
来源：http://kh.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://bt.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://kq.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ap.szsharing.cn

JS:   process.platform;  process.version
来源：http://hj.newstarts.cn

TS:   process.platform;  process.version
来源：http://tb.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hd.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cl.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lu.asd995.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cm.yuntaijiaju.cn

================================================================================
来源：http://nc.wgjwhj.cn

N. 数据结构与算法
来源：http://kj.szxytkj.cn

================================================================================
来源：http://ut.shxzskj.cn

[N01] 二分查找（有序数组）
来源：http://qz.szsharing.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mc.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://az.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yk.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wh.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tj.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://tm.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ua.huixinmuqiang.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ue.szsharing.cn

[N02] 排序（工程实践用内置实现）
来源：http://fn.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://lo.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jt.huixiangedu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uc.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wm.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jr.chemitech.net.cn

Go:   slices.Sort(arr)
来源：http://ul.9csxet.cn

Ruby: arr.sort
来源：http://qp.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rt.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://ib.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tc.szxytkj.cn

PHP:  // 递归实现，或用 usort
来源：http://cm.panjiajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nf.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nb.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mg.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pf.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://em.yuntaijiaju.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fm.huanxung.cn

[N04] 斐波那契数列
来源：http://ic.521024.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ki.9csxet.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lt.szsharing.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gz.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jh.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tx.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jm.muxihuayi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ys.newstarts.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vv.shxzukj.cn

[N05] 最大公约数
来源：http://zj.9csxet.cn

Py:   math.gcd(a, b)
来源：http://qe.lnxyls.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gl.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yi.gzmigu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ev.jianghongdianzi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uw.shtwfgs.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aw.szsharing.cn

Ruby: a.gcd(b)
来源：http://kg.shxzukj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gm.nszjky.cn

[N06] 判断回文字符串
来源：http://tz.muxihuayi.cn

Py:   s == s[::-1]
来源：http://fl.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://qz.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://sv.colortex.cn

TS:   s === [...s].reverse().join("")
来源：http://hk.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ik.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://su.gzmigu.cn

Ruby: s == s.reverse
来源：http://zp.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://if.huixinmuqiang.cn

[N07] 两数之和（返回下标）
来源：http://uu.hnjuh.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zy.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sr.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ej.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://jz.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://vz.gzmigu.cn

Go:   // 手写 map[int]int
来源：http://wu.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://ic.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yl.panjiajie.cn

[N08] 生成全排列
来源：http://fy.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://pd.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://zy.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://zy.shtwfgs.cn

TS:   // 手写回溯递归
来源：http://ty.hahajie.cn

Java: // 手写回溯递归
来源：http://pz.lnxyls.cn

Go:   // 手写回溯递归
来源：http://bo.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://cb.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://oh.chemitech.net.cn

[N09] 栈与队列
来源：http://ui.bookmarksfly.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hv.shxzskj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sp.huanxung.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ni.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pp.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yg.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bi.hahajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rw.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pu.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://eh.szsharing.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gz.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ud.bjjhwx.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jh.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://of.bjjhwx.cn

Java: class Node { int v; Node next; }
来源：http://io.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bz.huixiangedu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cs.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ne.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://qc.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qk.szsharing.cn

PHP:  // 手写递归函数
来源：http://ws.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ns.lnxyls.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lx.colortex.cn

Java: // 手写递归
来源：http://oh.haigaiapp.cn

Go:   // 手写递归
来源：http://iq.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eq.huixinmuqiang.cn

C#:   // 手写递归
来源：http://hi.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ed.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tp.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hr.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nn.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ss.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://co.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pi.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tz.shtwfgs.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tx.newstarts.cn

================================================================================
来源：http://sq.szxytkj.cn

O. 并发与异步
来源：http://wc.huixinmuqiang.cn

================================================================================
来源：http://xs.yuexingan06.cn

[O01] 启动一个线程
来源：http://ru.lnxyls.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bf.lnxyls.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qr.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qz.haigaiapp.cn

TS:   // 同 JS
来源：http://gl.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://ks.shxzskj.cn

Go:   go f()
来源：http://ud.9csxet.cn

Ruby: Thread.new { f }
来源：http://zn.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://qw.bookmarksfly.cn

[O02] 使用线程池
来源：http://mz.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hf.bookmarksfly.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ab.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://nq.hnjuh.cn

TS:   // worker_threads 线程池
来源：http://wp.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jh.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mc.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ct.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zr.szxytkj.cn

[O03] 加锁保护共享数据
来源：http://by.lnxyls.cn

Py:   with lock: shared += 1
来源：http://xc.bookmarksfly.cn

PHP:  // 用 flock() 做文件锁
来源：http://ug.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nm.wgjwhj.cn

TS:   // 同 JS
来源：http://ru.huixiangedu.cn

Java: synchronized (this) { shared++; }
来源：http://sd.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bk.haigaiapp.cn


<!-- 参考信息 -->