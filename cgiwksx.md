代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://np.huanxung.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ti.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://kt.haigaiapp.cn

Py:   pickle.dumps(obj)
来源：http://sp.shtwfgs.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oh.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://ql.shtwfgs.cn

TS:   v8.serialize(obj)        // Node
来源：http://tr.lnxyls.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vs.newstarts.cn

Go:   encoding/gob
来源：http://jo.yuntaijiaju.cn

Ruby: Marshal.dump(obj)
来源：http://ik.yuexingan06.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://px.shtwfgs.cn

================================================================================
来源：http://lv.shxzukj.cn

L. 网络请求
来源：http://qn.shxzskj.cn

================================================================================
来源：http://cq.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://so.lnxyls.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nr.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lk.huanxung.cn

JS:   await fetch(url)
来源：http://np.yuexingan06.cn

TS:   await fetch(url)
来源：http://de.jctech888.com.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gi.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://is.yuexingan06.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hh.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://al.chemitech.net.cn

[L02] 发送 POST JSON
来源：http://yp.panjiajie.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ys.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bc.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jv.jianghongdianzi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://br.huixinmuqiang.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ae.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qn.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gy.newstarts.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hi.hnjuh.cn

[L03] 设置自定义请求头
来源：http://fh.lnxyls.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ua.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yw.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yb.9csxet.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lt.wgjwhj.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hs.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://om.newstarts.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ph.newstarts.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yn.yuexingan06.cn

[L04] 设置超时
来源：http://qx.panjiajie.cn

Py:   requests.get(url, timeout=5)
来源：http://ph.shxzskj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tu.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ep.jctech888.com.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nd.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://vp.colortex.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ry.shtwfgs.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://na.chemitech.net.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ej.huanxung.cn

[L05] 上传文件（multipart）
来源：http://sq.panjiajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lh.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rv.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jg.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nx.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://iq.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hi.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://jk.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://iv.nszjky.cn

[L06] 解析响应为 JSON
来源：http://wf.chemitech.net.cn

Py:   resp.json()
来源：http://rz.shxzukj.cn

PHP:  json_decode($body, true);
来源：http://ue.newstarts.cn

JS:   await resp.json()
来源：http://qw.wgjwhj.cn

TS:   await resp.json()
来源：http://do.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vd.jianghongdianzi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ym.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://bg.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jj.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://th.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fh.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://lw.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://ke.newstarts.cn

TS:   resp.ok;  resp.status
来源：http://ov.jctech888.com.cn

Java: resp.statusCode()
来源：http://if.hnjuh.cn

Go:   resp.StatusCode
来源：http://ev.szsharing.cn

Ruby: resp.code.to_i
来源：http://fj.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://ro.lnxyls.cn

[L08] 并发请求多个地址
来源：http://wa.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mu.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ip.shtwfgs.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ps.shxzukj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hm.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qw.hnjuh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ak.huixiangedu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xv.shxzskj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://en.lnxyls.cn

================================================================================
来源：http://mi.newstarts.cn

M. 命令行 / 进程 / 环境
来源：http://wz.nicolike.cn

================================================================================
来源：http://jg.newstarts.cn

[M01] 读取命令行参数
来源：http://mn.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://xa.colortex.cn

PHP:  $argv;  $argc;
来源：http://ds.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://mt.jctech888.com.cn

TS:   process.argv.slice(2)
来源：http://ji.colortex.cn

Java: args 数组（main 方法参数）
来源：http://pf.nicolike.cn

Go:   os.Args[1:]
来源：http://mw.yuntaijiaju.cn

Ruby: ARGV
来源：http://lf.nszjky.cn

C#:   args 数组（Main 方法参数）
来源：http://gj.huanxung.cn

[M02] 读取环境变量
来源：http://ns.asd995.cn

Py:   os.environ.get("HOME")
来源：http://mv.9csxet.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gm.hnjuh.cn

JS:   process.env.HOME
来源：http://ng.newstarts.cn

TS:   process.env.HOME
来源：http://cu.hahajie.cn

Java: System.getenv("HOME")
来源：http://vu.jianghongdianzi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vu.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://yj.muxihuayi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oc.bjjhwx.cn

[M03] 执行外部命令
来源：http://se.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sh.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xy.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jf.haigaiapp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rq.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vq.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://py.nicolike.cn

Ruby: system("ls -l");  `ls -l`
来源：http://az.9csxet.cn

C#:   Process.Start("ls", "-l");
来源：http://yg.szxytkj.cn

[M04] 获取当前工作目录
来源：http://eu.haigaiapp.cn

Py:   os.getcwd()
来源：http://bj.panjiajie.cn

PHP:  getcwd();
来源：http://ie.shxzskj.cn

JS:   process.cwd()
来源：http://vj.jctech888.com.cn

TS:   process.cwd()
来源：http://pb.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://dt.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://es.lnxyls.cn

Ruby: Dir.pwd
来源：http://mq.hnjuh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fx.9csxet.cn

[M05] 设置退出码
来源：http://jm.huixiangedu.cn

Py:   sys.exit(1)
来源：http://lm.bookmarksfly.cn

PHP:  exit(1);
来源：http://ex.huixinmuqiang.cn

JS:   process.exit(1)
来源：http://uv.huanxung.cn

TS:   process.exit(1)
来源：http://ds.hnjuh.cn

Java: System.exit(1)
来源：http://gg.jctech888.com.cn

Go:   os.Exit(1)
来源：http://qz.nszjky.cn

Ruby: exit 1
来源：http://bk.shtwfgs.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yy.haigaiapp.cn

[M06] 向标准错误输出
来源：http://qj.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://gf.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ls.bjjhwx.cn

JS:   console.error("err")
来源：http://vn.muxihuayi.cn

TS:   console.error("err")
来源：http://jx.yuexingan06.cn

Java: System.err.println("err")
来源：http://fy.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kp.huixinmuqiang.cn

Ruby: warn "err"
来源：http://py.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://du.gzmigu.cn

[M07] 判断是否为主入口
来源：http://ea.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://cx.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ex.jianghongdianzi.cn

JS:   require.main === module
来源：http://ql.lnxyls.cn

TS:   require.main === module
来源：http://mk.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://dr.hahajie.cn

Go:   func main()
来源：http://vh.szxytkj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pp.szxytkj.cn

C#:   static void Main(string[] args)
来源：http://tr.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://ye.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://gn.szxytkj.cn

PHP:  PHP_OS;  phpversion();
来源：http://fw.jianghongdianzi.cn

JS:   process.platform;  process.version
来源：http://zt.nszjky.cn

TS:   process.platform;  process.version
来源：http://ej.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hr.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fg.bjjhwx.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mv.hahajie.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bx.hnjuh.cn

================================================================================
来源：http://re.szsharing.cn

N. 数据结构与算法
来源：http://lu.huixinmuqiang.cn

================================================================================
来源：http://pl.jctech888.com.cn

[N01] 二分查找（有序数组）
来源：http://ne.lnxyls.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ep.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bj.nicolike.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://et.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mt.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wq.shxzskj.cn

Go:   sort.SearchInts(arr, x)
来源：http://jo.nszjky.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zx.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://st.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://zm.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://wm.haigaiapp.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://im.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dc.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sj.nicolike.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yd.hahajie.cn

Go:   slices.Sort(arr)
来源：http://of.bjjhwx.cn

Ruby: arr.sort
来源：http://su.nszjky.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://yf.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://bj.szsharing.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qu.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://tw.asd995.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ub.bookmarksfly.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wx.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://th.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vh.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dg.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mr.newstarts.cn

[N04] 斐波那契数列
来源：http://ts.szsharing.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oh.wgjwhj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rx.shxzskj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ml.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eo.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hl.szxytkj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xw.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ed.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oj.nszjky.cn

[N05] 最大公约数
来源：http://pq.nszjky.cn

Py:   math.gcd(a, b)
来源：http://ht.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rj.yuntaijiaju.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kw.panjiajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tn.shtwfgs.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fz.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yi.yuexingan06.cn

Ruby: a.gcd(b)
来源：http://tt.huixinmuqiang.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lc.hahajie.cn

[N06] 判断回文字符串
来源：http://ji.shxzukj.cn

Py:   s == s[::-1]
来源：http://hy.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://in.huixiangedu.cn

JS:   s === [...s].reverse().join("")
来源：http://ub.jianghongdianzi.cn

TS:   s === [...s].reverse().join("")
来源：http://vt.yuntaijiaju.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://im.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://lm.szxytkj.cn

Ruby: s == s.reverse
来源：http://za.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://of.hahajie.cn

[N07] 两数之和（返回下标）
来源：http://nl.gzmigu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fb.chemitech.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mo.asd995.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pk.asd995.cn

TS:   // 手写 Map<string, number>
来源：http://sw.shtwfgs.cn

Java: // 手写 HashMap
来源：http://dp.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://yg.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://ly.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zc.jianghongdianzi.cn

[N08] 生成全排列
来源：http://ti.szxytkj.cn

Py:   itertools.permutations(arr)
来源：http://is.nszjky.cn

PHP:  // 手写递归交换
来源：http://wy.panjiajie.cn

JS:   // 手写回溯递归
来源：http://qd.muxihuayi.cn

TS:   // 手写回溯递归
来源：http://ax.wgjwhj.cn

Java: // 手写回溯递归
来源：http://rb.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://in.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://di.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://gc.9csxet.cn

[N09] 栈与队列
来源：http://wu.huixinmuqiang.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fu.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hm.haigaiapp.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ed.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://at.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zm.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://up.shxzskj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jb.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wg.lnxyls.cn

[N10] 链表节点定义
来源：http://rr.panjiajie.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ii.yuntaijiaju.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://al.huanxung.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ad.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://km.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://cc.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kd.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ul.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xi.521024.cn

[N11] 二叉树中序遍历
来源：http://jf.huanxung.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zm.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://ui.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ta.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://un.nszjky.cn

Java: // 手写递归
来源：http://zo.shxzskj.cn

Go:   // 手写递归
来源：http://if.lnxyls.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oi.shxzskj.cn

C#:   // 手写递归
来源：http://ic.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mu.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://of.shxzukj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ol.shxzukj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wg.newstarts.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dx.szsharing.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ka.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cs.huanxung.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ty.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fi.jctech888.com.cn

================================================================================
来源：http://hy.shxzskj.cn

O. 并发与异步
来源：http://nx.hnjuh.cn

================================================================================
来源：http://zm.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://ae.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oi.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dd.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xs.huixiangedu.cn

TS:   // 同 JS
来源：http://gl.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://ti.bjjhwx.cn

Go:   go f()
来源：http://oc.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://sg.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://xd.shxzukj.cn

[O02] 使用线程池
来源：http://kt.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://is.yuntaijiaju.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oj.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://qy.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://bo.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://td.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mi.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xq.lnxyls.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zi.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://gc.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://va.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ro.huixinmuqiang.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tf.hahajie.cn

TS:   // 同 JS
来源：http://yg.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://cx.shxzskj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jj.huixinmuqiang.cn


<!-- 参考信息 -->