代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ej.bjjhwx.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zy.shxzskj.cn

[K08] 二进制序列化（非 JSON）
来源：http://ii.yuntaijiaju.cn

Py:   pickle.dumps(obj)
来源：http://ew.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jj.muxihuayi.cn

JS:   v8.serialize(obj)        // Node
来源：http://zj.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://ow.nicolike.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jz.yuntaijiaju.cn

Go:   encoding/gob
来源：http://as.colortex.cn

Ruby: Marshal.dump(obj)
来源：http://gf.9csxet.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jc.gzmigu.cn

================================================================================
来源：http://df.newstarts.cn

L. 网络请求
来源：http://us.yuntaijiaju.cn

================================================================================
来源：http://mk.asd995.cn

[L01] 发送 GET 请求
来源：http://ws.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dh.huixiangedu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bd.bookmarksfly.cn

JS:   await fetch(url)
来源：http://il.nicolike.cn

TS:   await fetch(url)
来源：http://ga.nicolike.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uo.jianghongdianzi.cn

Go:   resp, err := http.Get(url)
来源：http://ch.bjjhwx.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://rj.521024.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://fw.521024.cn

[L02] 发送 POST JSON
来源：http://fz.9csxet.cn

Py:   requests.post(url, json={"a": 1})
来源：http://qw.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jg.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://iw.haigaiapp.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ys.szxytkj.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ht.wgjwhj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ho.nszjky.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jh.gzmigu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pm.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://xi.shxzukj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rw.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gt.haigaiapp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tc.bjjhwx.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://me.nicolike.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yf.gzmigu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cn.nicolike.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eu.panjiajie.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ds.hnjuh.cn

[L04] 设置超时
来源：http://sq.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://rz.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ny.shxzskj.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tt.shxzskj.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://py.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://of.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nr.szxytkj.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cd.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uk.newstarts.cn

[L05] 上传文件（multipart）
来源：http://lc.hahajie.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pv.haigaiapp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rt.wgjwhj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fw.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hi.newstarts.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pi.colortex.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fs.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://il.jianghongdianzi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fe.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://wv.yuntaijiaju.cn

Py:   resp.json()
来源：http://cm.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://md.yuexingan06.cn

JS:   await resp.json()
来源：http://nj.bjjhwx.cn

TS:   await resp.json()
来源：http://zh.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aa.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bv.jianghongdianzi.cn

Ruby: JSON.parse(resp.body)
来源：http://kh.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kz.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://sh.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://co.huixinmuqiang.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ss.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://uh.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://iu.chemitech.net.cn

Java: resp.statusCode()
来源：http://sb.chemitech.net.cn

Go:   resp.StatusCode
来源：http://gr.szsharing.cn

Ruby: resp.code.to_i
来源：http://yn.huixiangedu.cn

C#:   (int)resp.StatusCode
来源：http://pb.wgjwhj.cn

[L08] 并发请求多个地址
来源：http://on.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zd.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://pj.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bl.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lv.jctech888.com.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pa.bookmarksfly.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://uk.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dn.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gs.yuntaijiaju.cn

================================================================================
来源：http://ej.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://gg.shxzskj.cn

================================================================================
来源：http://dd.huixiangedu.cn

[M01] 读取命令行参数
来源：http://rc.521024.cn

Py:   sys.argv[1:]
来源：http://cm.521024.cn

PHP:  $argv;  $argc;
来源：http://fd.huanxung.cn

JS:   process.argv.slice(2)
来源：http://bj.nicolike.cn

TS:   process.argv.slice(2)
来源：http://vu.shtwfgs.cn

Java: args 数组（main 方法参数）
来源：http://mi.yuexingan06.cn

Go:   os.Args[1:]
来源：http://qw.haigaiapp.cn

Ruby: ARGV
来源：http://ff.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://qs.bookmarksfly.cn

[M02] 读取环境变量
来源：http://yc.huixinmuqiang.cn

Py:   os.environ.get("HOME")
来源：http://ke.521024.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://sg.hahajie.cn

JS:   process.env.HOME
来源：http://eo.shtwfgs.cn

TS:   process.env.HOME
来源：http://hk.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://ab.jctech888.com.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sy.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://pr.shxzskj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dc.newstarts.cn

[M03] 执行外部命令
来源：http://qx.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tn.yuexingan06.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yj.nszjky.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oz.nicolike.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ga.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fe.huanxung.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zp.jianghongdianzi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tk.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://aq.hahajie.cn

[M04] 获取当前工作目录
来源：http://zy.shtwfgs.cn

Py:   os.getcwd()
来源：http://gk.jianghongdianzi.cn

PHP:  getcwd();
来源：http://wu.yuexingan06.cn

JS:   process.cwd()
来源：http://ya.jianghongdianzi.cn

TS:   process.cwd()
来源：http://pe.hnjuh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ou.haigaiapp.cn

Go:   os.Getwd()
来源：http://ak.jctech888.com.cn

Ruby: Dir.pwd
来源：http://ub.hahajie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gl.szsharing.cn

[M05] 设置退出码
来源：http://or.jctech888.com.cn

Py:   sys.exit(1)
来源：http://ze.newstarts.cn

PHP:  exit(1);
来源：http://em.huixiangedu.cn

JS:   process.exit(1)
来源：http://hx.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://uq.521024.cn

Java: System.exit(1)
来源：http://sz.szsharing.cn

Go:   os.Exit(1)
来源：http://bi.huixinmuqiang.cn

Ruby: exit 1
来源：http://tz.chemitech.net.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eu.gzmigu.cn

[M06] 向标准错误输出
来源：http://ee.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://bi.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bs.nszjky.cn

JS:   console.error("err")
来源：http://zq.nicolike.cn

TS:   console.error("err")
来源：http://ep.shxzukj.cn

Java: System.err.println("err")
来源：http://ay.shtwfgs.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ap.newstarts.cn

Ruby: warn "err"
来源：http://kl.szsharing.cn

C#:   Console.Error.WriteLine("err")
来源：http://tr.asd995.cn

[M07] 判断是否为主入口
来源：http://ub.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://jn.panjiajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gp.shxzukj.cn

JS:   require.main === module
来源：http://ad.panjiajie.cn

TS:   require.main === module
来源：http://ar.hnjuh.cn

Java: public static void main(String[] args)
来源：http://nj.bookmarksfly.cn

Go:   func main()
来源：http://wi.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mm.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://xi.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://xd.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://kx.lnxyls.cn

PHP:  PHP_OS;  phpversion();
来源：http://eh.chemitech.net.cn

JS:   process.platform;  process.version
来源：http://rl.nicolike.cn

TS:   process.platform;  process.version
来源：http://yw.bjjhwx.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ew.nszjky.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yj.colortex.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dk.haigaiapp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zq.bjjhwx.cn

================================================================================
来源：http://yg.521024.cn

N. 数据结构与算法
来源：http://pa.521024.cn

================================================================================
来源：http://fc.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://cf.jianghongdianzi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ru.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://im.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ap.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zc.huanxung.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qo.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://en.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ul.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ph.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://au.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://dy.bookmarksfly.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tj.muxihuayi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tk.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tz.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ep.huixinmuqiang.cn

Go:   slices.Sort(arr)
来源：http://rf.panjiajie.cn

Ruby: arr.sort
来源：http://en.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://il.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://et.huanxung.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eq.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://vb.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bo.gzmigu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://su.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://is.shtwfgs.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dm.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fu.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mt.nicolike.cn

[N04] 斐波那契数列
来源：http://ql.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://im.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ra.huanxung.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ft.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jv.shxzukj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vp.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uq.nszjky.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bi.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xa.bjjhwx.cn

[N05] 最大公约数
来源：http://ig.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://lm.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qc.nicolike.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jh.yuntaijiaju.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gj.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tq.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pz.nszjky.cn

Ruby: a.gcd(b)
来源：http://us.nszjky.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://of.yuexingan06.cn

[N06] 判断回文字符串
来源：http://qz.shxzukj.cn

Py:   s == s[::-1]
来源：http://pe.521024.cn

PHP:  $s === strrev($s);
来源：http://mp.haigaiapp.cn

JS:   s === [...s].reverse().join("")
来源：http://yy.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://ur.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ra.nszjky.cn

Go:   // 双指针从两端比较
来源：http://fj.wgjwhj.cn

Ruby: s == s.reverse
来源：http://bf.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ui.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://bq.huixiangedu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ka.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kv.newstarts.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ub.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://qq.chemitech.net.cn

Java: // 手写 HashMap
来源：http://ct.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://wb.panjiajie.cn

Ruby: // 手写 Hash
来源：http://oi.shxzukj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://th.521024.cn

[N08] 生成全排列
来源：http://rh.panjiajie.cn

Py:   itertools.permutations(arr)
来源：http://vw.nszjky.cn

PHP:  // 手写递归交换
来源：http://gq.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://zf.szxytkj.cn

TS:   // 手写回溯递归
来源：http://wl.521024.cn

Java: // 手写回溯递归
来源：http://cc.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://jp.yuntaijiaju.cn

Ruby: arr.permutation.to_a
来源：http://wq.gzmigu.cn

C#:   // 手写回溯递归
来源：http://jg.nszjky.cn

[N09] 栈与队列
来源：http://qx.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zd.9csxet.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ud.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rx.chemitech.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vc.shxzskj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ce.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ly.jianghongdianzi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tj.nicolike.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://if.jctech888.com.cn

[N10] 链表节点定义
来源：http://ik.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ls.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gg.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://id.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jo.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://lb.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ya.colortex.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xw.shxzukj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://mn.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://wd.hnjuh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mq.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://gx.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qr.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jy.gzmigu.cn

Java: // 手写递归
来源：http://si.muxihuayi.cn

Go:   // 手写递归
来源：http://ir.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hb.huixinmuqiang.cn

C#:   // 手写递归
来源：http://vv.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zj.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ov.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jr.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bc.wgjwhj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fk.chemitech.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yn.wgjwhj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cs.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bu.nicolike.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://km.newstarts.cn

================================================================================
来源：http://fc.asd995.cn

O. 并发与异步
来源：http://iq.shxzskj.cn

================================================================================
来源：http://lu.nicolike.cn

[O01] 启动一个线程
来源：http://pe.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vm.newstarts.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://du.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lo.asd995.cn

TS:   // 同 JS
来源：http://kq.colortex.cn

Java: new Thread(() -> f()).start()
来源：http://gw.wgjwhj.cn

Go:   go f()
来源：http://hk.szsharing.cn

Ruby: Thread.new { f }
来源：http://nt.haigaiapp.cn

C#:   Task.Run(() => F());
来源：http://ba.haigaiapp.cn

[O02] 使用线程池
来源：http://wr.bjjhwx.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sj.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zc.521024.cn

JS:   // worker_threads 线程池
来源：http://lh.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://ur.jctech888.com.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lc.chemitech.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gk.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mx.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cr.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://rk.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://av.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://jv.szsharing.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ku.chemitech.net.cn

TS:   // 同 JS
来源：http://qu.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://xl.hahajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fz.shxzukj.cn


<!-- 参考信息 -->