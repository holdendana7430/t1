代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://on.szsharing.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ci.gzmigu.cn

[K08] 二进制序列化（非 JSON）
来源：http://an.szxytkj.cn

Py:   pickle.dumps(obj)
来源：http://ws.yuntaijiaju.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oj.shxzukj.cn

JS:   v8.serialize(obj)        // Node
来源：http://mv.panjiajie.cn

TS:   v8.serialize(obj)        // Node
来源：http://pw.bookmarksfly.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vp.shxzukj.cn

Go:   encoding/gob
来源：http://om.newstarts.cn

Ruby: Marshal.dump(obj)
来源：http://kj.huanxung.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ro.szxytkj.cn

================================================================================
来源：http://bl.colortex.cn

L. 网络请求
来源：http://ci.hnjuh.cn

================================================================================
来源：http://il.9csxet.cn

[L01] 发送 GET 请求
来源：http://tz.panjiajie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bx.shtwfgs.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ii.bjjhwx.cn

JS:   await fetch(url)
来源：http://fo.bjjhwx.cn

TS:   await fetch(url)
来源：http://my.hahajie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ez.yuntaijiaju.cn

Go:   resp, err := http.Get(url)
来源：http://sk.yuntaijiaju.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://qg.hahajie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vc.lnxyls.cn

[L02] 发送 POST JSON
来源：http://xq.shxzskj.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ww.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gb.haigaiapp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ol.shxzukj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yg.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lq.shxzskj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wq.bjjhwx.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yh.huanxung.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ca.shxzskj.cn

[L03] 设置自定义请求头
来源：http://ov.huixiangedu.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ez.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fc.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://il.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qj.nszjky.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eo.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bj.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mh.9csxet.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rf.lnxyls.cn

[L04] 设置超时
来源：http://ef.chemitech.net.cn

Py:   requests.get(url, timeout=5)
来源：http://mq.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nc.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sl.szsharing.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rr.wgjwhj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nl.wgjwhj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jx.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jo.newstarts.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sy.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://sj.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pe.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nk.yuexingan06.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gy.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qi.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rb.521024.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fp.newstarts.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zk.yuntaijiaju.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://po.hahajie.cn

[L06] 解析响应为 JSON
来源：http://uy.nicolike.cn

Py:   resp.json()
来源：http://qv.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ns.chemitech.net.cn

JS:   await resp.json()
来源：http://ju.nicolike.cn

TS:   await resp.json()
来源：http://lb.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rp.gzmigu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ss.huanxung.cn

Ruby: JSON.parse(resp.body)
来源：http://cf.521024.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vd.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://jx.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hv.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mi.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://ig.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://zb.asd995.cn

Java: resp.statusCode()
来源：http://tx.asd995.cn

Go:   resp.StatusCode
来源：http://qz.shxzukj.cn

Ruby: resp.code.to_i
来源：http://vj.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://mo.nicolike.cn

[L08] 并发请求多个地址
来源：http://bb.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hq.hnjuh.cn

PHP:  curl_multi_init() 系列
来源：http://xn.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ai.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ow.asd995.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://np.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ah.muxihuayi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jy.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ef.yuexingan06.cn

================================================================================
来源：http://op.huanxung.cn

M. 命令行 / 进程 / 环境
来源：http://vh.9csxet.cn

================================================================================
来源：http://zs.bjjhwx.cn

[M01] 读取命令行参数
来源：http://rn.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://be.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://jf.bjjhwx.cn

JS:   process.argv.slice(2)
来源：http://ak.wgjwhj.cn

TS:   process.argv.slice(2)
来源：http://al.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://wf.9csxet.cn

Go:   os.Args[1:]
来源：http://an.shxzskj.cn

Ruby: ARGV
来源：http://rw.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://sl.huanxung.cn

[M02] 读取环境变量
来源：http://wv.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://ch.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cm.asd995.cn

JS:   process.env.HOME
来源：http://dk.yuexingan06.cn

TS:   process.env.HOME
来源：http://ln.9csxet.cn

Java: System.getenv("HOME")
来源：http://nw.521024.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://li.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://hu.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://io.panjiajie.cn

[M03] 执行外部命令
来源：http://ut.yuntaijiaju.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wh.9csxet.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fz.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cl.9csxet.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zc.szsharing.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ga.szxytkj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aq.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cv.shtwfgs.cn

C#:   Process.Start("ls", "-l");
来源：http://kv.nicolike.cn

[M04] 获取当前工作目录
来源：http://uf.haigaiapp.cn

Py:   os.getcwd()
来源：http://xi.muxihuayi.cn

PHP:  getcwd();
来源：http://mg.asd995.cn

JS:   process.cwd()
来源：http://vf.szxytkj.cn

TS:   process.cwd()
来源：http://om.9csxet.cn

Java: Path.of("").toAbsolutePath()
来源：http://gj.huixiangedu.cn

Go:   os.Getwd()
来源：http://tx.asd995.cn

Ruby: Dir.pwd
来源：http://am.jianghongdianzi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ee.huixiangedu.cn

[M05] 设置退出码
来源：http://as.hnjuh.cn

Py:   sys.exit(1)
来源：http://zf.nicolike.cn

PHP:  exit(1);
来源：http://he.bjjhwx.cn

JS:   process.exit(1)
来源：http://iv.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://om.asd995.cn

Java: System.exit(1)
来源：http://zf.panjiajie.cn

Go:   os.Exit(1)
来源：http://wn.huanxung.cn

Ruby: exit 1
来源：http://xm.huanxung.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oj.jctech888.com.cn

[M06] 向标准错误输出
来源：http://pl.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://st.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pg.lnxyls.cn

JS:   console.error("err")
来源：http://ud.chemitech.net.cn

TS:   console.error("err")
来源：http://tq.bookmarksfly.cn

Java: System.err.println("err")
来源：http://ig.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xf.bjjhwx.cn

Ruby: warn "err"
来源：http://it.huanxung.cn

C#:   Console.Error.WriteLine("err")
来源：http://np.shxzskj.cn

[M07] 判断是否为主入口
来源：http://yl.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://gb.huixiangedu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hk.yuntaijiaju.cn

JS:   require.main === module
来源：http://bt.asd995.cn

TS:   require.main === module
来源：http://mj.gzmigu.cn

Java: public static void main(String[] args)
来源：http://ra.lnxyls.cn

Go:   func main()
来源：http://wt.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lg.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://nm.bookmarksfly.cn

[M08] 获取系统与运行时信息
来源：http://qz.bookmarksfly.cn

Py:   platform.system();  platform.python_version()
来源：http://ka.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://jk.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://tg.colortex.cn

TS:   process.platform;  process.version
来源：http://vp.bookmarksfly.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oz.yuexingan06.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rr.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://px.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://lt.szsharing.cn

================================================================================
来源：http://uh.haigaiapp.cn

N. 数据结构与算法
来源：http://qv.jctech888.com.cn

================================================================================
来源：http://kk.hahajie.cn

[N01] 二分查找（有序数组）
来源：http://ho.yuexingan06.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mc.hnjuh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ge.yuexingan06.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.hahajie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bm.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ft.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://cm.hahajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yw.muxihuayi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pv.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ug.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://jm.lnxyls.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vi.nszjky.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bd.9csxet.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bk.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://up.haigaiapp.cn

Go:   slices.Sort(arr)
来源：http://up.shtwfgs.cn

Ruby: arr.sort
来源：http://du.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zf.yuexingan06.cn

[N03] 快速排序（分治示例）
来源：http://sh.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://mv.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ud.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yq.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tb.huixiangedu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://in.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xa.shtwfgs.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bt.9csxet.cn

[N04] 斐波那契数列
来源：http://cx.wgjwhj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zi.newstarts.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ju.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gn.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ey.asd995.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rr.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sp.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://un.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ra.521024.cn

[N05] 最大公约数
来源：http://wg.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://yq.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ti.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gp.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tc.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ey.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ht.gzmigu.cn

Ruby: a.gcd(b)
来源：http://uj.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yr.newstarts.cn

[N06] 判断回文字符串
来源：http://qt.nicolike.cn

Py:   s == s[::-1]
来源：http://ol.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://yj.9csxet.cn

JS:   s === [...s].reverse().join("")
来源：http://uh.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://bn.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://in.hahajie.cn

Go:   // 双指针从两端比较
来源：http://sa.colortex.cn

Ruby: s == s.reverse
来源：http://rb.szsharing.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zh.shtwfgs.cn

[N07] 两数之和（返回下标）
来源：http://td.521024.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cx.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fj.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cs.szsharing.cn

TS:   // 手写 Map<string, number>
来源：http://eg.gzmigu.cn

Java: // 手写 HashMap
来源：http://ba.521024.cn

Go:   // 手写 map[int]int
来源：http://rd.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://dv.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aq.shxzskj.cn

[N08] 生成全排列
来源：http://ab.hahajie.cn

Py:   itertools.permutations(arr)
来源：http://ni.colortex.cn

PHP:  // 手写递归交换
来源：http://ft.szxytkj.cn

JS:   // 手写回溯递归
来源：http://qy.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://wj.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://bo.asd995.cn

Go:   // 手写回溯递归
来源：http://al.szxytkj.cn

Ruby: arr.permutation.to_a
来源：http://qm.huanxung.cn

C#:   // 手写回溯递归
来源：http://wm.nicolike.cn

[N09] 栈与队列
来源：http://ez.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ga.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hb.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gg.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yo.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ic.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nx.szsharing.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fi.jctech888.com.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://of.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://sr.huanxung.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ps.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tc.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oi.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ie.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://uz.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xt.asd995.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xg.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bn.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://pf.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iy.chemitech.net.cn

PHP:  // 手写递归函数
来源：http://cb.huixiangedu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jc.shxzskj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wj.jianghongdianzi.cn

Java: // 手写递归
来源：http://wg.panjiajie.cn

Go:   // 手写递归
来源：http://nd.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://up.shxzskj.cn

C#:   // 手写递归
来源：http://sb.panjiajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fl.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sw.panjiajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ni.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://to.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xz.colortex.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bm.szsharing.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yb.yuexingan06.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mk.nszjky.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://as.yuntaijiaju.cn

================================================================================
来源：http://yz.huanxung.cn

O. 并发与异步
来源：http://az.yuntaijiaju.cn

================================================================================
来源：http://ib.chemitech.net.cn

[O01] 启动一个线程
来源：http://wa.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tk.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tn.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nh.shxzskj.cn

TS:   // 同 JS
来源：http://xq.yuexingan06.cn

Java: new Thread(() -> f()).start()
来源：http://zg.szxytkj.cn

Go:   go f()
来源：http://up.hahajie.cn

Ruby: Thread.new { f }
来源：http://ci.wgjwhj.cn

C#:   Task.Run(() => F());
来源：http://bw.jianghongdianzi.cn

[O02] 使用线程池
来源：http://as.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bj.jctech888.com.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://km.shxzukj.cn

JS:   // worker_threads 线程池
来源：http://mh.szsharing.cn

TS:   // worker_threads 线程池
来源：http://ak.asd995.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zs.nicolike.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nr.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ha.asd995.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://th.gzmigu.cn

[O03] 加锁保护共享数据
来源：http://ms.hnjuh.cn

Py:   with lock: shared += 1
来源：http://gi.huixinmuqiang.cn

PHP:  // 用 flock() 做文件锁
来源：http://ar.shtwfgs.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://il.bjjhwx.cn

TS:   // 同 JS
来源：http://zl.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://ll.haigaiapp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vs.huanxung.cn


<!-- 参考信息 -->