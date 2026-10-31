代发 wailian999

[L03] 设置自定义请求头
来源：http://vd.muxihuayi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fm.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ec.yuntaijiaju.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hn.jctech888.com.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qs.huanxung.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xn.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vd.hahajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jf.shxzskj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zk.nszjky.cn

[L04] 设置超时
来源：http://sw.nicolike.cn

Py:   requests.get(url, timeout=5)
来源：http://au.szsharing.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://nr.newstarts.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jl.yuexingan06.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eq.huanxung.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hl.shxzukj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ws.nszjky.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pp.haigaiapp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ni.nicolike.cn

[L05] 上传文件（multipart）
来源：http://di.bjjhwx.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ek.bjjhwx.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rm.panjiajie.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://su.newstarts.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kc.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dn.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mb.panjiajie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cp.521024.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mk.colortex.cn

[L06] 解析响应为 JSON
来源：http://vt.colortex.cn

Py:   resp.json()
来源：http://fr.huixiangedu.cn

PHP:  json_decode($body, true);
来源：http://dv.hnjuh.cn

JS:   await resp.json()
来源：http://ep.nszjky.cn

TS:   await resp.json()
来源：http://wh.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sy.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rk.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://bc.jianghongdianzi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://iw.huanxung.cn

[L07] 处理 HTTP 状态码
来源：http://wy.newstarts.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fa.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wf.bjjhwx.cn

JS:   resp.ok;  resp.status
来源：http://hz.bookmarksfly.cn

TS:   resp.ok;  resp.status
来源：http://uq.jctech888.com.cn

Java: resp.statusCode()
来源：http://xs.gzmigu.cn

Go:   resp.StatusCode
来源：http://sq.haigaiapp.cn

Ruby: resp.code.to_i
来源：http://js.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://yz.bjjhwx.cn

[L08] 并发请求多个地址
来源：http://ja.hnjuh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://td.shxzskj.cn

PHP:  curl_multi_init() 系列
来源：http://gu.hahajie.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zr.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wh.newstarts.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ck.szsharing.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ma.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zs.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ud.szsharing.cn

================================================================================
来源：http://xq.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://nx.521024.cn

================================================================================
来源：http://vq.panjiajie.cn

[M01] 读取命令行参数
来源：http://ik.jianghongdianzi.cn

Py:   sys.argv[1:]
来源：http://lt.shxzukj.cn

PHP:  $argv;  $argc;
来源：http://vk.newstarts.cn

JS:   process.argv.slice(2)
来源：http://wh.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://mc.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://rj.shxzskj.cn

Go:   os.Args[1:]
来源：http://oe.9csxet.cn

Ruby: ARGV
来源：http://br.colortex.cn

C#:   args 数组（Main 方法参数）
来源：http://ov.nszjky.cn

[M02] 读取环境变量
来源：http://wx.hahajie.cn

Py:   os.environ.get("HOME")
来源：http://sj.szsharing.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ed.jctech888.com.cn

JS:   process.env.HOME
来源：http://oj.bjjhwx.cn

TS:   process.env.HOME
来源：http://vz.asd995.cn

Java: System.getenv("HOME")
来源：http://sw.gzmigu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sv.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://zp.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pv.hahajie.cn

[M03] 执行外部命令
来源：http://ah.hnjuh.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pv.gzmigu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hj.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ry.chemitech.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ro.bjjhwx.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qf.nicolike.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nw.wgjwhj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ql.hahajie.cn

C#:   Process.Start("ls", "-l");
来源：http://wd.asd995.cn

[M04] 获取当前工作目录
来源：http://yq.nszjky.cn

Py:   os.getcwd()
来源：http://fa.newstarts.cn

PHP:  getcwd();
来源：http://hz.bookmarksfly.cn

JS:   process.cwd()
来源：http://dg.shxzskj.cn

TS:   process.cwd()
来源：http://bs.hahajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://gc.gzmigu.cn

Go:   os.Getwd()
来源：http://qo.chemitech.net.cn

Ruby: Dir.pwd
来源：http://kb.szxytkj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gi.yuntaijiaju.cn

[M05] 设置退出码
来源：http://tt.wgjwhj.cn

Py:   sys.exit(1)
来源：http://jg.yuntaijiaju.cn

PHP:  exit(1);
来源：http://op.panjiajie.cn

JS:   process.exit(1)
来源：http://lv.yuntaijiaju.cn

TS:   process.exit(1)
来源：http://be.panjiajie.cn

Java: System.exit(1)
来源：http://iu.shxzskj.cn

Go:   os.Exit(1)
来源：http://jm.newstarts.cn

Ruby: exit 1
来源：http://ln.yuexingan06.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://th.gzmigu.cn

[M06] 向标准错误输出
来源：http://pb.hnjuh.cn

Py:   print("err", file=sys.stderr)
来源：http://wx.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gx.jctech888.com.cn

JS:   console.error("err")
来源：http://kv.yuexingan06.cn

TS:   console.error("err")
来源：http://iq.nicolike.cn

Java: System.err.println("err")
来源：http://qc.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qx.muxihuayi.cn

Ruby: warn "err"
来源：http://lk.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://ez.hahajie.cn

[M07] 判断是否为主入口
来源：http://vg.muxihuayi.cn

Py:   if __name__ == "__main__":
来源：http://he.521024.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ja.szsharing.cn

JS:   require.main === module
来源：http://xx.yuntaijiaju.cn

TS:   require.main === module
来源：http://fx.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://ke.bookmarksfly.cn

Go:   func main()
来源：http://qq.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uz.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://mc.panjiajie.cn

[M08] 获取系统与运行时信息
来源：http://cs.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://lf.nicolike.cn

PHP:  PHP_OS;  phpversion();
来源：http://on.huanxung.cn

JS:   process.platform;  process.version
来源：http://dt.huixinmuqiang.cn

TS:   process.platform;  process.version
来源：http://gi.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gp.bookmarksfly.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qw.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hl.chemitech.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zq.hnjuh.cn

================================================================================
来源：http://ii.nicolike.cn

N. 数据结构与算法
来源：http://cg.yuntaijiaju.cn

================================================================================
来源：http://yn.huanxung.cn

[N01] 二分查找（有序数组）
来源：http://xu.wgjwhj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gd.bookmarksfly.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ux.jctech888.com.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yx.asd995.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://um.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tv.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://ej.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ke.asd995.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kt.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://rf.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://tx.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hd.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://im.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kz.shxzukj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pg.hahajie.cn

Go:   slices.Sort(arr)
来源：http://mo.wgjwhj.cn

Ruby: arr.sort
来源：http://pz.shxzukj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xh.colortex.cn

[N03] 快速排序（分治示例）
来源：http://vh.nicolike.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aw.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://eq.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bb.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lr.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nv.hahajie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yz.huixinmuqiang.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aj.jianghongdianzi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vs.bookmarksfly.cn

[N04] 斐波那契数列
来源：http://ls.gzmigu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ji.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qn.colortex.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ea.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pz.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jc.colortex.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ou.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lt.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qd.bjjhwx.cn

[N05] 最大公约数
来源：http://zi.shxzukj.cn

Py:   math.gcd(a, b)
来源：http://jx.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oc.bjjhwx.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dy.521024.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nf.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://er.szsharing.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vd.hnjuh.cn

Ruby: a.gcd(b)
来源：http://zt.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ht.jianghongdianzi.cn

[N06] 判断回文字符串
来源：http://qw.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://lh.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://od.bjjhwx.cn

JS:   s === [...s].reverse().join("")
来源：http://tj.muxihuayi.cn

TS:   s === [...s].reverse().join("")
来源：http://it.wgjwhj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yd.huixinmuqiang.cn

Go:   // 双指针从两端比较
来源：http://qm.colortex.cn

Ruby: s == s.reverse
来源：http://ed.asd995.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ip.colortex.cn

[N07] 两数之和（返回下标）
来源：http://va.szxytkj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mp.huanxung.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pc.gzmigu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yh.wgjwhj.cn

TS:   // 手写 Map<string, number>
来源：http://pg.hnjuh.cn

Java: // 手写 HashMap
来源：http://ct.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://mu.jctech888.com.cn

Ruby: // 手写 Hash
来源：http://fc.yuexingan06.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cp.yuexingan06.cn

[N08] 生成全排列
来源：http://ww.bookmarksfly.cn

Py:   itertools.permutations(arr)
来源：http://nb.newstarts.cn

PHP:  // 手写递归交换
来源：http://dj.9csxet.cn

JS:   // 手写回溯递归
来源：http://qu.colortex.cn

TS:   // 手写回溯递归
来源：http://lh.521024.cn

Java: // 手写回溯递归
来源：http://wa.huanxung.cn

Go:   // 手写回溯递归
来源：http://ve.521024.cn

Ruby: arr.permutation.to_a
来源：http://xv.muxihuayi.cn

C#:   // 手写回溯递归
来源：http://fl.lnxyls.cn

[N09] 栈与队列
来源：http://df.521024.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tg.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ie.shxzukj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ox.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xz.szxytkj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ai.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oy.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cy.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ov.yuexingan06.cn

[N10] 链表节点定义
来源：http://eu.wgjwhj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://so.huixiangedu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wp.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ao.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://js.hnjuh.cn

Java: class Node { int v; Node next; }
来源：http://oi.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ft.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://oh.shxzskj.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ex.nicolike.cn

[N11] 二叉树中序遍历
来源：http://ld.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tz.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://zp.9csxet.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vh.panjiajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eb.gzmigu.cn

Java: // 手写递归
来源：http://vj.asd995.cn

Go:   // 手写递归
来源：http://oo.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gu.nszjky.cn

C#:   // 手写递归
来源：http://gx.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bo.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nb.jctech888.com.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kt.gzmigu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vb.panjiajie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tp.nszjky.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fu.shtwfgs.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gu.shtwfgs.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://di.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wo.haigaiapp.cn

================================================================================
来源：http://rs.shxzskj.cn

O. 并发与异步
来源：http://il.colortex.cn

================================================================================
来源：http://ey.9csxet.cn

[O01] 启动一个线程
来源：http://lk.wgjwhj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gs.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bl.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://md.hnjuh.cn

TS:   // 同 JS
来源：http://br.jctech888.com.cn

Java: new Thread(() -> f()).start()
来源：http://qq.bjjhwx.cn

Go:   go f()
来源：http://gp.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://qw.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://ko.bjjhwx.cn

[O02] 使用线程池
来源：http://wy.jctech888.com.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tz.nszjky.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ou.newstarts.cn

JS:   // worker_threads 线程池
来源：http://gl.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://eg.bookmarksfly.cn

Java: Executors.newFixedThreadPool(4)
来源：http://op.gzmigu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uf.jctech888.com.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fs.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yz.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://qt.hnjuh.cn

Py:   with lock: shared += 1
来源：http://fo.nszjky.cn

PHP:  // 用 flock() 做文件锁
来源：http://tk.szxytkj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cu.shxzskj.cn

TS:   // 同 JS
来源：http://si.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://np.gzmigu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ox.nicolike.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sf.jctech888.com.cn

C#:   lock (gate) { shared++; }
来源：http://dh.bjjhwx.cn

[O04] 定义异步函数并等待
来源：http://oz.521024.cn

Py:   async def f():⏎    await g()
来源：http://bx.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ca.yuntaijiaju.cn

JS:   async function f() { await g(); }
来源：http://zx.bjjhwx.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://di.muxihuayi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://am.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zw.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hh.hnjuh.cn

C#:   async Task F() { await G(); }
来源：http://jc.szsharing.cn

[O05] 并发执行并等待全部完成
来源：http://pf.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://hj.wgjwhj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://im.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://fe.nszjky.cn

TS:   await Promise.all(tasks)
来源：http://oi.huanxung.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yt.huanxung.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ph.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://je.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jl.shtwfgs.cn

[O06] 使用进程池
来源：http://fj.newstarts.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vy.yuntaijiaju.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cy.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://zb.newstarts.cn

TS:   // child_process / cluster 模块
来源：http://ic.colortex.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dl.panjiajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lr.gzmigu.cn

Ruby: // fork 块
来源：http://ai.9csxet.cn

C#:   Parallel.For
来源：http://si.shxzukj.cn

================================================================================
来源：http://mb.huanxung.cn

P. 常用工具函数
来源：http://on.jianghongdianzi.cn

================================================================================
来源：http://mq.bookmarksfly.cn


<!-- 参考信息 -->