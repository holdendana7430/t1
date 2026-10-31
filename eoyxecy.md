代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yy.jctech888.com.cn

JS:   await fetch(url)
来源：http://nl.nicolike.cn

TS:   await fetch(url)
来源：http://bg.huixinmuqiang.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://le.jctech888.com.cn

Go:   resp, err := http.Get(url)
来源：http://ba.newstarts.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ec.bjjhwx.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jj.panjiajie.cn

[L02] 发送 POST JSON
来源：http://hw.chemitech.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wv.521024.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wu.szxytkj.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://my.chemitech.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gu.yuexingan06.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bi.yuntaijiaju.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xv.panjiajie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://al.nszjky.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gq.szsharing.cn

[L03] 设置自定义请求头
来源：http://zn.colortex.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ly.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dq.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ym.huixiangedu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ga.521024.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dy.haigaiapp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qh.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fd.jctech888.com.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fq.nicolike.cn

[L04] 设置超时
来源：http://yz.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://mb.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ho.nszjky.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://go.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nn.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hh.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oj.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mk.jctech888.com.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gn.shtwfgs.cn

[L05] 上传文件（multipart）
来源：http://ex.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hm.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dz.muxihuayi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gk.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sb.huixiangedu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bo.bookmarksfly.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tl.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eu.szxytkj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://af.hahajie.cn

[L06] 解析响应为 JSON
来源：http://oo.hnjuh.cn

Py:   resp.json()
来源：http://fu.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://ck.nicolike.cn

JS:   await resp.json()
来源：http://gf.newstarts.cn

TS:   await resp.json()
来源：http://ac.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://os.chemitech.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pb.hahajie.cn

Ruby: JSON.parse(resp.body)
来源：http://no.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xy.huixiangedu.cn

[L07] 处理 HTTP 状态码
来源：http://os.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hc.colortex.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ek.colortex.cn

JS:   resp.ok;  resp.status
来源：http://qc.shxzukj.cn

TS:   resp.ok;  resp.status
来源：http://et.muxihuayi.cn

Java: resp.statusCode()
来源：http://ff.chemitech.net.cn

Go:   resp.StatusCode
来源：http://br.szxytkj.cn

Ruby: resp.code.to_i
来源：http://vf.jianghongdianzi.cn

C#:   (int)resp.StatusCode
来源：http://il.shxzskj.cn

[L08] 并发请求多个地址
来源：http://rr.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fe.9csxet.cn

PHP:  curl_multi_init() 系列
来源：http://mp.9csxet.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nu.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jl.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ov.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aj.yuntaijiaju.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hu.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mo.bjjhwx.cn

================================================================================
来源：http://wg.shxzukj.cn

M. 命令行 / 进程 / 环境
来源：http://pb.szxytkj.cn

================================================================================
来源：http://zt.9csxet.cn

[M01] 读取命令行参数
来源：http://os.nszjky.cn

Py:   sys.argv[1:]
来源：http://lo.huanxung.cn

PHP:  $argv;  $argc;
来源：http://mk.gzmigu.cn

JS:   process.argv.slice(2)
来源：http://kv.shtwfgs.cn

TS:   process.argv.slice(2)
来源：http://bt.colortex.cn

Java: args 数组（main 方法参数）
来源：http://qy.hnjuh.cn

Go:   os.Args[1:]
来源：http://cw.shxzukj.cn

Ruby: ARGV
来源：http://pi.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://gr.muxihuayi.cn

[M02] 读取环境变量
来源：http://fr.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://vs.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dt.hnjuh.cn

JS:   process.env.HOME
来源：http://rn.bookmarksfly.cn

TS:   process.env.HOME
来源：http://be.yuntaijiaju.cn

Java: System.getenv("HOME")
来源：http://tg.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vw.hahajie.cn

Ruby: ENV["HOME"]
来源：http://sv.nicolike.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dx.szsharing.cn

[M03] 执行外部命令
来源：http://au.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zl.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ff.bookmarksfly.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://rr.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wr.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wr.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kx.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://yj.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://uh.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://ze.jctech888.com.cn

Py:   os.getcwd()
来源：http://tb.jianghongdianzi.cn

PHP:  getcwd();
来源：http://xz.521024.cn

JS:   process.cwd()
来源：http://gu.huixiangedu.cn

TS:   process.cwd()
来源：http://tj.yuexingan06.cn

Java: Path.of("").toAbsolutePath()
来源：http://ri.haigaiapp.cn

Go:   os.Getwd()
来源：http://lq.jctech888.com.cn

Ruby: Dir.pwd
来源：http://qz.newstarts.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wd.newstarts.cn

[M05] 设置退出码
来源：http://fx.yuexingan06.cn

Py:   sys.exit(1)
来源：http://lg.huixinmuqiang.cn

PHP:  exit(1);
来源：http://re.huixiangedu.cn

JS:   process.exit(1)
来源：http://vc.bookmarksfly.cn

TS:   process.exit(1)
来源：http://im.bookmarksfly.cn

Java: System.exit(1)
来源：http://zi.shtwfgs.cn

Go:   os.Exit(1)
来源：http://qu.jianghongdianzi.cn

Ruby: exit 1
来源：http://ue.nszjky.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mi.huanxung.cn

[M06] 向标准错误输出
来源：http://kf.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://qs.panjiajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ef.newstarts.cn

JS:   console.error("err")
来源：http://kv.jctech888.com.cn

TS:   console.error("err")
来源：http://ow.haigaiapp.cn

Java: System.err.println("err")
来源：http://qi.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vx.nicolike.cn

Ruby: warn "err"
来源：http://zb.9csxet.cn

C#:   Console.Error.WriteLine("err")
来源：http://nw.nicolike.cn

[M07] 判断是否为主入口
来源：http://vv.wgjwhj.cn

Py:   if __name__ == "__main__":
来源：http://gm.haigaiapp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fo.9csxet.cn

JS:   require.main === module
来源：http://ta.jctech888.com.cn

TS:   require.main === module
来源：http://nb.jianghongdianzi.cn

Java: public static void main(String[] args)
来源：http://vh.colortex.cn

Go:   func main()
来源：http://vk.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gm.nicolike.cn

C#:   static void Main(string[] args)
来源：http://ux.shxzukj.cn

[M08] 获取系统与运行时信息
来源：http://er.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://va.shtwfgs.cn

PHP:  PHP_OS;  phpversion();
来源：http://ah.hnjuh.cn

JS:   process.platform;  process.version
来源：http://xs.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://tj.panjiajie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://in.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ju.gzmigu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://na.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iq.yuexingan06.cn

================================================================================
来源：http://ci.asd995.cn

N. 数据结构与算法
来源：http://gc.huanxung.cn

================================================================================
来源：http://jo.bookmarksfly.cn

[N01] 二分查找（有序数组）
来源：http://ll.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cc.shxzskj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ec.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qf.wgjwhj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jz.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mp.bookmarksfly.cn

Go:   sort.SearchInts(arr, x)
来源：http://go.lnxyls.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qy.colortex.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dd.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://eo.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vs.colortex.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xd.hnjuh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gr.yuntaijiaju.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dp.shxzskj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lh.shtwfgs.cn

Go:   slices.Sort(arr)
来源：http://kf.yuntaijiaju.cn

Ruby: arr.sort
来源：http://mv.9csxet.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rs.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://rl.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nx.huanxung.cn

PHP:  // 递归实现，或用 usort
来源：http://qh.szsharing.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tb.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://da.huixiangedu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zc.colortex.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pm.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jw.asd995.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fr.szxytkj.cn

[N04] 斐波那契数列
来源：http://bl.yuexingan06.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ew.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nl.shxzukj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ft.bookmarksfly.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jw.bjjhwx.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vk.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fz.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jv.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zd.hnjuh.cn

[N05] 最大公约数
来源：http://at.jctech888.com.cn

Py:   math.gcd(a, b)
来源：http://qg.huixinmuqiang.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ff.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dx.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jq.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jp.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://of.muxihuayi.cn

Ruby: a.gcd(b)
来源：http://qi.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ur.yuntaijiaju.cn

[N06] 判断回文字符串
来源：http://iw.chemitech.net.cn

Py:   s == s[::-1]
来源：http://sd.szxytkj.cn

PHP:  $s === strrev($s);
来源：http://sw.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://xk.chemitech.net.cn

TS:   s === [...s].reverse().join("")
来源：http://bf.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fb.szxytkj.cn

Go:   // 双指针从两端比较
来源：http://gh.yuexingan06.cn

Ruby: s == s.reverse
来源：http://hp.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yj.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://sn.lnxyls.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bi.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hf.shxzskj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pw.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://ok.hnjuh.cn

Java: // 手写 HashMap
来源：http://dc.szsharing.cn

Go:   // 手写 map[int]int
来源：http://ri.huanxung.cn

Ruby: // 手写 Hash
来源：http://dn.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cy.jctech888.com.cn

[N08] 生成全排列
来源：http://pi.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://fb.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://id.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://zm.newstarts.cn

TS:   // 手写回溯递归
来源：http://jd.newstarts.cn

Java: // 手写回溯递归
来源：http://bb.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://ct.szsharing.cn

Ruby: arr.permutation.to_a
来源：http://kg.hahajie.cn

C#:   // 手写回溯递归
来源：http://sg.huixiangedu.cn

[N09] 栈与队列
来源：http://br.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ba.szsharing.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eb.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xz.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bb.muxihuayi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oj.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fr.chemitech.net.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ur.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zp.bjjhwx.cn

[N10] 链表节点定义
来源：http://cj.9csxet.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nv.muxihuayi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://sr.haigaiapp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://al.chemitech.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://es.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://od.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kk.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wv.hahajie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ol.yuexingan06.cn

[N11] 二叉树中序遍历
来源：http://fz.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ha.szsharing.cn

PHP:  // 手写递归函数
来源：http://xx.nszjky.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yi.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nc.chemitech.net.cn

Java: // 手写递归
来源：http://gs.muxihuayi.cn

Go:   // 手写递归
来源：http://lc.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://en.panjiajie.cn

C#:   // 手写递归
来源：http://ap.nszjky.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iv.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dw.huanxung.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jb.jctech888.com.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ts.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ud.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bv.szxytkj.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yf.lnxyls.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://va.yuntaijiaju.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yk.521024.cn

================================================================================
来源：http://wp.hnjuh.cn

O. 并发与异步
来源：http://tm.szxytkj.cn

================================================================================
来源：http://ns.shtwfgs.cn

[O01] 启动一个线程
来源：http://hz.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sq.asd995.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gx.huixinmuqiang.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ir.gzmigu.cn

TS:   // 同 JS
来源：http://qj.lnxyls.cn

Java: new Thread(() -> f()).start()
来源：http://lj.huanxung.cn

Go:   go f()
来源：http://sa.gzmigu.cn

Ruby: Thread.new { f }
来源：http://bv.gzmigu.cn

C#:   Task.Run(() => F());
来源：http://zj.hahajie.cn

[O02] 使用线程池
来源：http://db.shtwfgs.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jg.szsharing.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ra.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://ec.muxihuayi.cn

TS:   // worker_threads 线程池
来源：http://cc.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bq.shtwfgs.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iy.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sr.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ov.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://nh.newstarts.cn

Py:   with lock: shared += 1
来源：http://kd.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://ve.jianghongdianzi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zv.jianghongdianzi.cn

TS:   // 同 JS
来源：http://ul.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://wx.newstarts.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qi.521024.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xk.huixiangedu.cn

C#:   lock (gate) { shared++; }
来源：http://mf.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://ij.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://sm.jctech888.com.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fp.nicolike.cn

JS:   async function f() { await g(); }
来源：http://zy.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qq.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mb.bjjhwx.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eb.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tf.szxytkj.cn

C#:   async Task F() { await G(); }
来源：http://sw.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://sh.yuexingan06.cn

Py:   asyncio.gather(*tasks)
来源：http://br.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fz.bookmarksfly.cn

JS:   await Promise.all(tasks)
来源：http://yt.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://ez.nszjky.cn


<!-- 参考信息 -->