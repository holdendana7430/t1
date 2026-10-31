代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uy.wgjwhj.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zq.jianghongdianzi.cn

[K08] 二进制序列化（非 JSON）
来源：http://ia.shxzskj.cn

Py:   pickle.dumps(obj)
来源：http://ww.gzmigu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nq.bjjhwx.cn

JS:   v8.serialize(obj)        // Node
来源：http://or.chemitech.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://lu.huanxung.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fs.newstarts.cn

Go:   encoding/gob
来源：http://mz.nszjky.cn

Ruby: Marshal.dump(obj)
来源：http://ci.yuntaijiaju.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wz.hnjuh.cn

================================================================================
来源：http://dh.yuexingan06.cn

L. 网络请求
来源：http://fk.nicolike.cn

================================================================================
来源：http://yv.haigaiapp.cn

[L01] 发送 GET 请求
来源：http://hh.jctech888.com.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tt.huixinmuqiang.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bb.colortex.cn

JS:   await fetch(url)
来源：http://uu.szxytkj.cn

TS:   await fetch(url)
来源：http://ag.nszjky.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xg.shtwfgs.cn

Go:   resp, err := http.Get(url)
来源：http://xm.jctech888.com.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://yb.shxzukj.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xc.huixinmuqiang.cn

[L02] 发送 POST JSON
来源：http://nd.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ln.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zj.shtwfgs.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vi.szxytkj.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xu.521024.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xm.panjiajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dc.521024.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ts.bjjhwx.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cq.lnxyls.cn

[L03] 设置自定义请求头
来源：http://hw.haigaiapp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fp.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://pt.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dz.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tk.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://si.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qv.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ks.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://df.newstarts.cn

[L04] 设置超时
来源：http://cm.muxihuayi.cn

Py:   requests.get(url, timeout=5)
来源：http://ne.muxihuayi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tw.huixiangedu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tz.nszjky.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ps.hnjuh.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ra.jianghongdianzi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ts.huixinmuqiang.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pe.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sp.chemitech.net.cn

[L05] 上传文件（multipart）
来源：http://kn.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hj.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fm.shxzukj.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xz.szxytkj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jr.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://om.chemitech.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hd.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ph.huixinmuqiang.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://re.huanxung.cn

[L06] 解析响应为 JSON
来源：http://rb.huixiangedu.cn

Py:   resp.json()
来源：http://sv.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ij.521024.cn

JS:   await resp.json()
来源：http://mw.newstarts.cn

TS:   await resp.json()
来源：http://cn.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cd.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ff.shxzskj.cn

Ruby: JSON.parse(resp.body)
来源：http://zd.jctech888.com.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://en.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://dr.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nk.muxihuayi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ec.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://go.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://pg.nszjky.cn

Java: resp.statusCode()
来源：http://cn.jctech888.com.cn

Go:   resp.StatusCode
来源：http://fx.nicolike.cn

Ruby: resp.code.to_i
来源：http://if.bookmarksfly.cn

C#:   (int)resp.StatusCode
来源：http://zp.bookmarksfly.cn

[L08] 并发请求多个地址
来源：http://tn.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nc.gzmigu.cn

PHP:  curl_multi_init() 系列
来源：http://cl.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://if.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nv.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gb.asd995.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://db.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yr.haigaiapp.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uo.haigaiapp.cn

================================================================================
来源：http://lv.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://ld.yuntaijiaju.cn

================================================================================
来源：http://wp.shxzskj.cn

[M01] 读取命令行参数
来源：http://cb.jctech888.com.cn

Py:   sys.argv[1:]
来源：http://hr.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://gu.colortex.cn

JS:   process.argv.slice(2)
来源：http://xo.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://tp.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://fv.huixiangedu.cn

Go:   os.Args[1:]
来源：http://rn.gzmigu.cn

Ruby: ARGV
来源：http://ou.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ms.hnjuh.cn

[M02] 读取环境变量
来源：http://mr.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://lz.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vz.shxzskj.cn

JS:   process.env.HOME
来源：http://ew.huixiangedu.cn

TS:   process.env.HOME
来源：http://rd.gzmigu.cn

Java: System.getenv("HOME")
来源：http://rp.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bi.jctech888.com.cn

Ruby: ENV["HOME"]
来源：http://ub.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wz.szxytkj.cn

[M03] 执行外部命令
来源：http://ar.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zq.jctech888.com.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oo.colortex.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mo.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vr.yuexingan06.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fm.colortex.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kh.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yo.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://zm.panjiajie.cn

[M04] 获取当前工作目录
来源：http://zm.lnxyls.cn

Py:   os.getcwd()
来源：http://ej.huanxung.cn

PHP:  getcwd();
来源：http://bw.szxytkj.cn

JS:   process.cwd()
来源：http://lg.szsharing.cn

TS:   process.cwd()
来源：http://kk.nicolike.cn

Java: Path.of("").toAbsolutePath()
来源：http://xc.newstarts.cn

Go:   os.Getwd()
来源：http://ry.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://np.muxihuayi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ny.panjiajie.cn

[M05] 设置退出码
来源：http://fe.colortex.cn

Py:   sys.exit(1)
来源：http://ij.panjiajie.cn

PHP:  exit(1);
来源：http://vt.9csxet.cn

JS:   process.exit(1)
来源：http://ux.huixiangedu.cn

TS:   process.exit(1)
来源：http://pq.bookmarksfly.cn

Java: System.exit(1)
来源：http://rg.huixiangedu.cn

Go:   os.Exit(1)
来源：http://pd.521024.cn

Ruby: exit 1
来源：http://to.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hb.szxytkj.cn

[M06] 向标准错误输出
来源：http://va.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://nx.shtwfgs.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fd.521024.cn

JS:   console.error("err")
来源：http://ie.colortex.cn

TS:   console.error("err")
来源：http://ww.newstarts.cn

Java: System.err.println("err")
来源：http://gs.newstarts.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jb.yuexingan06.cn

Ruby: warn "err"
来源：http://wu.jianghongdianzi.cn

C#:   Console.Error.WriteLine("err")
来源：http://hy.panjiajie.cn

[M07] 判断是否为主入口
来源：http://nb.colortex.cn

Py:   if __name__ == "__main__":
来源：http://rv.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://le.hahajie.cn

JS:   require.main === module
来源：http://zy.nszjky.cn

TS:   require.main === module
来源：http://mu.huanxung.cn

Java: public static void main(String[] args)
来源：http://iw.521024.cn

Go:   func main()
来源：http://hy.bookmarksfly.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sb.newstarts.cn

C#:   static void Main(string[] args)
来源：http://ua.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://ns.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://mp.chemitech.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://ua.panjiajie.cn

JS:   process.platform;  process.version
来源：http://wi.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://qi.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ef.shxzskj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sl.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iq.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dn.shxzukj.cn

================================================================================
来源：http://hh.jctech888.com.cn

N. 数据结构与算法
来源：http://co.hnjuh.cn

================================================================================
来源：http://lp.panjiajie.cn

[N01] 二分查找（有序数组）
来源：http://zp.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zk.lnxyls.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tn.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://do.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zv.shxzukj.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pv.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://iq.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xj.szxytkj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ax.hahajie.cn

[N02] 排序（工程实践用内置实现）
来源：http://mi.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://vg.hnjuh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mp.asd995.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mn.huanxung.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sx.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ii.huanxung.cn

Go:   slices.Sort(arr)
来源：http://lw.nszjky.cn

Ruby: arr.sort
来源：http://eo.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wq.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://hn.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uh.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://nv.yuexingan06.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ru.haigaiapp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lz.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hw.nicolike.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hw.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uu.9csxet.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uj.nicolike.cn

[N04] 斐波那契数列
来源：http://dv.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zp.shxzskj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sz.9csxet.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zr.shxzskj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ll.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bv.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gp.huixinmuqiang.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zo.colortex.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ne.jctech888.com.cn

[N05] 最大公约数
来源：http://yh.jianghongdianzi.cn

Py:   math.gcd(a, b)
来源：http://mh.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lf.hnjuh.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ja.szsharing.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hw.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hn.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ya.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://un.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jx.lnxyls.cn

[N06] 判断回文字符串
来源：http://ld.shxzukj.cn

Py:   s == s[::-1]
来源：http://pk.9csxet.cn

PHP:  $s === strrev($s);
来源：http://bj.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://dr.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://ph.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bi.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ln.chemitech.net.cn

Ruby: s == s.reverse
来源：http://ky.panjiajie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ev.muxihuayi.cn

[N07] 两数之和（返回下标）
来源：http://sv.bookmarksfly.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xq.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oh.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cb.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://fl.newstarts.cn

Java: // 手写 HashMap
来源：http://ai.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://dt.szxytkj.cn

Ruby: // 手写 Hash
来源：http://xh.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://fm.shxzukj.cn

[N08] 生成全排列
来源：http://an.asd995.cn

Py:   itertools.permutations(arr)
来源：http://xp.chemitech.net.cn

PHP:  // 手写递归交换
来源：http://dw.szxytkj.cn

JS:   // 手写回溯递归
来源：http://od.colortex.cn

TS:   // 手写回溯递归
来源：http://ut.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ka.colortex.cn

Go:   // 手写回溯递归
来源：http://bs.bookmarksfly.cn

Ruby: arr.permutation.to_a
来源：http://wa.szsharing.cn

C#:   // 手写回溯递归
来源：http://rz.colortex.cn

[N09] 栈与队列
来源：http://kq.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xb.wgjwhj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ra.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bu.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qq.jctech888.com.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bj.asd995.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ec.colortex.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://py.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ld.jctech888.com.cn

[N10] 链表节点定义
来源：http://vr.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vt.nszjky.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gq.521024.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cl.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mc.huixinmuqiang.cn

Java: class Node { int v; Node next; }
来源：http://am.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sd.shxzukj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bf.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nn.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://dk.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sw.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://us.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ai.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ad.hnjuh.cn

Java: // 手写递归
来源：http://cw.nicolike.cn

Go:   // 手写递归
来源：http://vu.hahajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jl.shxzskj.cn

C#:   // 手写递归
来源：http://js.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ou.nicolike.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hr.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pp.szsharing.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pv.haigaiapp.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mu.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oj.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kx.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ut.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fw.bookmarksfly.cn

================================================================================
来源：http://bl.panjiajie.cn

O. 并发与异步
来源：http://ug.gzmigu.cn

================================================================================
来源：http://kc.9csxet.cn

[O01] 启动一个线程
来源：http://iy.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yp.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tq.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vk.lnxyls.cn

TS:   // 同 JS
来源：http://gw.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://lv.huixiangedu.cn

Go:   go f()
来源：http://ut.szxytkj.cn

Ruby: Thread.new { f }
来源：http://bj.nicolike.cn

C#:   Task.Run(() => F());
来源：http://zs.asd995.cn

[O02] 使用线程池
来源：http://an.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://me.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bo.hahajie.cn

JS:   // worker_threads 线程池
来源：http://ob.nszjky.cn

TS:   // worker_threads 线程池
来源：http://qz.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tk.shxzskj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xt.yuexingan06.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cr.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ej.huixiangedu.cn

[O03] 加锁保护共享数据
来源：http://bg.jctech888.com.cn

Py:   with lock: shared += 1
来源：http://mv.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://rd.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wo.521024.cn

TS:   // 同 JS
来源：http://gv.gzmigu.cn

Java: synchronized (this) { shared++; }
来源：http://pz.muxihuayi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kk.asd995.cn


<!-- 参考信息 -->