代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tf.chemitech.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yo.521024.cn

[K08] 二进制序列化（非 JSON）
来源：http://yj.shxzukj.cn

Py:   pickle.dumps(obj)
来源：http://cj.nicolike.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tu.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://re.lnxyls.cn

TS:   v8.serialize(obj)        // Node
来源：http://la.gzmigu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://en.bookmarksfly.cn

Go:   encoding/gob
来源：http://zw.asd995.cn

Ruby: Marshal.dump(obj)
来源：http://jf.521024.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://up.jianghongdianzi.cn

================================================================================
来源：http://bt.asd995.cn

L. 网络请求
来源：http://de.wgjwhj.cn

================================================================================
来源：http://ad.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://nm.hnjuh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oc.hnjuh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pp.hahajie.cn

JS:   await fetch(url)
来源：http://in.9csxet.cn

TS:   await fetch(url)
来源：http://ss.9csxet.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ls.haigaiapp.cn

Go:   resp, err := http.Get(url)
来源：http://oy.lnxyls.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://cx.szxytkj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jn.shxzukj.cn

[L02] 发送 POST JSON
来源：http://io.yuexingan06.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nu.hnjuh.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://po.shxzukj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fx.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ow.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ya.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://po.huixiangedu.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fm.wgjwhj.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ez.yuntaijiaju.cn

[L03] 设置自定义请求头
来源：http://qa.jianghongdianzi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sq.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ju.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zg.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tp.bookmarksfly.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://el.huixiangedu.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jm.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://el.huanxung.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pm.huanxung.cn

[L04] 设置超时
来源：http://re.szsharing.cn

Py:   requests.get(url, timeout=5)
来源：http://xp.nicolike.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gl.asd995.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://du.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jq.huixiangedu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qe.hahajie.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://km.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mb.huixiangedu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lt.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://mf.wgjwhj.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hn.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hu.szxytkj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qk.hnjuh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dr.shxzskj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xt.jianghongdianzi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gu.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://km.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://eh.huanxung.cn

[L06] 解析响应为 JSON
来源：http://en.9csxet.cn

Py:   resp.json()
来源：http://yh.bjjhwx.cn

PHP:  json_decode($body, true);
来源：http://xj.gzmigu.cn

JS:   await resp.json()
来源：http://ur.9csxet.cn

TS:   await resp.json()
来源：http://nk.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zg.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xe.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://cs.hnjuh.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qf.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://ks.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qo.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://re.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://zt.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://pd.lnxyls.cn

Java: resp.statusCode()
来源：http://qf.huixiangedu.cn

Go:   resp.StatusCode
来源：http://nj.9csxet.cn

Ruby: resp.code.to_i
来源：http://gd.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://nq.shtwfgs.cn

[L08] 并发请求多个地址
来源：http://pn.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vd.yuexingan06.cn

PHP:  curl_multi_init() 系列
来源：http://cd.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://po.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hf.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xi.haigaiapp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zh.gzmigu.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rn.9csxet.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fk.bookmarksfly.cn

================================================================================
来源：http://ap.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://dl.jianghongdianzi.cn

================================================================================
来源：http://ek.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://rr.shtwfgs.cn

Py:   sys.argv[1:]
来源：http://ga.yuntaijiaju.cn

PHP:  $argv;  $argc;
来源：http://gc.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://nt.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://un.gzmigu.cn

Java: args 数组（main 方法参数）
来源：http://dk.huixiangedu.cn

Go:   os.Args[1:]
来源：http://ar.muxihuayi.cn

Ruby: ARGV
来源：http://mq.hnjuh.cn

C#:   args 数组（Main 方法参数）
来源：http://fm.huanxung.cn

[M02] 读取环境变量
来源：http://lg.shtwfgs.cn

Py:   os.environ.get("HOME")
来源：http://zh.haigaiapp.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mv.hnjuh.cn

JS:   process.env.HOME
来源：http://wz.haigaiapp.cn

TS:   process.env.HOME
来源：http://nh.szsharing.cn

Java: System.getenv("HOME")
来源：http://yy.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vk.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://nb.asd995.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fm.yuexingan06.cn

[M03] 执行外部命令
来源：http://hq.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vd.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xm.521024.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pj.panjiajie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://cg.asd995.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ew.shxzukj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nk.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bp.huixiangedu.cn

C#:   Process.Start("ls", "-l");
来源：http://dp.bjjhwx.cn

[M04] 获取当前工作目录
来源：http://uv.huanxung.cn

Py:   os.getcwd()
来源：http://xl.panjiajie.cn

PHP:  getcwd();
来源：http://wn.yuexingan06.cn

JS:   process.cwd()
来源：http://ek.chemitech.net.cn

TS:   process.cwd()
来源：http://lz.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://af.shtwfgs.cn

Go:   os.Getwd()
来源：http://yb.szxytkj.cn

Ruby: Dir.pwd
来源：http://th.bookmarksfly.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rr.gzmigu.cn

[M05] 设置退出码
来源：http://ku.szxytkj.cn

Py:   sys.exit(1)
来源：http://lj.jianghongdianzi.cn

PHP:  exit(1);
来源：http://pr.yuexingan06.cn

JS:   process.exit(1)
来源：http://sn.szsharing.cn

TS:   process.exit(1)
来源：http://yd.hnjuh.cn

Java: System.exit(1)
来源：http://hh.asd995.cn

Go:   os.Exit(1)
来源：http://lt.chemitech.net.cn

Ruby: exit 1
来源：http://dp.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zp.szxytkj.cn

[M06] 向标准错误输出
来源：http://st.wgjwhj.cn

Py:   print("err", file=sys.stderr)
来源：http://nz.bjjhwx.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yw.huixinmuqiang.cn

JS:   console.error("err")
来源：http://rn.chemitech.net.cn

TS:   console.error("err")
来源：http://zk.panjiajie.cn

Java: System.err.println("err")
来源：http://mc.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zx.newstarts.cn

Ruby: warn "err"
来源：http://nh.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://iy.newstarts.cn

[M07] 判断是否为主入口
来源：http://wq.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://jc.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kr.chemitech.net.cn

JS:   require.main === module
来源：http://sy.yuntaijiaju.cn

TS:   require.main === module
来源：http://oc.nicolike.cn

Java: public static void main(String[] args)
来源：http://ri.yuntaijiaju.cn

Go:   func main()
来源：http://ls.huanxung.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bg.asd995.cn

C#:   static void Main(string[] args)
来源：http://tr.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://kq.shtwfgs.cn

Py:   platform.system();  platform.python_version()
来源：http://yw.shxzukj.cn

PHP:  PHP_OS;  phpversion();
来源：http://xy.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://zy.jctech888.com.cn

TS:   process.platform;  process.version
来源：http://oz.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pb.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sr.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oj.colortex.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nd.huixiangedu.cn

================================================================================
来源：http://yc.asd995.cn

N. 数据结构与算法
来源：http://ib.lnxyls.cn

================================================================================
来源：http://ic.lnxyls.cn

[N01] 二分查找（有序数组）
来源：http://ky.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://tw.shxzukj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://te.shxzukj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aa.bjjhwx.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kc.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zq.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://fu.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zp.shxzskj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://li.nicolike.cn

[N02] 排序（工程实践用内置实现）
来源：http://fz.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://yc.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tj.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ao.newstarts.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gm.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mv.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://iq.wgjwhj.cn

Ruby: arr.sort
来源：http://lp.szxytkj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hy.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://ax.yuntaijiaju.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fh.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://nx.huanxung.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xi.wgjwhj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ik.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gk.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lz.asd995.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lh.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aw.shtwfgs.cn

[N04] 斐波那契数列
来源：http://zn.yuntaijiaju.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mh.nszjky.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://is.bjjhwx.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oi.huanxung.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zs.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ni.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fa.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fz.bookmarksfly.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://an.bookmarksfly.cn

[N05] 最大公约数
来源：http://uy.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://jx.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jw.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gl.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zc.shxzskj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qo.bookmarksfly.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jh.yuntaijiaju.cn

Ruby: a.gcd(b)
来源：http://uj.bookmarksfly.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://za.newstarts.cn

[N06] 判断回文字符串
来源：http://ec.asd995.cn

Py:   s == s[::-1]
来源：http://dk.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://ly.hahajie.cn

JS:   s === [...s].reverse().join("")
来源：http://kt.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://uw.szsharing.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yy.colortex.cn

Go:   // 双指针从两端比较
来源：http://nv.yuexingan06.cn

Ruby: s == s.reverse
来源：http://bi.lnxyls.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://md.yuntaijiaju.cn

[N07] 两数之和（返回下标）
来源：http://la.jianghongdianzi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mh.shtwfgs.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hw.jctech888.com.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ek.muxihuayi.cn

TS:   // 手写 Map<string, number>
来源：http://ms.szsharing.cn

Java: // 手写 HashMap
来源：http://bg.hnjuh.cn

Go:   // 手写 map[int]int
来源：http://ji.nszjky.cn

Ruby: // 手写 Hash
来源：http://kj.colortex.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tz.jianghongdianzi.cn

[N08] 生成全排列
来源：http://rc.huixiangedu.cn

Py:   itertools.permutations(arr)
来源：http://oi.hahajie.cn

PHP:  // 手写递归交换
来源：http://jc.nicolike.cn

JS:   // 手写回溯递归
来源：http://dm.newstarts.cn

TS:   // 手写回溯递归
来源：http://aj.szsharing.cn

Java: // 手写回溯递归
来源：http://ss.szsharing.cn

Go:   // 手写回溯递归
来源：http://qw.nszjky.cn

Ruby: arr.permutation.to_a
来源：http://qc.szsharing.cn

C#:   // 手写回溯递归
来源：http://vd.hahajie.cn

[N09] 栈与队列
来源：http://zg.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ku.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yc.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ex.521024.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qo.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wz.hnjuh.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eq.muxihuayi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hb.9csxet.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xt.bookmarksfly.cn

[N10] 链表节点定义
来源：http://wo.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vl.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tl.panjiajie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ji.szxytkj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ki.lnxyls.cn

Java: class Node { int v; Node next; }
来源：http://vg.bjjhwx.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kv.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ys.gzmigu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ju.nicolike.cn

[N11] 二叉树中序遍历
来源：http://fq.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fx.9csxet.cn

PHP:  // 手写递归函数
来源：http://kl.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wy.jianghongdianzi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fr.szxytkj.cn

Java: // 手写递归
来源：http://dv.yuntaijiaju.cn

Go:   // 手写递归
来源：http://sc.nszjky.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://he.haigaiapp.cn

C#:   // 手写递归
来源：http://no.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ph.szsharing.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tg.szxytkj.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ho.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hr.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uy.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yc.lnxyls.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fs.wgjwhj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ah.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bt.hahajie.cn

================================================================================
来源：http://wb.wgjwhj.cn

O. 并发与异步
来源：http://gl.jctech888.com.cn

================================================================================
来源：http://sh.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://bg.asd995.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vb.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sh.wgjwhj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qq.colortex.cn

TS:   // 同 JS
来源：http://na.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://zd.jianghongdianzi.cn

Go:   go f()
来源：http://yk.newstarts.cn

Ruby: Thread.new { f }
来源：http://jj.colortex.cn

C#:   Task.Run(() => F());
来源：http://bx.asd995.cn

[O02] 使用线程池
来源：http://hv.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cg.panjiajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yo.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wh.521024.cn

TS:   // worker_threads 线程池
来源：http://gt.nszjky.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eg.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lt.shtwfgs.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zn.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tp.521024.cn

[O03] 加锁保护共享数据
来源：http://fp.gzmigu.cn

Py:   with lock: shared += 1
来源：http://yh.bjjhwx.cn

PHP:  // 用 flock() 做文件锁
来源：http://cp.9csxet.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jg.521024.cn

TS:   // 同 JS
来源：http://wg.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://jg.jctech888.com.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ga.jctech888.com.cn


<!-- 参考信息 -->