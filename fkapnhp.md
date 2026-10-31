代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bw.gzmigu.cn

[L04] 设置超时
来源：http://oi.haigaiapp.cn

Py:   requests.get(url, timeout=5)
来源：http://hp.shtwfgs.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://al.chemitech.net.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://il.muxihuayi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nc.muxihuayi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://km.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cu.jianghongdianzi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ut.hahajie.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://oa.muxihuayi.cn

[L05] 上传文件（multipart）
来源：http://gq.newstarts.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yg.nszjky.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ju.colortex.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jl.szsharing.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ny.jianghongdianzi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ey.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qy.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nh.newstarts.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://qn.newstarts.cn

[L06] 解析响应为 JSON
来源：http://vl.yuntaijiaju.cn

Py:   resp.json()
来源：http://al.yuexingan06.cn

PHP:  json_decode($body, true);
来源：http://jh.asd995.cn

JS:   await resp.json()
来源：http://bx.gzmigu.cn

TS:   await resp.json()
来源：http://qo.bjjhwx.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tw.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rj.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://tz.shxzukj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xs.bookmarksfly.cn

[L07] 处理 HTTP 状态码
来源：http://ph.521024.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ba.hnjuh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mj.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://mq.szsharing.cn

TS:   resp.ok;  resp.status
来源：http://iz.nszjky.cn

Java: resp.statusCode()
来源：http://nv.colortex.cn

Go:   resp.StatusCode
来源：http://uo.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ld.hahajie.cn

C#:   (int)resp.StatusCode
来源：http://bx.yuexingan06.cn

[L08] 并发请求多个地址
来源：http://uy.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jg.szxytkj.cn

PHP:  curl_multi_init() 系列
来源：http://nl.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rx.huixiangedu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vt.colortex.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bk.nicolike.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://to.jianghongdianzi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mt.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oq.jctech888.com.cn

================================================================================
来源：http://ir.shxzskj.cn

M. 命令行 / 进程 / 环境
来源：http://bt.yuexingan06.cn

================================================================================
来源：http://gu.wgjwhj.cn

[M01] 读取命令行参数
来源：http://vk.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://ys.nszjky.cn

PHP:  $argv;  $argc;
来源：http://hc.9csxet.cn

JS:   process.argv.slice(2)
来源：http://iy.nszjky.cn

TS:   process.argv.slice(2)
来源：http://nz.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://xz.haigaiapp.cn

Go:   os.Args[1:]
来源：http://eb.shxzskj.cn

Ruby: ARGV
来源：http://ic.bjjhwx.cn

C#:   args 数组（Main 方法参数）
来源：http://zq.szxytkj.cn

[M02] 读取环境变量
来源：http://le.bookmarksfly.cn

Py:   os.environ.get("HOME")
来源：http://zt.gzmigu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ez.huixiangedu.cn

JS:   process.env.HOME
来源：http://px.panjiajie.cn

TS:   process.env.HOME
来源：http://uy.shxzskj.cn

Java: System.getenv("HOME")
来源：http://yr.huixiangedu.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cb.szxytkj.cn

Ruby: ENV["HOME"]
来源：http://gj.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uq.nicolike.cn

[M03] 执行外部命令
来源：http://ah.newstarts.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://df.szxytkj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ws.wgjwhj.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dr.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mq.panjiajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vm.chemitech.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qb.gzmigu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xs.chemitech.net.cn

C#:   Process.Start("ls", "-l");
来源：http://ly.9csxet.cn

[M04] 获取当前工作目录
来源：http://qs.hahajie.cn

Py:   os.getcwd()
来源：http://hd.yuexingan06.cn

PHP:  getcwd();
来源：http://wm.jianghongdianzi.cn

JS:   process.cwd()
来源：http://uv.chemitech.net.cn

TS:   process.cwd()
来源：http://dp.gzmigu.cn

Java: Path.of("").toAbsolutePath()
来源：http://em.huixiangedu.cn

Go:   os.Getwd()
来源：http://xg.521024.cn

Ruby: Dir.pwd
来源：http://lb.yuntaijiaju.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wm.jianghongdianzi.cn

[M05] 设置退出码
来源：http://mw.panjiajie.cn

Py:   sys.exit(1)
来源：http://sd.nszjky.cn

PHP:  exit(1);
来源：http://ry.yuexingan06.cn

JS:   process.exit(1)
来源：http://an.panjiajie.cn

TS:   process.exit(1)
来源：http://wf.hnjuh.cn

Java: System.exit(1)
来源：http://ms.yuexingan06.cn

Go:   os.Exit(1)
来源：http://lv.huanxung.cn

Ruby: exit 1
来源：http://pt.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ur.shxzukj.cn

[M06] 向标准错误输出
来源：http://vt.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://vo.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://sa.nicolike.cn

JS:   console.error("err")
来源：http://uz.shxzukj.cn

TS:   console.error("err")
来源：http://tm.panjiajie.cn

Java: System.err.println("err")
来源：http://rl.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nz.szsharing.cn

Ruby: warn "err"
来源：http://pp.bookmarksfly.cn

C#:   Console.Error.WriteLine("err")
来源：http://qv.bjjhwx.cn

[M07] 判断是否为主入口
来源：http://op.szxytkj.cn

Py:   if __name__ == "__main__":
来源：http://sh.muxihuayi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ou.newstarts.cn

JS:   require.main === module
来源：http://kp.521024.cn

TS:   require.main === module
来源：http://nk.haigaiapp.cn

Java: public static void main(String[] args)
来源：http://dt.bjjhwx.cn

Go:   func main()
来源：http://hv.nicolike.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ak.chemitech.net.cn

C#:   static void Main(string[] args)
来源：http://wq.521024.cn

[M08] 获取系统与运行时信息
来源：http://qg.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://ky.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://yk.hahajie.cn

JS:   process.platform;  process.version
来源：http://lr.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://gy.chemitech.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mo.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mx.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pn.huixiangedu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gn.jianghongdianzi.cn

================================================================================
来源：http://ze.szsharing.cn

N. 数据结构与算法
来源：http://zm.bookmarksfly.cn

================================================================================
来源：http://ak.szsharing.cn

[N01] 二分查找（有序数组）
来源：http://md.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oh.9csxet.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pu.huanxung.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gm.shxzukj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ys.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dc.asd995.cn

Go:   sort.SearchInts(arr, x)
来源：http://wb.nicolike.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://la.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lp.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://fd.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://xt.nicolike.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nm.bjjhwx.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zh.gzmigu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xp.huixinmuqiang.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cm.wgjwhj.cn

Go:   slices.Sort(arr)
来源：http://il.huixinmuqiang.cn

Ruby: arr.sort
来源：http://hh.huanxung.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vc.panjiajie.cn

[N03] 快速排序（分治示例）
来源：http://ya.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fn.bjjhwx.cn

PHP:  // 递归实现，或用 usort
来源：http://sv.jctech888.com.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qm.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fg.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ed.bookmarksfly.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xg.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qj.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bv.jianghongdianzi.cn

[N04] 斐波那契数列
来源：http://gf.hahajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hh.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mb.lnxyls.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rw.lnxyls.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bg.colortex.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ct.shxzskj.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yo.huixiangedu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://li.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://my.bookmarksfly.cn

[N05] 最大公约数
来源：http://xh.hnjuh.cn

Py:   math.gcd(a, b)
来源：http://gd.muxihuayi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lw.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hk.shxzukj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wo.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wm.hnjuh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mv.newstarts.cn

Ruby: a.gcd(b)
来源：http://hz.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://en.huixinmuqiang.cn

[N06] 判断回文字符串
来源：http://qk.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://sw.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://gu.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://uj.yuntaijiaju.cn

TS:   s === [...s].reverse().join("")
来源：http://su.jctech888.com.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tl.yuexingan06.cn

Go:   // 双指针从两端比较
来源：http://hb.bjjhwx.cn

Ruby: s == s.reverse
来源：http://em.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kp.newstarts.cn

[N07] 两数之和（返回下标）
来源：http://xr.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vy.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hh.9csxet.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ng.nicolike.cn

TS:   // 手写 Map<string, number>
来源：http://cb.newstarts.cn

Java: // 手写 HashMap
来源：http://rr.9csxet.cn

Go:   // 手写 map[int]int
来源：http://yn.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://rg.jianghongdianzi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://de.shtwfgs.cn

[N08] 生成全排列
来源：http://wp.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://bq.bjjhwx.cn

PHP:  // 手写递归交换
来源：http://pv.bookmarksfly.cn

JS:   // 手写回溯递归
来源：http://tn.haigaiapp.cn

TS:   // 手写回溯递归
来源：http://ch.hahajie.cn

Java: // 手写回溯递归
来源：http://kv.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://ra.shxzskj.cn

Ruby: arr.permutation.to_a
来源：http://lc.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://my.newstarts.cn

[N09] 栈与队列
来源：http://gc.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wn.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rg.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ho.newstarts.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://in.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gb.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bc.lnxyls.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hb.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cc.muxihuayi.cn

[N10] 链表节点定义
来源：http://vt.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ns.szsharing.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ss.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rc.huixinmuqiang.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dc.shtwfgs.cn

Java: class Node { int v; Node next; }
来源：http://cn.colortex.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hh.jctech888.com.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eh.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://br.panjiajie.cn

[N11] 二叉树中序遍历
来源：http://ft.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hd.bookmarksfly.cn

PHP:  // 手写递归函数
来源：http://xu.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://op.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mk.huixinmuqiang.cn

Java: // 手写递归
来源：http://fh.yuntaijiaju.cn

Go:   // 手写递归
来源：http://wk.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://od.szxytkj.cn

C#:   // 手写递归
来源：http://bh.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://go.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fe.hnjuh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://td.huixiangedu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iu.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dt.huanxung.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ba.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kd.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gk.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gc.haigaiapp.cn

================================================================================
来源：http://si.bookmarksfly.cn

O. 并发与异步
来源：http://nm.bjjhwx.cn

================================================================================
来源：http://fr.yuexingan06.cn

[O01] 启动一个线程
来源：http://jt.newstarts.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xn.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ca.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tp.shxzskj.cn

TS:   // 同 JS
来源：http://bj.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://za.huixiangedu.cn

Go:   go f()
来源：http://je.panjiajie.cn

Ruby: Thread.new { f }
来源：http://fq.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://ku.szsharing.cn

[O02] 使用线程池
来源：http://vq.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eo.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kk.newstarts.cn

JS:   // worker_threads 线程池
来源：http://oa.haigaiapp.cn

TS:   // worker_threads 线程池
来源：http://ht.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://al.wgjwhj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pt.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ks.jctech888.com.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pk.chemitech.net.cn

[O03] 加锁保护共享数据
来源：http://it.colortex.cn

Py:   with lock: shared += 1
来源：http://mh.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://ql.nicolike.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wh.jianghongdianzi.cn

TS:   // 同 JS
来源：http://rh.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://fs.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kl.jctech888.com.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ro.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://qw.shxzskj.cn

[O04] 定义异步函数并等待
来源：http://li.huanxung.cn

Py:   async def f():⏎    await g()
来源：http://ko.shxzukj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zj.shtwfgs.cn

JS:   async function f() { await g(); }
来源：http://vl.bookmarksfly.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rg.wgjwhj.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gq.jctech888.com.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dp.nszjky.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qz.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://jz.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://tx.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://ec.9csxet.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ky.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://ap.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://nk.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xu.muxihuayi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pa.shtwfgs.cn

Ruby: threads.map(&:join)
来源：http://jp.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sl.bookmarksfly.cn

[O06] 使用进程池
来源：http://jx.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yg.panjiajie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lb.shxzskj.cn

JS:   // child_process / cluster 模块
来源：http://si.shxzskj.cn

TS:   // child_process / cluster 模块
来源：http://fm.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fj.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hx.szxytkj.cn

Ruby: // fork 块
来源：http://ln.521024.cn

C#:   Parallel.For
来源：http://ph.hahajie.cn

================================================================================
来源：http://zm.lnxyls.cn

P. 常用工具函数
来源：http://rj.9csxet.cn

================================================================================
来源：http://rb.jctech888.com.cn

[P01] 生成 UUID
来源：http://fq.huanxung.cn

Py:   str(uuid.uuid4())
来源：http://jy.nszjky.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xt.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://at.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://ur.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://xq.panjiajie.cn

Go:   // 用 github.com/google/uuid
来源：http://bg.huixiangedu.cn

Ruby: SecureRandom.uuid
来源：http://lt.huixiangedu.cn


<!-- 参考信息 -->