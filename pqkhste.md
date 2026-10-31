代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tz.shxzukj.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cm.shtwfgs.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nl.lnxyls.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ym.shxzukj.cn

[L03] 设置自定义请求头
来源：http://df.newstarts.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zd.panjiajie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sy.9csxet.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://af.panjiajie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kg.gzmigu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ql.jianghongdianzi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ay.szsharing.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nn.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://af.chemitech.net.cn

[L04] 设置超时
来源：http://th.bjjhwx.cn

Py:   requests.get(url, timeout=5)
来源：http://qv.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sc.colortex.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://av.huixiangedu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wi.jctech888.com.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ai.nicolike.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cm.521024.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kw.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://he.szsharing.cn

[L05] 上传文件（multipart）
来源：http://ut.9csxet.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jx.szxytkj.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yr.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uh.jctech888.com.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ep.hnjuh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zi.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pr.huixinmuqiang.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yq.wgjwhj.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qe.shtwfgs.cn

[L06] 解析响应为 JSON
来源：http://nr.asd995.cn

Py:   resp.json()
来源：http://jv.muxihuayi.cn

PHP:  json_decode($body, true);
来源：http://si.shtwfgs.cn

JS:   await resp.json()
来源：http://ar.shxzskj.cn

TS:   await resp.json()
来源：http://co.nicolike.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mk.szxytkj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tv.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://ur.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ik.nicolike.cn

[L07] 处理 HTTP 状态码
来源：http://iz.chemitech.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mg.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pg.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://bk.shxzskj.cn

TS:   resp.ok;  resp.status
来源：http://uf.shxzukj.cn

Java: resp.statusCode()
来源：http://if.huixinmuqiang.cn

Go:   resp.StatusCode
来源：http://ev.newstarts.cn

Ruby: resp.code.to_i
来源：http://bf.muxihuayi.cn

C#:   (int)resp.StatusCode
来源：http://ht.muxihuayi.cn

[L08] 并发请求多个地址
来源：http://um.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ee.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://vq.haigaiapp.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fi.jctech888.com.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rs.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gs.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oy.521024.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.hnjuh.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tf.huixinmuqiang.cn

================================================================================
来源：http://eo.haigaiapp.cn

M. 命令行 / 进程 / 环境
来源：http://iv.huixiangedu.cn

================================================================================
来源：http://rc.jianghongdianzi.cn

[M01] 读取命令行参数
来源：http://nl.shxzukj.cn

Py:   sys.argv[1:]
来源：http://ix.asd995.cn

PHP:  $argv;  $argc;
来源：http://rl.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://iw.nszjky.cn

TS:   process.argv.slice(2)
来源：http://li.9csxet.cn

Java: args 数组（main 方法参数）
来源：http://qi.muxihuayi.cn

Go:   os.Args[1:]
来源：http://yj.shxzukj.cn

Ruby: ARGV
来源：http://pm.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://ho.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://cc.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://io.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cd.asd995.cn

JS:   process.env.HOME
来源：http://ju.yuntaijiaju.cn

TS:   process.env.HOME
来源：http://co.jctech888.com.cn

Java: System.getenv("HOME")
来源：http://zw.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rn.hnjuh.cn

Ruby: ENV["HOME"]
来源：http://jd.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wg.colortex.cn

[M03] 执行外部命令
来源：http://jn.muxihuayi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bu.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wl.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uv.huanxung.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hj.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ke.panjiajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tt.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://hn.bookmarksfly.cn

C#:   Process.Start("ls", "-l");
来源：http://nr.hnjuh.cn

[M04] 获取当前工作目录
来源：http://wp.wgjwhj.cn

Py:   os.getcwd()
来源：http://hh.shxzskj.cn

PHP:  getcwd();
来源：http://vb.haigaiapp.cn

JS:   process.cwd()
来源：http://xl.yuntaijiaju.cn

TS:   process.cwd()
来源：http://px.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://ks.szsharing.cn

Go:   os.Getwd()
来源：http://fa.bjjhwx.cn

Ruby: Dir.pwd
来源：http://hj.jctech888.com.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oh.muxihuayi.cn

[M05] 设置退出码
来源：http://yd.9csxet.cn

Py:   sys.exit(1)
来源：http://gp.hnjuh.cn

PHP:  exit(1);
来源：http://kh.gzmigu.cn

JS:   process.exit(1)
来源：http://la.nszjky.cn

TS:   process.exit(1)
来源：http://pz.shxzskj.cn

Java: System.exit(1)
来源：http://bc.hahajie.cn

Go:   os.Exit(1)
来源：http://xc.yuexingan06.cn

Ruby: exit 1
来源：http://qa.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.yuntaijiaju.cn

[M06] 向标准错误输出
来源：http://lw.yuntaijiaju.cn

Py:   print("err", file=sys.stderr)
来源：http://ib.bookmarksfly.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://su.shtwfgs.cn

JS:   console.error("err")
来源：http://va.huanxung.cn

TS:   console.error("err")
来源：http://pi.panjiajie.cn

Java: System.err.println("err")
来源：http://kp.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://or.nicolike.cn

Ruby: warn "err"
来源：http://fb.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://zx.newstarts.cn

[M07] 判断是否为主入口
来源：http://oy.521024.cn

Py:   if __name__ == "__main__":
来源：http://hm.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fq.nicolike.cn

JS:   require.main === module
来源：http://eb.yuexingan06.cn

TS:   require.main === module
来源：http://pg.muxihuayi.cn

Java: public static void main(String[] args)
来源：http://ra.nicolike.cn

Go:   func main()
来源：http://wg.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xp.asd995.cn

C#:   static void Main(string[] args)
来源：http://tc.yuntaijiaju.cn

[M08] 获取系统与运行时信息
来源：http://ws.newstarts.cn

Py:   platform.system();  platform.python_version()
来源：http://hh.bookmarksfly.cn

PHP:  PHP_OS;  phpversion();
来源：http://co.hnjuh.cn

JS:   process.platform;  process.version
来源：http://bg.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://qw.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cp.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sm.hahajie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ek.jctech888.com.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gn.panjiajie.cn

================================================================================
来源：http://vg.colortex.cn

N. 数据结构与算法
来源：http://gk.nicolike.cn

================================================================================
来源：http://wk.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://xu.szxytkj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sw.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mb.haigaiapp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://au.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zx.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://is.huixinmuqiang.cn

Go:   sort.SearchInts(arr, x)
来源：http://eh.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://aw.huixiangedu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ib.shtwfgs.cn

[N02] 排序（工程实践用内置实现）
来源：http://mo.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://ia.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vu.shxzukj.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gs.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://re.bjjhwx.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yv.huanxung.cn

Go:   slices.Sort(arr)
来源：http://fu.gzmigu.cn

Ruby: arr.sort
来源：http://wx.shxzskj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ib.asd995.cn

[N03] 快速排序（分治示例）
来源：http://gb.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bh.shxzukj.cn

PHP:  // 递归实现，或用 usort
来源：http://xg.hnjuh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hg.hnjuh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hw.yuntaijiaju.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jn.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xm.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wo.hnjuh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ie.huixinmuqiang.cn

[N04] 斐波那契数列
来源：http://dw.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jf.yuntaijiaju.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ot.muxihuayi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zk.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nw.chemitech.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yf.nszjky.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yt.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iw.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qv.colortex.cn

[N05] 最大公约数
来源：http://xs.lnxyls.cn

Py:   math.gcd(a, b)
来源：http://oj.jctech888.com.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rf.jianghongdianzi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rt.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ya.hnjuh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kn.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fi.hahajie.cn

Ruby: a.gcd(b)
来源：http://vg.colortex.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hj.wgjwhj.cn

[N06] 判断回文字符串
来源：http://cu.huixiangedu.cn

Py:   s == s[::-1]
来源：http://jw.shtwfgs.cn

PHP:  $s === strrev($s);
来源：http://og.yuntaijiaju.cn

JS:   s === [...s].reverse().join("")
来源：http://ag.shxzskj.cn

TS:   s === [...s].reverse().join("")
来源：http://et.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ld.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://oi.shxzskj.cn

Ruby: s == s.reverse
来源：http://oq.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ab.jianghongdianzi.cn

[N07] 两数之和（返回下标）
来源：http://ww.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vc.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yq.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rn.shxzskj.cn

TS:   // 手写 Map<string, number>
来源：http://ru.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://dw.hahajie.cn

Go:   // 手写 map[int]int
来源：http://af.yuntaijiaju.cn

Ruby: // 手写 Hash
来源：http://kt.szsharing.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jb.wgjwhj.cn

[N08] 生成全排列
来源：http://op.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://jt.shxzskj.cn

PHP:  // 手写递归交换
来源：http://wk.shxzskj.cn

JS:   // 手写回溯递归
来源：http://wd.gzmigu.cn

TS:   // 手写回溯递归
来源：http://td.chemitech.net.cn

Java: // 手写回溯递归
来源：http://tx.panjiajie.cn

Go:   // 手写回溯递归
来源：http://xc.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://zd.shxzskj.cn

C#:   // 手写回溯递归
来源：http://ow.szxytkj.cn

[N09] 栈与队列
来源：http://oi.shxzskj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ww.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://js.newstarts.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vy.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oi.huanxung.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pa.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://co.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wf.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://np.muxihuayi.cn

[N10] 链表节点定义
来源：http://mm.huixiangedu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ij.yuexingan06.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tu.colortex.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yg.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jw.wgjwhj.cn

Java: class Node { int v; Node next; }
来源：http://ed.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tz.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xm.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ta.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://lc.9csxet.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ng.huanxung.cn

PHP:  // 手写递归函数
来源：http://pq.huanxung.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uy.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fn.shxzukj.cn

Java: // 手写递归
来源：http://oa.huanxung.cn

Go:   // 手写递归
来源：http://jc.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nj.shxzskj.cn

C#:   // 手写递归
来源：http://ku.yuntaijiaju.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tg.huanxung.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ot.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://an.muxihuayi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kc.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gk.yuntaijiaju.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kd.huixiangedu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yt.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zp.colortex.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rb.huixiangedu.cn

================================================================================
来源：http://ac.hahajie.cn

O. 并发与异步
来源：http://ca.jctech888.com.cn

================================================================================
来源：http://xa.wgjwhj.cn

[O01] 启动一个线程
来源：http://bz.panjiajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ua.shxzskj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ej.9csxet.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nc.9csxet.cn

TS:   // 同 JS
来源：http://zx.nicolike.cn

Java: new Thread(() -> f()).start()
来源：http://oq.szsharing.cn

Go:   go f()
来源：http://lf.haigaiapp.cn

Ruby: Thread.new { f }
来源：http://pg.yuntaijiaju.cn

C#:   Task.Run(() => F());
来源：http://mc.521024.cn

[O02] 使用线程池
来源：http://ls.panjiajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ic.hahajie.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gw.panjiajie.cn

JS:   // worker_threads 线程池
来源：http://nd.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://qv.yuntaijiaju.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fw.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ow.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ix.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rs.jctech888.com.cn

[O03] 加锁保护共享数据
来源：http://pm.gzmigu.cn

Py:   with lock: shared += 1
来源：http://qq.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://nl.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mk.jctech888.com.cn

TS:   // 同 JS
来源：http://wo.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://iv.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fn.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xq.yuexingan06.cn

C#:   lock (gate) { shared++; }
来源：http://lo.huanxung.cn

[O04] 定义异步函数并等待
来源：http://ae.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ia.lnxyls.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ls.nicolike.cn

JS:   async function f() { await g(); }
来源：http://tp.colortex.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yf.gzmigu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ut.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sr.shxzskj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lf.haigaiapp.cn

C#:   async Task F() { await G(); }
来源：http://hw.yuntaijiaju.cn

[O05] 并发执行并等待全部完成
来源：http://cc.chemitech.net.cn

Py:   asyncio.gather(*tasks)
来源：http://bf.hahajie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mq.hahajie.cn

JS:   await Promise.all(tasks)
来源：http://bi.bookmarksfly.cn

TS:   await Promise.all(tasks)
来源：http://oe.muxihuayi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zi.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gl.huanxung.cn

Ruby: threads.map(&:join)
来源：http://hv.chemitech.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cw.wgjwhj.cn

[O06] 使用进程池
来源：http://sb.huanxung.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nh.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sl.bookmarksfly.cn

JS:   // child_process / cluster 模块
来源：http://vy.gzmigu.cn

TS:   // child_process / cluster 模块
来源：http://gd.yuntaijiaju.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sv.bjjhwx.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qh.shtwfgs.cn

Ruby: // fork 块
来源：http://id.jctech888.com.cn


<!-- 参考信息 -->