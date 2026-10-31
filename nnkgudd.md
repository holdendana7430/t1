代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pb.chemitech.net.cn

[L04] 设置超时
来源：http://hd.hahajie.cn

Py:   requests.get(url, timeout=5)
来源：http://my.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cc.hnjuh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lh.bookmarksfly.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zy.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mj.521024.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://in.nicolike.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jn.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jq.nszjky.cn

[L05] 上传文件（multipart）
来源：http://pq.yuexingan06.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ed.bookmarksfly.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fn.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yj.muxihuayi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gm.asd995.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fi.huixiangedu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ea.colortex.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nz.hnjuh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sh.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://mq.yuntaijiaju.cn

Py:   resp.json()
来源：http://zg.yuntaijiaju.cn

PHP:  json_decode($body, true);
来源：http://vp.huixiangedu.cn

JS:   await resp.json()
来源：http://qy.haigaiapp.cn

TS:   await resp.json()
来源：http://bn.asd995.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://uy.hnjuh.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bg.nszjky.cn

Ruby: JSON.parse(resp.body)
来源：http://ff.newstarts.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nw.huixinmuqiang.cn

[L07] 处理 HTTP 状态码
来源：http://bw.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ql.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ek.panjiajie.cn

JS:   resp.ok;  resp.status
来源：http://ts.hnjuh.cn

TS:   resp.ok;  resp.status
来源：http://ah.shxzskj.cn

Java: resp.statusCode()
来源：http://zi.hnjuh.cn

Go:   resp.StatusCode
来源：http://wq.huanxung.cn

Ruby: resp.code.to_i
来源：http://hb.gzmigu.cn

C#:   (int)resp.StatusCode
来源：http://uv.szsharing.cn

[L08] 并发请求多个地址
来源：http://gr.panjiajie.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ag.szsharing.cn

PHP:  curl_multi_init() 系列
来源：http://gk.szxytkj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pi.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gl.nszjky.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bw.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xm.shtwfgs.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://aw.bjjhwx.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://as.bookmarksfly.cn

================================================================================
来源：http://aa.asd995.cn

M. 命令行 / 进程 / 环境
来源：http://mw.chemitech.net.cn

================================================================================
来源：http://xf.huanxung.cn

[M01] 读取命令行参数
来源：http://sw.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://kw.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://bg.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://qa.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://yx.muxihuayi.cn

Java: args 数组（main 方法参数）
来源：http://yw.huanxung.cn

Go:   os.Args[1:]
来源：http://bi.newstarts.cn

Ruby: ARGV
来源：http://ue.newstarts.cn

C#:   args 数组（Main 方法参数）
来源：http://zi.huanxung.cn

[M02] 读取环境变量
来源：http://za.9csxet.cn

Py:   os.environ.get("HOME")
来源：http://cs.szxytkj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jc.muxihuayi.cn

JS:   process.env.HOME
来源：http://cf.hahajie.cn

TS:   process.env.HOME
来源：http://jd.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://fk.shtwfgs.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tc.huixiangedu.cn

Ruby: ENV["HOME"]
来源：http://nj.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hl.chemitech.net.cn

[M03] 执行外部命令
来源：http://mn.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://se.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ki.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ii.yuntaijiaju.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://vj.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ci.521024.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://up.huixiangedu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ah.gzmigu.cn

C#:   Process.Start("ls", "-l");
来源：http://gn.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://xn.muxihuayi.cn

Py:   os.getcwd()
来源：http://jo.muxihuayi.cn

PHP:  getcwd();
来源：http://hx.shtwfgs.cn

JS:   process.cwd()
来源：http://ly.nszjky.cn

TS:   process.cwd()
来源：http://uh.jctech888.com.cn

Java: Path.of("").toAbsolutePath()
来源：http://ph.huanxung.cn

Go:   os.Getwd()
来源：http://wn.shxzskj.cn

Ruby: Dir.pwd
来源：http://zb.9csxet.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iw.szxytkj.cn

[M05] 设置退出码
来源：http://jm.panjiajie.cn

Py:   sys.exit(1)
来源：http://jt.panjiajie.cn

PHP:  exit(1);
来源：http://co.haigaiapp.cn

JS:   process.exit(1)
来源：http://wk.521024.cn

TS:   process.exit(1)
来源：http://ri.szsharing.cn

Java: System.exit(1)
来源：http://tk.asd995.cn

Go:   os.Exit(1)
来源：http://sm.hahajie.cn

Ruby: exit 1
来源：http://xr.hnjuh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://td.yuexingan06.cn

[M06] 向标准错误输出
来源：http://ro.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://wu.szsharing.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ra.newstarts.cn

JS:   console.error("err")
来源：http://fv.nicolike.cn

TS:   console.error("err")
来源：http://dm.jianghongdianzi.cn

Java: System.err.println("err")
来源：http://ic.hahajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gx.huixiangedu.cn

Ruby: warn "err"
来源：http://kr.haigaiapp.cn

C#:   Console.Error.WriteLine("err")
来源：http://zc.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://ge.shtwfgs.cn

Py:   if __name__ == "__main__":
来源：http://ew.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ww.huixiangedu.cn

JS:   require.main === module
来源：http://la.chemitech.net.cn

TS:   require.main === module
来源：http://du.bookmarksfly.cn

Java: public static void main(String[] args)
来源：http://ws.panjiajie.cn

Go:   func main()
来源：http://te.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mt.lnxyls.cn

C#:   static void Main(string[] args)
来源：http://ex.yuexingan06.cn

[M08] 获取系统与运行时信息
来源：http://ok.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://xw.jianghongdianzi.cn

PHP:  PHP_OS;  phpversion();
来源：http://qi.szxytkj.cn

JS:   process.platform;  process.version
来源：http://iq.colortex.cn

TS:   process.platform;  process.version
来源：http://ks.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lv.nicolike.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://os.wgjwhj.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fr.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://iz.nszjky.cn

================================================================================
来源：http://ur.chemitech.net.cn

N. 数据结构与算法
来源：http://ys.asd995.cn

================================================================================
来源：http://nq.hnjuh.cn

[N01] 二分查找（有序数组）
来源：http://wo.huixiangedu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bl.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://um.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ro.colortex.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cw.hnjuh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wk.hahajie.cn

Go:   sort.SearchInts(arr, x)
来源：http://uq.muxihuayi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vi.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ce.chemitech.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://xb.bookmarksfly.cn

Py:   sorted(arr);  arr.sort()
来源：http://on.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xc.521024.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sy.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sp.jctech888.com.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gb.colortex.cn

Go:   slices.Sort(arr)
来源：http://ip.asd995.cn

Ruby: arr.sort
来源：http://tc.521024.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xo.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://lr.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wo.hahajie.cn

PHP:  // 递归实现，或用 usort
来源：http://vi.hahajie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ys.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kg.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vz.shxzukj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ak.panjiajie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jp.muxihuayi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pf.nszjky.cn

[N04] 斐波那契数列
来源：http://av.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ls.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vq.hahajie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wy.bjjhwx.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://po.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cc.shxzukj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gg.gzmigu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cj.huixinmuqiang.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wz.chemitech.net.cn

[N05] 最大公约数
来源：http://ii.panjiajie.cn

Py:   math.gcd(a, b)
来源：http://gn.huanxung.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vo.szxytkj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tn.hahajie.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vb.nszjky.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wh.chemitech.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rl.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://ev.shtwfgs.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lg.panjiajie.cn

[N06] 判断回文字符串
来源：http://ih.huixiangedu.cn

Py:   s == s[::-1]
来源：http://zb.lnxyls.cn

PHP:  $s === strrev($s);
来源：http://en.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://ji.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://bb.hahajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tk.jctech888.com.cn

Go:   // 双指针从两端比较
来源：http://dv.hahajie.cn

Ruby: s == s.reverse
来源：http://nc.shtwfgs.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://aa.bookmarksfly.cn

[N07] 两数之和（返回下标）
来源：http://bz.hahajie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cy.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sz.wgjwhj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ze.huanxung.cn

TS:   // 手写 Map<string, number>
来源：http://em.huixinmuqiang.cn

Java: // 手写 HashMap
来源：http://el.nszjky.cn

Go:   // 手写 map[int]int
来源：http://de.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://ix.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bc.yuntaijiaju.cn

[N08] 生成全排列
来源：http://wh.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://lx.huanxung.cn

PHP:  // 手写递归交换
来源：http://bf.szxytkj.cn

JS:   // 手写回溯递归
来源：http://ib.jctech888.com.cn

TS:   // 手写回溯递归
来源：http://lz.huanxung.cn

Java: // 手写回溯递归
来源：http://oi.huixinmuqiang.cn

Go:   // 手写回溯递归
来源：http://tv.huixiangedu.cn

Ruby: arr.permutation.to_a
来源：http://ct.huixinmuqiang.cn

C#:   // 手写回溯递归
来源：http://of.newstarts.cn

[N09] 栈与队列
来源：http://jv.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oy.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dy.hnjuh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dx.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ja.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bu.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ej.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cr.bjjhwx.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rh.bookmarksfly.cn

[N10] 链表节点定义
来源：http://st.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fe.gzmigu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xv.shxzukj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qk.asd995.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yx.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://pb.jianghongdianzi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://sx.jianghongdianzi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://on.haigaiapp.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ag.jctech888.com.cn

[N11] 二叉树中序遍历
来源：http://sq.hahajie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yi.9csxet.cn

PHP:  // 手写递归函数
来源：http://ha.yuexingan06.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xa.asd995.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pv.hnjuh.cn

Java: // 手写递归
来源：http://xo.9csxet.cn

Go:   // 手写递归
来源：http://nx.wgjwhj.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zq.muxihuayi.cn

C#:   // 手写递归
来源：http://om.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ug.hahajie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ov.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ir.nicolike.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nn.shxzukj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pd.jianghongdianzi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nu.jianghongdianzi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tm.521024.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kl.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iy.szxytkj.cn

================================================================================
来源：http://pv.wgjwhj.cn

O. 并发与异步
来源：http://ch.asd995.cn

================================================================================
来源：http://th.nicolike.cn

[O01] 启动一个线程
来源：http://vd.huanxung.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uw.szxytkj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zi.huixiangedu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://af.szxytkj.cn

TS:   // 同 JS
来源：http://ht.asd995.cn

Java: new Thread(() -> f()).start()
来源：http://up.nszjky.cn

Go:   go f()
来源：http://bv.jianghongdianzi.cn

Ruby: Thread.new { f }
来源：http://yt.nicolike.cn

C#:   Task.Run(() => F());
来源：http://ob.asd995.cn

[O02] 使用线程池
来源：http://xa.nszjky.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eq.gzmigu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eg.jianghongdianzi.cn

JS:   // worker_threads 线程池
来源：http://jh.asd995.cn

TS:   // worker_threads 线程池
来源：http://zj.wgjwhj.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wq.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sd.newstarts.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bk.newstarts.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sy.hnjuh.cn

[O03] 加锁保护共享数据
来源：http://hz.yuexingan06.cn

Py:   with lock: shared += 1
来源：http://xc.9csxet.cn

PHP:  // 用 flock() 做文件锁
来源：http://xr.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vd.hahajie.cn

TS:   // 同 JS
来源：http://qy.huixinmuqiang.cn

Java: synchronized (this) { shared++; }
来源：http://lc.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://em.gzmigu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jz.yuntaijiaju.cn

C#:   lock (gate) { shared++; }
来源：http://fi.haigaiapp.cn

[O04] 定义异步函数并等待
来源：http://oq.szsharing.cn

Py:   async def f():⏎    await g()
来源：http://xh.chemitech.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wv.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://ni.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fc.yuntaijiaju.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jl.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lj.9csxet.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kf.colortex.cn

C#:   async Task F() { await G(); }
来源：http://uo.szxytkj.cn

[O05] 并发执行并等待全部完成
来源：http://dy.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://gn.nszjky.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ph.gzmigu.cn

JS:   await Promise.all(tasks)
来源：http://sj.nicolike.cn

TS:   await Promise.all(tasks)
来源：http://vx.huixiangedu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dk.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zs.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://vx.yuexingan06.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rp.bookmarksfly.cn

[O06] 使用进程池
来源：http://aj.521024.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zo.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qj.9csxet.cn

JS:   // child_process / cluster 模块
来源：http://fn.huanxung.cn

TS:   // child_process / cluster 模块
来源：http://ij.asd995.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tk.newstarts.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fe.hahajie.cn

Ruby: // fork 块
来源：http://ib.panjiajie.cn

C#:   Parallel.For
来源：http://mp.nszjky.cn

================================================================================
来源：http://ck.wgjwhj.cn

P. 常用工具函数
来源：http://gt.chemitech.net.cn

================================================================================
来源：http://gl.huanxung.cn

[P01] 生成 UUID
来源：http://zu.jianghongdianzi.cn

Py:   str(uuid.uuid4())
来源：http://vj.jianghongdianzi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xw.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://qd.haigaiapp.cn

TS:   crypto.randomUUID()
来源：http://xa.yuntaijiaju.cn

Java: UUID.randomUUID().toString()
来源：http://ws.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://ln.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://uv.hahajie.cn


<!-- 参考信息 -->