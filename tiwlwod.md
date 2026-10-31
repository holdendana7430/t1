代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tq.yuexingan06.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gk.nicolike.cn

[K08] 二进制序列化（非 JSON）
来源：http://ez.wgjwhj.cn

Py:   pickle.dumps(obj)
来源：http://tg.wgjwhj.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ib.colortex.cn

JS:   v8.serialize(obj)        // Node
来源：http://mb.hnjuh.cn

TS:   v8.serialize(obj)        // Node
来源：http://np.jianghongdianzi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ao.yuexingan06.cn

Go:   encoding/gob
来源：http://st.panjiajie.cn

Ruby: Marshal.dump(obj)
来源：http://lv.newstarts.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wr.shxzskj.cn

================================================================================
来源：http://zl.szsharing.cn

L. 网络请求
来源：http://oo.lnxyls.cn

================================================================================
来源：http://wz.hahajie.cn

[L01] 发送 GET 请求
来源：http://jf.gzmigu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://se.newstarts.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kx.lnxyls.cn

JS:   await fetch(url)
来源：http://wd.chemitech.net.cn

TS:   await fetch(url)
来源：http://rf.bookmarksfly.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cj.wgjwhj.cn

Go:   resp, err := http.Get(url)
来源：http://pp.bookmarksfly.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ak.huixinmuqiang.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wm.hnjuh.cn

[L02] 发送 POST JSON
来源：http://nn.huixiangedu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://sb.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vx.asd995.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ds.huixinmuqiang.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qm.colortex.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sw.hahajie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rs.haigaiapp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://de.asd995.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nl.asd995.cn

[L03] 设置自定义请求头
来源：http://no.9csxet.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ve.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lt.gzmigu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pn.hahajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sb.jctech888.com.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lb.bjjhwx.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cm.lnxyls.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zm.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jw.panjiajie.cn

[L04] 设置超时
来源：http://xq.newstarts.cn

Py:   requests.get(url, timeout=5)
来源：http://hj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dg.shtwfgs.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mh.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mk.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://py.newstarts.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://eg.chemitech.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dn.wgjwhj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wr.jianghongdianzi.cn

[L05] 上传文件（multipart）
来源：http://mh.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hu.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ge.shtwfgs.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mx.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xq.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qe.nicolike.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://me.hahajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ef.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lk.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://sz.shxzukj.cn

Py:   resp.json()
来源：http://xf.huanxung.cn

PHP:  json_decode($body, true);
来源：http://jv.yuntaijiaju.cn

JS:   await resp.json()
来源：http://fn.chemitech.net.cn

TS:   await resp.json()
来源：http://md.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bw.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jd.panjiajie.cn

Ruby: JSON.parse(resp.body)
来源：http://wo.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://io.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://rg.shtwfgs.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tk.jianghongdianzi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://td.bookmarksfly.cn

JS:   resp.ok;  resp.status
来源：http://jn.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://nw.shtwfgs.cn

Java: resp.statusCode()
来源：http://gf.huanxung.cn

Go:   resp.StatusCode
来源：http://qc.chemitech.net.cn

Ruby: resp.code.to_i
来源：http://kt.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://if.shxzskj.cn

[L08] 并发请求多个地址
来源：http://nn.szxytkj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://is.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ru.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://df.hahajie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lo.szxytkj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zv.jianghongdianzi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cw.panjiajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vo.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lh.yuexingan06.cn

================================================================================
来源：http://xt.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://qe.muxihuayi.cn

================================================================================
来源：http://sg.yuexingan06.cn

[M01] 读取命令行参数
来源：http://eu.lnxyls.cn

Py:   sys.argv[1:]
来源：http://pw.9csxet.cn

PHP:  $argv;  $argc;
来源：http://ro.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ef.yuexingan06.cn

TS:   process.argv.slice(2)
来源：http://kq.521024.cn

Java: args 数组（main 方法参数）
来源：http://by.colortex.cn

Go:   os.Args[1:]
来源：http://dc.panjiajie.cn

Ruby: ARGV
来源：http://py.asd995.cn

C#:   args 数组（Main 方法参数）
来源：http://ab.nszjky.cn

[M02] 读取环境变量
来源：http://vu.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://oj.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nb.gzmigu.cn

JS:   process.env.HOME
来源：http://jm.muxihuayi.cn

TS:   process.env.HOME
来源：http://yl.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://zq.huanxung.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yg.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://fr.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ic.521024.cn

[M03] 执行外部命令
来源：http://qv.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qz.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cb.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://pq.jctech888.com.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xq.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eb.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xf.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mv.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://jv.jianghongdianzi.cn

[M04] 获取当前工作目录
来源：http://so.lnxyls.cn

Py:   os.getcwd()
来源：http://no.huixiangedu.cn

PHP:  getcwd();
来源：http://bl.szxytkj.cn

JS:   process.cwd()
来源：http://wc.yuexingan06.cn

TS:   process.cwd()
来源：http://bl.bjjhwx.cn

Java: Path.of("").toAbsolutePath()
来源：http://fa.lnxyls.cn

Go:   os.Getwd()
来源：http://xl.shtwfgs.cn

Ruby: Dir.pwd
来源：http://px.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kj.szxytkj.cn

[M05] 设置退出码
来源：http://dz.nszjky.cn

Py:   sys.exit(1)
来源：http://gv.wgjwhj.cn

PHP:  exit(1);
来源：http://ta.asd995.cn

JS:   process.exit(1)
来源：http://ih.9csxet.cn

TS:   process.exit(1)
来源：http://rx.gzmigu.cn

Java: System.exit(1)
来源：http://re.chemitech.net.cn

Go:   os.Exit(1)
来源：http://mv.chemitech.net.cn

Ruby: exit 1
来源：http://re.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://po.szxytkj.cn

[M06] 向标准错误输出
来源：http://mx.yuexingan06.cn

Py:   print("err", file=sys.stderr)
来源：http://ul.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jq.shxzskj.cn

JS:   console.error("err")
来源：http://pd.newstarts.cn

TS:   console.error("err")
来源：http://xh.521024.cn

Java: System.err.println("err")
来源：http://rn.jctech888.com.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://za.szsharing.cn

Ruby: warn "err"
来源：http://qn.newstarts.cn

C#:   Console.Error.WriteLine("err")
来源：http://ki.9csxet.cn

[M07] 判断是否为主入口
来源：http://kv.newstarts.cn

Py:   if __name__ == "__main__":
来源：http://jt.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://df.hnjuh.cn

JS:   require.main === module
来源：http://qy.shtwfgs.cn

TS:   require.main === module
来源：http://ou.colortex.cn

Java: public static void main(String[] args)
来源：http://kx.shxzukj.cn

Go:   func main()
来源：http://yz.9csxet.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jd.muxihuayi.cn

C#:   static void Main(string[] args)
来源：http://zc.muxihuayi.cn

[M08] 获取系统与运行时信息
来源：http://po.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://xb.asd995.cn

PHP:  PHP_OS;  phpversion();
来源：http://wu.yuexingan06.cn

JS:   process.platform;  process.version
来源：http://jh.gzmigu.cn

TS:   process.platform;  process.version
来源：http://rt.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qr.huanxung.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qe.hnjuh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lz.szsharing.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://er.jianghongdianzi.cn

================================================================================
来源：http://pi.shxzskj.cn

N. 数据结构与算法
来源：http://qk.chemitech.net.cn

================================================================================
来源：http://iu.colortex.cn

[N01] 二分查找（有序数组）
来源：http://gg.jctech888.com.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ei.asd995.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ix.bookmarksfly.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ms.lnxyls.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://db.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://se.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://ez.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sh.haigaiapp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ye.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://bu.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ao.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fn.jctech888.com.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kd.bookmarksfly.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zy.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kh.nicolike.cn

Go:   slices.Sort(arr)
来源：http://wz.521024.cn

Ruby: arr.sort
来源：http://iu.bjjhwx.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://by.gzmigu.cn

[N03] 快速排序（分治示例）
来源：http://fw.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bf.wgjwhj.cn

PHP:  // 递归实现，或用 usort
来源：http://wt.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xd.huixinmuqiang.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mm.lnxyls.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wu.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cr.yuntaijiaju.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uf.huixinmuqiang.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zx.muxihuayi.cn

[N04] 斐波那契数列
来源：http://dq.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yl.szxytkj.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vo.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dd.huixiangedu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uq.szxytkj.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fk.jctech888.com.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ca.panjiajie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ml.chemitech.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oq.bookmarksfly.cn

[N05] 最大公约数
来源：http://xc.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://iu.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://or.521024.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ik.chemitech.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eq.wgjwhj.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sg.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tv.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://sj.nicolike.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tx.szxytkj.cn

[N06] 判断回文字符串
来源：http://tl.shxzskj.cn

Py:   s == s[::-1]
来源：http://jk.huixinmuqiang.cn

PHP:  $s === strrev($s);
来源：http://oi.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://fg.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://rs.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bh.szsharing.cn

Go:   // 双指针从两端比较
来源：http://ws.nicolike.cn

Ruby: s == s.reverse
来源：http://xm.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ut.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://bf.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bg.szsharing.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qj.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://og.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://ra.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://us.jianghongdianzi.cn

Go:   // 手写 map[int]int
来源：http://ih.huanxung.cn

Ruby: // 手写 Hash
来源：http://ga.lnxyls.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pb.hahajie.cn

[N08] 生成全排列
来源：http://hc.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://lt.hahajie.cn

PHP:  // 手写递归交换
来源：http://ts.huixiangedu.cn

JS:   // 手写回溯递归
来源：http://tv.9csxet.cn

TS:   // 手写回溯递归
来源：http://kb.huanxung.cn

Java: // 手写回溯递归
来源：http://xu.521024.cn

Go:   // 手写回溯递归
来源：http://tz.hnjuh.cn

Ruby: arr.permutation.to_a
来源：http://jr.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://wi.nicolike.cn

[N09] 栈与队列
来源：http://jc.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lw.muxihuayi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ci.521024.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zg.bookmarksfly.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yj.yuntaijiaju.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bx.gzmigu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hd.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jk.newstarts.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ch.shxzskj.cn

[N10] 链表节点定义
来源：http://ez.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yy.huixinmuqiang.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://of.shtwfgs.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cx.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sn.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://jk.muxihuayi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://xs.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mr.bjjhwx.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jw.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://bk.yuntaijiaju.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wy.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://ik.shtwfgs.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cx.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sg.521024.cn

Java: // 手写递归
来源：http://iz.gzmigu.cn

Go:   // 手写递归
来源：http://uv.newstarts.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://uz.bjjhwx.cn

C#:   // 手写递归
来源：http://eh.hnjuh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uw.yuexingan06.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xz.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dk.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pg.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zn.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nu.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ur.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jl.asd995.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bb.shxzukj.cn

================================================================================
来源：http://tx.jianghongdianzi.cn

O. 并发与异步
来源：http://tt.yuexingan06.cn

================================================================================
来源：http://lm.521024.cn

[O01] 启动一个线程
来源：http://qh.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ls.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yl.lnxyls.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gu.huixinmuqiang.cn

TS:   // 同 JS
来源：http://vm.521024.cn

Java: new Thread(() -> f()).start()
来源：http://uh.haigaiapp.cn

Go:   go f()
来源：http://je.szsharing.cn

Ruby: Thread.new { f }
来源：http://nl.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://sf.nszjky.cn

[O02] 使用线程池
来源：http://tz.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ju.shxzukj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wu.gzmigu.cn

JS:   // worker_threads 线程池
来源：http://cr.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://sf.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://he.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uj.huanxung.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sd.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ap.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://yi.gzmigu.cn

Py:   with lock: shared += 1
来源：http://er.jctech888.com.cn

PHP:  // 用 flock() 做文件锁
来源：http://nk.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fa.huixiangedu.cn

TS:   // 同 JS
来源：http://nf.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://xj.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://in.asd995.cn


<!-- 参考信息 -->