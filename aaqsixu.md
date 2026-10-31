代发 wailian999

Go:   encoding/gob
来源：http://cg.wgjwhj.cn

Ruby: Marshal.dump(obj)
来源：http://sx.muxihuayi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ux.9csxet.cn

================================================================================
来源：http://rs.bjjhwx.cn

L. 网络请求
来源：http://tj.jctech888.com.cn

================================================================================
来源：http://xd.muxihuayi.cn

[L01] 发送 GET 请求
来源：http://yy.yuntaijiaju.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ta.shxzskj.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ut.bjjhwx.cn

JS:   await fetch(url)
来源：http://hj.hnjuh.cn

TS:   await fetch(url)
来源：http://zi.szsharing.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jr.521024.cn

Go:   resp, err := http.Get(url)
来源：http://ox.muxihuayi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sj.jctech888.com.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lr.newstarts.cn

[L02] 发送 POST JSON
来源：http://dc.lnxyls.cn

Py:   requests.post(url, json={"a": 1})
来源：http://nj.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uk.gzmigu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vo.gzmigu.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hn.asd995.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ox.521024.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vc.jctech888.com.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zc.yuexingan06.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pl.gzmigu.cn

[L03] 设置自定义请求头
来源：http://ic.521024.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rc.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ha.yuexingan06.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pz.gzmigu.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dt.bjjhwx.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://iy.521024.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jb.colortex.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mo.huixiangedu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pt.hahajie.cn

[L04] 设置超时
来源：http://er.jianghongdianzi.cn

Py:   requests.get(url, timeout=5)
来源：http://ma.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yk.9csxet.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vu.huanxung.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gm.yuexingan06.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hl.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mx.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sh.jianghongdianzi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vo.bookmarksfly.cn

[L05] 上传文件（multipart）
来源：http://yu.nszjky.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vx.huixinmuqiang.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tz.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://se.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eb.colortex.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pl.panjiajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yj.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tj.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kb.szxytkj.cn

[L06] 解析响应为 JSON
来源：http://ot.szxytkj.cn

Py:   resp.json()
来源：http://aj.521024.cn

PHP:  json_decode($body, true);
来源：http://cg.nicolike.cn

JS:   await resp.json()
来源：http://gm.lnxyls.cn

TS:   await resp.json()
来源：http://pm.huixinmuqiang.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tt.yuexingan06.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tn.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://rp.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rd.gzmigu.cn

[L07] 处理 HTTP 状态码
来源：http://ry.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vg.shtwfgs.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uk.huixiangedu.cn

JS:   resp.ok;  resp.status
来源：http://nw.szxytkj.cn

TS:   resp.ok;  resp.status
来源：http://wx.haigaiapp.cn

Java: resp.statusCode()
来源：http://ii.nicolike.cn

Go:   resp.StatusCode
来源：http://wz.yuexingan06.cn

Ruby: resp.code.to_i
来源：http://iy.521024.cn

C#:   (int)resp.StatusCode
来源：http://gc.panjiajie.cn

[L08] 并发请求多个地址
来源：http://am.yuexingan06.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ax.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://ly.huanxung.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wc.hnjuh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cb.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iw.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://io.newstarts.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ni.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zi.hnjuh.cn

================================================================================
来源：http://ng.huixinmuqiang.cn

M. 命令行 / 进程 / 环境
来源：http://nt.huanxung.cn

================================================================================
来源：http://vy.nicolike.cn

[M01] 读取命令行参数
来源：http://fn.yuntaijiaju.cn

Py:   sys.argv[1:]
来源：http://ei.huixinmuqiang.cn

PHP:  $argv;  $argc;
来源：http://ts.szsharing.cn

JS:   process.argv.slice(2)
来源：http://cf.nszjky.cn

TS:   process.argv.slice(2)
来源：http://hq.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://da.wgjwhj.cn

Go:   os.Args[1:]
来源：http://vt.hahajie.cn

Ruby: ARGV
来源：http://dt.shtwfgs.cn

C#:   args 数组（Main 方法参数）
来源：http://hi.asd995.cn

[M02] 读取环境变量
来源：http://hv.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://xt.newstarts.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rw.szsharing.cn

JS:   process.env.HOME
来源：http://dk.newstarts.cn

TS:   process.env.HOME
来源：http://vl.szsharing.cn

Java: System.getenv("HOME")
来源：http://ir.bookmarksfly.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ev.bookmarksfly.cn

Ruby: ENV["HOME"]
来源：http://sa.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tg.nicolike.cn

[M03] 执行外部命令
来源：http://rw.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xe.yuntaijiaju.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oy.panjiajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qe.yuexingan06.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gu.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gh.newstarts.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ia.asd995.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cy.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://co.lnxyls.cn

[M04] 获取当前工作目录
来源：http://cc.newstarts.cn

Py:   os.getcwd()
来源：http://fe.shxzskj.cn

PHP:  getcwd();
来源：http://in.shxzukj.cn

JS:   process.cwd()
来源：http://va.yuntaijiaju.cn

TS:   process.cwd()
来源：http://fz.bookmarksfly.cn

Java: Path.of("").toAbsolutePath()
来源：http://vv.yuexingan06.cn

Go:   os.Getwd()
来源：http://eq.jctech888.com.cn

Ruby: Dir.pwd
来源：http://zc.wgjwhj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nj.jctech888.com.cn

[M05] 设置退出码
来源：http://hc.shxzukj.cn

Py:   sys.exit(1)
来源：http://cz.shtwfgs.cn

PHP:  exit(1);
来源：http://na.hahajie.cn

JS:   process.exit(1)
来源：http://tg.lnxyls.cn

TS:   process.exit(1)
来源：http://nv.nicolike.cn

Java: System.exit(1)
来源：http://tw.gzmigu.cn

Go:   os.Exit(1)
来源：http://sb.9csxet.cn

Ruby: exit 1
来源：http://mn.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://li.9csxet.cn

[M06] 向标准错误输出
来源：http://hw.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://bh.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qa.nszjky.cn

JS:   console.error("err")
来源：http://kt.colortex.cn

TS:   console.error("err")
来源：http://ex.hnjuh.cn

Java: System.err.println("err")
来源：http://ov.bjjhwx.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vq.jctech888.com.cn

Ruby: warn "err"
来源：http://xw.bjjhwx.cn

C#:   Console.Error.WriteLine("err")
来源：http://qy.lnxyls.cn

[M07] 判断是否为主入口
来源：http://mb.hahajie.cn

Py:   if __name__ == "__main__":
来源：http://xp.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ck.yuntaijiaju.cn

JS:   require.main === module
来源：http://bd.jianghongdianzi.cn

TS:   require.main === module
来源：http://uk.szxytkj.cn

Java: public static void main(String[] args)
来源：http://lk.yuntaijiaju.cn

Go:   func main()
来源：http://fq.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rm.huixinmuqiang.cn

C#:   static void Main(string[] args)
来源：http://xu.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://fj.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://dy.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://dx.shtwfgs.cn

JS:   process.platform;  process.version
来源：http://px.yuntaijiaju.cn

TS:   process.platform;  process.version
来源：http://al.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qd.asd995.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jt.9csxet.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yi.hnjuh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bd.szsharing.cn

================================================================================
来源：http://yi.panjiajie.cn

N. 数据结构与算法
来源：http://yt.bookmarksfly.cn

================================================================================
来源：http://ov.chemitech.net.cn

[N01] 二分查找（有序数组）
来源：http://ml.haigaiapp.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bj.muxihuayi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ta.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cp.chemitech.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sp.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://te.haigaiapp.cn

Go:   sort.SearchInts(arr, x)
来源：http://aw.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qs.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vk.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://rn.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://pg.huanxung.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gt.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dz.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yx.chemitech.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zf.9csxet.cn

Go:   slices.Sort(arr)
来源：http://bj.yuntaijiaju.cn

Ruby: arr.sort
来源：http://fy.shtwfgs.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fc.huixinmuqiang.cn

[N03] 快速排序（分治示例）
来源：http://rq.gzmigu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nt.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://fz.wgjwhj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xx.huixiangedu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tk.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://us.haigaiapp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ki.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uy.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bz.nicolike.cn

[N04] 斐波那契数列
来源：http://ch.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kp.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nw.szxytkj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fo.szsharing.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ax.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kx.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ss.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rn.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bp.hnjuh.cn

[N05] 最大公约数
来源：http://ho.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://gl.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iz.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zk.jianghongdianzi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://we.szsharing.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ml.haigaiapp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sw.colortex.cn

Ruby: a.gcd(b)
来源：http://sz.muxihuayi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tf.shtwfgs.cn

[N06] 判断回文字符串
来源：http://vi.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://cy.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://va.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://nr.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://hj.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fp.newstarts.cn

Go:   // 双指针从两端比较
来源：http://is.hnjuh.cn

Ruby: s == s.reverse
来源：http://fk.yuexingan06.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ts.521024.cn

[N07] 两数之和（返回下标）
来源：http://wi.bjjhwx.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hy.panjiajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nu.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ma.bjjhwx.cn

TS:   // 手写 Map<string, number>
来源：http://rn.shxzukj.cn

Java: // 手写 HashMap
来源：http://wd.newstarts.cn

Go:   // 手写 map[int]int
来源：http://ws.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://fd.shtwfgs.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yg.jctech888.com.cn

[N08] 生成全排列
来源：http://gx.yuntaijiaju.cn

Py:   itertools.permutations(arr)
来源：http://ah.yuexingan06.cn

PHP:  // 手写递归交换
来源：http://jh.lnxyls.cn

JS:   // 手写回溯递归
来源：http://vk.panjiajie.cn

TS:   // 手写回溯递归
来源：http://zx.yuntaijiaju.cn

Java: // 手写回溯递归
来源：http://ih.szsharing.cn

Go:   // 手写回溯递归
来源：http://zv.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://lg.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://df.newstarts.cn

[N09] 栈与队列
来源：http://mv.nszjky.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xn.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cu.wgjwhj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vb.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zt.gzmigu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qr.yuntaijiaju.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vp.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uf.gzmigu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ly.wgjwhj.cn

[N10] 链表节点定义
来源：http://br.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cm.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xx.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lp.yuexingan06.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://za.asd995.cn

Java: class Node { int v; Node next; }
来源：http://xx.huanxung.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ut.muxihuayi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pq.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wu.521024.cn

[N11] 二叉树中序遍历
来源：http://uj.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yv.panjiajie.cn

PHP:  // 手写递归函数
来源：http://nl.asd995.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lv.yuntaijiaju.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wa.muxihuayi.cn

Java: // 手写递归
来源：http://lv.chemitech.net.cn

Go:   // 手写递归
来源：http://if.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oj.bjjhwx.cn

C#:   // 手写递归
来源：http://bu.wgjwhj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mn.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://js.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eb.shxzskj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jt.bookmarksfly.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zw.lnxyls.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ue.muxihuayi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rp.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ay.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ik.shxzskj.cn

================================================================================
来源：http://gb.muxihuayi.cn

O. 并发与异步
来源：http://er.haigaiapp.cn

================================================================================
来源：http://ju.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://on.nszjky.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tv.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dp.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qs.lnxyls.cn

TS:   // 同 JS
来源：http://cd.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://rq.huixinmuqiang.cn

Go:   go f()
来源：http://ii.9csxet.cn

Ruby: Thread.new { f }
来源：http://jy.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://jk.hahajie.cn

[O02] 使用线程池
来源：http://da.9csxet.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wc.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zg.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://fx.jianghongdianzi.cn

TS:   // worker_threads 线程池
来源：http://xc.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gb.huixinmuqiang.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fw.bookmarksfly.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pm.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hr.haigaiapp.cn

[O03] 加锁保护共享数据
来源：http://oa.huanxung.cn

Py:   with lock: shared += 1
来源：http://ym.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://gj.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://si.521024.cn

TS:   // 同 JS
来源：http://rx.chemitech.net.cn

Java: synchronized (this) { shared++; }
来源：http://wo.panjiajie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ji.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bz.szsharing.cn

C#:   lock (gate) { shared++; }
来源：http://oi.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://hw.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://mg.yuexingan06.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rd.haigaiapp.cn

JS:   async function f() { await g(); }
来源：http://rd.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dl.lnxyls.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yr.szsharing.cn


<!-- 参考信息 -->