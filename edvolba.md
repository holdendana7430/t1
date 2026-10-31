代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ks.jianghongdianzi.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sr.yuexingan06.cn

[K08] 二进制序列化（非 JSON）
来源：http://dr.hnjuh.cn

Py:   pickle.dumps(obj)
来源：http://mz.jctech888.com.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zg.asd995.cn

JS:   v8.serialize(obj)        // Node
来源：http://vi.521024.cn

TS:   v8.serialize(obj)        // Node
来源：http://hk.muxihuayi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ff.shtwfgs.cn

Go:   encoding/gob
来源：http://pk.shxzskj.cn

Ruby: Marshal.dump(obj)
来源：http://bc.jctech888.com.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ot.huixinmuqiang.cn

================================================================================
来源：http://gs.hahajie.cn

L. 网络请求
来源：http://is.asd995.cn

================================================================================
来源：http://wn.wgjwhj.cn

[L01] 发送 GET 请求
来源：http://gq.chemitech.net.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://js.nicolike.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://br.yuntaijiaju.cn

JS:   await fetch(url)
来源：http://kj.hahajie.cn

TS:   await fetch(url)
来源：http://et.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yc.huanxung.cn

Go:   resp, err := http.Get(url)
来源：http://fp.nicolike.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xa.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oa.asd995.cn

[L02] 发送 POST JSON
来源：http://xz.bookmarksfly.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xe.huixiangedu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sc.szsharing.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tn.yuexingan06.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ry.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wu.bjjhwx.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ji.shxzukj.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ay.szxytkj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ra.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ma.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qv.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ya.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uz.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rv.hnjuh.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aa.yuexingan06.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xa.jianghongdianzi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://yl.lnxyls.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gv.nszjky.cn

[L04] 设置超时
来源：http://kb.huixinmuqiang.cn

Py:   requests.get(url, timeout=5)
来源：http://jw.shxzukj.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uk.wgjwhj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cq.lnxyls.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iz.jianghongdianzi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tz.jctech888.com.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mh.asd995.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jr.huanxung.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kg.lnxyls.cn

[L05] 上传文件（multipart）
来源：http://rg.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bn.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://br.bjjhwx.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uh.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://th.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gm.shtwfgs.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gd.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lj.huanxung.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dj.bookmarksfly.cn

[L06] 解析响应为 JSON
来源：http://wh.hnjuh.cn

Py:   resp.json()
来源：http://gl.521024.cn

PHP:  json_decode($body, true);
来源：http://ta.panjiajie.cn

JS:   await resp.json()
来源：http://wn.hahajie.cn

TS:   await resp.json()
来源：http://kv.huixiangedu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://my.huanxung.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sz.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://xx.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://is.hahajie.cn

[L07] 处理 HTTP 状态码
来源：http://bz.panjiajie.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://be.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xk.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://ws.panjiajie.cn

TS:   resp.ok;  resp.status
来源：http://dk.shxzskj.cn

Java: resp.statusCode()
来源：http://wk.huixiangedu.cn

Go:   resp.StatusCode
来源：http://nk.newstarts.cn

Ruby: resp.code.to_i
来源：http://hj.yuntaijiaju.cn

C#:   (int)resp.StatusCode
来源：http://xb.huanxung.cn

[L08] 并发请求多个地址
来源：http://oj.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://me.nicolike.cn

PHP:  curl_multi_init() 系列
来源：http://dl.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kl.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jt.hnjuh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://un.521024.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://se.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qa.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://at.newstarts.cn

================================================================================
来源：http://dz.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://xc.jianghongdianzi.cn

================================================================================
来源：http://jo.panjiajie.cn

[M01] 读取命令行参数
来源：http://uk.wgjwhj.cn

Py:   sys.argv[1:]
来源：http://xo.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://gf.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://ig.yuntaijiaju.cn

TS:   process.argv.slice(2)
来源：http://tn.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://ag.newstarts.cn

Go:   os.Args[1:]
来源：http://eh.521024.cn

Ruby: ARGV
来源：http://ok.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://sn.gzmigu.cn

[M02] 读取环境变量
来源：http://lu.nicolike.cn

Py:   os.environ.get("HOME")
来源：http://gg.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ii.yuexingan06.cn

JS:   process.env.HOME
来源：http://nk.yuexingan06.cn

TS:   process.env.HOME
来源：http://jk.shtwfgs.cn

Java: System.getenv("HOME")
来源：http://qr.hahajie.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jt.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://ii.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gk.521024.cn

[M03] 执行外部命令
来源：http://wv.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mi.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ls.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ay.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fa.9csxet.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tq.asd995.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xq.shtwfgs.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ac.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://dz.wgjwhj.cn

[M04] 获取当前工作目录
来源：http://wi.nszjky.cn

Py:   os.getcwd()
来源：http://mn.asd995.cn

PHP:  getcwd();
来源：http://vm.asd995.cn

JS:   process.cwd()
来源：http://uo.yuexingan06.cn

TS:   process.cwd()
来源：http://ud.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://lw.asd995.cn

Go:   os.Getwd()
来源：http://ds.nszjky.cn

Ruby: Dir.pwd
来源：http://oi.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://mc.nszjky.cn

[M05] 设置退出码
来源：http://jk.nicolike.cn

Py:   sys.exit(1)
来源：http://ra.hnjuh.cn

PHP:  exit(1);
来源：http://ms.szxytkj.cn

JS:   process.exit(1)
来源：http://pm.shxzukj.cn

TS:   process.exit(1)
来源：http://om.huixinmuqiang.cn

Java: System.exit(1)
来源：http://ba.521024.cn

Go:   os.Exit(1)
来源：http://ff.wgjwhj.cn

Ruby: exit 1
来源：http://bp.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ah.nszjky.cn

[M06] 向标准错误输出
来源：http://co.lnxyls.cn

Py:   print("err", file=sys.stderr)
来源：http://wj.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qt.wgjwhj.cn

JS:   console.error("err")
来源：http://ou.gzmigu.cn

TS:   console.error("err")
来源：http://da.huanxung.cn

Java: System.err.println("err")
来源：http://ei.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fp.nszjky.cn

Ruby: warn "err"
来源：http://cd.hahajie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.shxzskj.cn

[M07] 判断是否为主入口
来源：http://hp.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://cq.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://af.jianghongdianzi.cn

JS:   require.main === module
来源：http://de.jctech888.com.cn

TS:   require.main === module
来源：http://pa.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://sl.huixinmuqiang.cn

Go:   func main()
来源：http://zo.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://so.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://fj.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://yx.bjjhwx.cn

Py:   platform.system();  platform.python_version()
来源：http://ej.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://eq.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://wd.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://qf.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wq.huixiangedu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kt.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mm.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vk.haigaiapp.cn

================================================================================
来源：http://ym.muxihuayi.cn

N. 数据结构与算法
来源：http://zz.lnxyls.cn

================================================================================
来源：http://pp.jianghongdianzi.cn

[N01] 二分查找（有序数组）
来源：http://sd.bjjhwx.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sv.lnxyls.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://za.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ws.huixinmuqiang.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tu.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://lg.gzmigu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://on.bjjhwx.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gu.huanxung.cn

[N02] 排序（工程实践用内置实现）
来源：http://nu.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://cr.muxihuayi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pi.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ic.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bj.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qn.nicolike.cn

Go:   slices.Sort(arr)
来源：http://lb.shxzukj.cn

Ruby: arr.sort
来源：http://kh.panjiajie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pq.yuntaijiaju.cn

[N03] 快速排序（分治示例）
来源：http://vi.jctech888.com.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ro.yuexingan06.cn

PHP:  // 递归实现，或用 usort
来源：http://fq.yuntaijiaju.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fj.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bv.shxzskj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ua.szsharing.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sf.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zj.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://la.panjiajie.cn

[N04] 斐波那契数列
来源：http://ax.jctech888.com.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cm.szsharing.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bz.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zx.jianghongdianzi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ez.panjiajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sy.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sq.haigaiapp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eo.muxihuayi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tr.chemitech.net.cn

[N05] 最大公约数
来源：http://ng.bjjhwx.cn

Py:   math.gcd(a, b)
来源：http://fz.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://la.newstarts.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://du.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zl.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jf.jctech888.com.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hv.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://sf.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://re.colortex.cn

[N06] 判断回文字符串
来源：http://er.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://lo.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://vs.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://qn.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://an.bjjhwx.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qg.bjjhwx.cn

Go:   // 双指针从两端比较
来源：http://ev.gzmigu.cn

Ruby: s == s.reverse
来源：http://yi.shxzukj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yb.nszjky.cn

[N07] 两数之和（返回下标）
来源：http://iz.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ab.lnxyls.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wb.nicolike.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cz.haigaiapp.cn

TS:   // 手写 Map<string, number>
来源：http://xf.yuexingan06.cn

Java: // 手写 HashMap
来源：http://wg.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://bl.huixinmuqiang.cn

Ruby: // 手写 Hash
来源：http://ab.hahajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rd.nicolike.cn

[N08] 生成全排列
来源：http://sd.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://gp.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://ue.shxzukj.cn

JS:   // 手写回溯递归
来源：http://wd.szxytkj.cn

TS:   // 手写回溯递归
来源：http://td.huanxung.cn

Java: // 手写回溯递归
来源：http://ns.nszjky.cn

Go:   // 手写回溯递归
来源：http://al.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ny.nicolike.cn

C#:   // 手写回溯递归
来源：http://qc.shxzukj.cn

[N09] 栈与队列
来源：http://sy.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sa.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dw.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qf.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yv.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cz.panjiajie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wn.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ro.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rn.yuntaijiaju.cn

[N10] 链表节点定义
来源：http://zh.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bn.hahajie.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bl.szxytkj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xo.lnxyls.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yg.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://qc.huixinmuqiang.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gn.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ui.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ki.huanxung.cn

[N11] 二叉树中序遍历
来源：http://nl.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fo.shtwfgs.cn

PHP:  // 手写递归函数
来源：http://kd.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ez.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nw.shtwfgs.cn

Java: // 手写递归
来源：http://sc.yuntaijiaju.cn

Go:   // 手写递归
来源：http://eh.521024.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ax.asd995.cn

C#:   // 手写递归
来源：http://rv.shtwfgs.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vm.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ji.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vd.shtwfgs.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zr.huixinmuqiang.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ya.huixinmuqiang.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rb.huixinmuqiang.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hv.bjjhwx.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ai.lnxyls.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kf.szsharing.cn

================================================================================
来源：http://ks.huanxung.cn

O. 并发与异步
来源：http://bf.huixiangedu.cn

================================================================================
来源：http://vk.panjiajie.cn

[O01] 启动一个线程
来源：http://ms.521024.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zq.huixinmuqiang.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://em.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ah.9csxet.cn

TS:   // 同 JS
来源：http://sq.jianghongdianzi.cn

Java: new Thread(() -> f()).start()
来源：http://kg.9csxet.cn

Go:   go f()
来源：http://eh.muxihuayi.cn

Ruby: Thread.new { f }
来源：http://hj.yuexingan06.cn

C#:   Task.Run(() => F());
来源：http://dq.huanxung.cn

[O02] 使用线程池
来源：http://fh.huixiangedu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yg.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sr.wgjwhj.cn

JS:   // worker_threads 线程池
来源：http://on.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://vz.szxytkj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ty.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sc.nszjky.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vu.521024.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ni.panjiajie.cn

[O03] 加锁保护共享数据
来源：http://nb.huixinmuqiang.cn

Py:   with lock: shared += 1
来源：http://ob.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://ki.hnjuh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://km.nicolike.cn

TS:   // 同 JS
来源：http://lv.nicolike.cn

Java: synchronized (this) { shared++; }
来源：http://vq.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ey.szxytkj.cn


<!-- 参考信息 -->