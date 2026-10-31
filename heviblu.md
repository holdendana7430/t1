代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xv.yuntaijiaju.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://et.huixiangedu.cn

[K08] 二进制序列化（非 JSON）
来源：http://mn.huixiangedu.cn

Py:   pickle.dumps(obj)
来源：http://if.muxihuayi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://bk.yuexingan06.cn

JS:   v8.serialize(obj)        // Node
来源：http://yc.szsharing.cn

TS:   v8.serialize(obj)        // Node
来源：http://ny.colortex.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xe.jctech888.com.cn

Go:   encoding/gob
来源：http://ky.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://hz.wgjwhj.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oo.shxzukj.cn

================================================================================
来源：http://qs.nicolike.cn

L. 网络请求
来源：http://ca.shxzskj.cn

================================================================================
来源：http://ev.colortex.cn

[L01] 发送 GET 请求
来源：http://pt.huixiangedu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://je.wgjwhj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ke.huixinmuqiang.cn

JS:   await fetch(url)
来源：http://re.nicolike.cn

TS:   await fetch(url)
来源：http://ta.yuexingan06.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wv.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://qp.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cj.9csxet.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jr.huixiangedu.cn

[L02] 发送 POST JSON
来源：http://wx.haigaiapp.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vp.chemitech.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://on.bookmarksfly.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iu.asd995.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ky.jianghongdianzi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://at.9csxet.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ss.chemitech.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bi.nicolike.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nm.panjiajie.cn

[L03] 设置自定义请求头
来源：http://zd.nszjky.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xx.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qb.nszjky.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lb.haigaiapp.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jp.newstarts.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ns.bookmarksfly.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ll.bjjhwx.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hr.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lp.panjiajie.cn

[L04] 设置超时
来源：http://cq.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://cl.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ff.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ja.chemitech.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ms.9csxet.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://or.shtwfgs.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://li.bookmarksfly.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://oz.muxihuayi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rt.huixinmuqiang.cn

[L05] 上传文件（multipart）
来源：http://lx.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ix.yuntaijiaju.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jf.asd995.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://iz.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mf.panjiajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qx.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kg.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yw.lnxyls.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cl.huixinmuqiang.cn

[L06] 解析响应为 JSON
来源：http://wn.szsharing.cn

Py:   resp.json()
来源：http://ma.hnjuh.cn

PHP:  json_decode($body, true);
来源：http://oj.panjiajie.cn

JS:   await resp.json()
来源：http://at.bookmarksfly.cn

TS:   await resp.json()
来源：http://lm.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fx.asd995.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ds.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://gp.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cs.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://st.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kc.haigaiapp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ma.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://xu.yuntaijiaju.cn

TS:   resp.ok;  resp.status
来源：http://gt.asd995.cn

Java: resp.statusCode()
来源：http://bn.huanxung.cn

Go:   resp.StatusCode
来源：http://qs.huanxung.cn

Ruby: resp.code.to_i
来源：http://kc.bjjhwx.cn

C#:   (int)resp.StatusCode
来源：http://ls.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://kl.muxihuayi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dn.wgjwhj.cn

PHP:  curl_multi_init() 系列
来源：http://ko.huixiangedu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ft.jianghongdianzi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nd.yuexingan06.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vj.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nn.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jt.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xg.szsharing.cn

================================================================================
来源：http://dx.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://wg.shtwfgs.cn

================================================================================
来源：http://ig.chemitech.net.cn

[M01] 读取命令行参数
来源：http://oy.asd995.cn

Py:   sys.argv[1:]
来源：http://lb.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://kp.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://si.9csxet.cn

TS:   process.argv.slice(2)
来源：http://em.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://ql.gzmigu.cn

Go:   os.Args[1:]
来源：http://pr.szxytkj.cn

Ruby: ARGV
来源：http://un.szsharing.cn

C#:   args 数组（Main 方法参数）
来源：http://py.newstarts.cn

[M02] 读取环境变量
来源：http://hw.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://bt.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vw.wgjwhj.cn

JS:   process.env.HOME
来源：http://or.newstarts.cn

TS:   process.env.HOME
来源：http://cv.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://sr.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dh.huanxung.cn

Ruby: ENV["HOME"]
来源：http://jk.jctech888.com.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ol.lnxyls.cn

[M03] 执行外部命令
来源：http://ra.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://za.newstarts.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ig.shxzskj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rf.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qi.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eo.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zy.lnxyls.cn

Ruby: system("ls -l");  `ls -l`
来源：http://za.521024.cn

C#:   Process.Start("ls", "-l");
来源：http://ax.9csxet.cn

[M04] 获取当前工作目录
来源：http://yc.muxihuayi.cn

Py:   os.getcwd()
来源：http://gl.bjjhwx.cn

PHP:  getcwd();
来源：http://mf.huixinmuqiang.cn

JS:   process.cwd()
来源：http://jk.wgjwhj.cn

TS:   process.cwd()
来源：http://wg.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://ai.nszjky.cn

Go:   os.Getwd()
来源：http://cq.gzmigu.cn

Ruby: Dir.pwd
来源：http://sx.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vx.9csxet.cn

[M05] 设置退出码
来源：http://bd.asd995.cn

Py:   sys.exit(1)
来源：http://ff.gzmigu.cn

PHP:  exit(1);
来源：http://rd.521024.cn

JS:   process.exit(1)
来源：http://ps.bjjhwx.cn

TS:   process.exit(1)
来源：http://gf.huanxung.cn

Java: System.exit(1)
来源：http://qd.hahajie.cn

Go:   os.Exit(1)
来源：http://xg.521024.cn

Ruby: exit 1
来源：http://ow.bookmarksfly.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xi.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://aa.jctech888.com.cn

Py:   print("err", file=sys.stderr)
来源：http://jx.asd995.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vp.yuexingan06.cn

JS:   console.error("err")
来源：http://bu.szsharing.cn

TS:   console.error("err")
来源：http://uu.szxytkj.cn

Java: System.err.println("err")
来源：http://ct.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gg.haigaiapp.cn

Ruby: warn "err"
来源：http://vv.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://eg.nszjky.cn

[M07] 判断是否为主入口
来源：http://vl.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://my.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jb.521024.cn

JS:   require.main === module
来源：http://bj.9csxet.cn

TS:   require.main === module
来源：http://co.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://sy.huanxung.cn

Go:   func main()
来源：http://qu.muxihuayi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vn.szsharing.cn

C#:   static void Main(string[] args)
来源：http://fq.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://tt.shxzukj.cn

Py:   platform.system();  platform.python_version()
来源：http://io.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://wo.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://za.huixiangedu.cn

TS:   process.platform;  process.version
来源：http://xn.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://go.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://aw.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zg.szxytkj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://he.lnxyls.cn

================================================================================
来源：http://jo.521024.cn

N. 数据结构与算法
来源：http://ed.haigaiapp.cn

================================================================================
来源：http://ih.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://bw.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://en.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dx.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sd.huixinmuqiang.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ax.wgjwhj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ew.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://bq.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yc.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cw.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://kj.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://wb.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yw.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bk.521024.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fz.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9csxet.cn

Go:   slices.Sort(arr)
来源：http://vb.521024.cn

Ruby: arr.sort
来源：http://te.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://we.lnxyls.cn

[N03] 快速排序（分治示例）
来源：http://jx.muxihuayi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pp.shxzskj.cn

PHP:  // 递归实现，或用 usort
来源：http://xb.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://to.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yn.huanxung.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jd.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sx.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://js.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xz.gzmigu.cn

[N04] 斐波那契数列
来源：http://gt.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fp.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dm.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hs.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ev.muxihuayi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rq.huixiangedu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://av.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qh.jianghongdianzi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qm.gzmigu.cn

[N05] 最大公约数
来源：http://zj.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://ht.521024.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ar.huixinmuqiang.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://te.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zw.9csxet.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yz.yuntaijiaju.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ds.szsharing.cn

Ruby: a.gcd(b)
来源：http://tr.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qx.panjiajie.cn

[N06] 判断回文字符串
来源：http://of.yuexingan06.cn

Py:   s == s[::-1]
来源：http://qw.newstarts.cn

PHP:  $s === strrev($s);
来源：http://ft.521024.cn

JS:   s === [...s].reverse().join("")
来源：http://ds.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://kl.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pk.chemitech.net.cn

Go:   // 双指针从两端比较
来源：http://jw.asd995.cn

Ruby: s == s.reverse
来源：http://st.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://fp.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://vi.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wb.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lt.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sq.nszjky.cn

TS:   // 手写 Map<string, number>
来源：http://lb.nszjky.cn

Java: // 手写 HashMap
来源：http://rn.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://vj.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://nd.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mn.hahajie.cn

[N08] 生成全排列
来源：http://id.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://mj.haigaiapp.cn

PHP:  // 手写递归交换
来源：http://kp.colortex.cn

JS:   // 手写回溯递归
来源：http://ld.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://pz.huixinmuqiang.cn

Java: // 手写回溯递归
来源：http://oo.yuntaijiaju.cn

Go:   // 手写回溯递归
来源：http://pz.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://ad.lnxyls.cn

C#:   // 手写回溯递归
来源：http://mt.huixiangedu.cn

[N09] 栈与队列
来源：http://in.hahajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kd.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bs.huixinmuqiang.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ds.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fe.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://he.shxzukj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zq.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ls.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wr.huixiangedu.cn

[N10] 链表节点定义
来源：http://wg.521024.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nk.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fm.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://my.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wb.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://wq.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bb.chemitech.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yu.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dl.9csxet.cn

[N11] 二叉树中序遍历
来源：http://us.panjiajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iu.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://cc.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://go.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vo.bookmarksfly.cn

Java: // 手写递归
来源：http://ms.nszjky.cn

Go:   // 手写递归
来源：http://fv.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://id.nicolike.cn

C#:   // 手写递归
来源：http://wv.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dr.colortex.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hr.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://so.hnjuh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://op.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ju.asd995.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ln.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gq.colortex.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fw.newstarts.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jo.jctech888.com.cn

================================================================================
来源：http://rp.bjjhwx.cn

O. 并发与异步
来源：http://mt.wgjwhj.cn

================================================================================
来源：http://zq.szxytkj.cn

[O01] 启动一个线程
来源：http://zi.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iz.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fr.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ey.colortex.cn

TS:   // 同 JS
来源：http://uc.huixinmuqiang.cn

Java: new Thread(() -> f()).start()
来源：http://wu.nicolike.cn

Go:   go f()
来源：http://hp.yuexingan06.cn

Ruby: Thread.new { f }
来源：http://yz.nicolike.cn

C#:   Task.Run(() => F());
来源：http://ph.lnxyls.cn

[O02] 使用线程池
来源：http://ay.gzmigu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xy.shtwfgs.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rd.newstarts.cn

JS:   // worker_threads 线程池
来源：http://eh.521024.cn

TS:   // worker_threads 线程池
来源：http://qi.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jn.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://um.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ms.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fk.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://vw.hnjuh.cn

Py:   with lock: shared += 1
来源：http://hx.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://wq.muxihuayi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qj.jctech888.com.cn

TS:   // 同 JS
来源：http://bd.521024.cn

Java: synchronized (this) { shared++; }
来源：http://my.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://li.haigaiapp.cn


<!-- 参考信息 -->