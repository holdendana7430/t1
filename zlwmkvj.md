代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tj.huixinmuqiang.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ni.szxytkj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zf.shxzskj.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://si.haigaiapp.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pm.shxzukj.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ak.huanxung.cn

[L05] 上传文件（multipart）
来源：http://ow.nicolike.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://rl.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kb.huixinmuqiang.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sl.shxzskj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pv.muxihuayi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pb.szxytkj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kr.wgjwhj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zl.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zp.nicolike.cn

[L06] 解析响应为 JSON
来源：http://rm.chemitech.net.cn

Py:   resp.json()
来源：http://nn.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://zj.shtwfgs.cn

JS:   await resp.json()
来源：http://qi.gzmigu.cn

TS:   await resp.json()
来源：http://zy.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gq.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vd.szxytkj.cn

Ruby: JSON.parse(resp.body)
来源：http://ya.huixiangedu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hk.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://tw.shxzskj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fq.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bu.nicolike.cn

JS:   resp.ok;  resp.status
来源：http://lk.haigaiapp.cn

TS:   resp.ok;  resp.status
来源：http://lz.szxytkj.cn

Java: resp.statusCode()
来源：http://ho.hnjuh.cn

Go:   resp.StatusCode
来源：http://mk.hnjuh.cn

Ruby: resp.code.to_i
来源：http://mb.9csxet.cn

C#:   (int)resp.StatusCode
来源：http://xf.9csxet.cn

[L08] 并发请求多个地址
来源：http://gb.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gu.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://yy.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ja.huanxung.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sr.panjiajie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xn.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://em.nicolike.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zq.panjiajie.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ad.jctech888.com.cn

================================================================================
来源：http://wt.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://co.newstarts.cn

================================================================================
来源：http://vm.panjiajie.cn

[M01] 读取命令行参数
来源：http://oh.hahajie.cn

Py:   sys.argv[1:]
来源：http://pj.colortex.cn

PHP:  $argv;  $argc;
来源：http://hf.muxihuayi.cn

JS:   process.argv.slice(2)
来源：http://wg.9csxet.cn

TS:   process.argv.slice(2)
来源：http://yj.yuexingan06.cn

Java: args 数组（main 方法参数）
来源：http://dt.lnxyls.cn

Go:   os.Args[1:]
来源：http://hn.chemitech.net.cn

Ruby: ARGV
来源：http://by.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://sq.szxytkj.cn

[M02] 读取环境变量
来源：http://ka.haigaiapp.cn

Py:   os.environ.get("HOME")
来源：http://iy.colortex.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wh.huixiangedu.cn

JS:   process.env.HOME
来源：http://tx.wgjwhj.cn

TS:   process.env.HOME
来源：http://ig.hnjuh.cn

Java: System.getenv("HOME")
来源：http://yr.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ny.9csxet.cn

Ruby: ENV["HOME"]
来源：http://ic.9csxet.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xz.nicolike.cn

[M03] 执行外部命令
来源：http://qf.chemitech.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hq.huanxung.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vc.hahajie.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xy.huixinmuqiang.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ic.szxytkj.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gk.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aj.yuexingan06.cn

Ruby: system("ls -l");  `ls -l`
来源：http://vh.hnjuh.cn

C#:   Process.Start("ls", "-l");
来源：http://wl.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://zx.newstarts.cn

Py:   os.getcwd()
来源：http://fc.shtwfgs.cn

PHP:  getcwd();
来源：http://ee.shxzskj.cn

JS:   process.cwd()
来源：http://ts.jianghongdianzi.cn

TS:   process.cwd()
来源：http://li.haigaiapp.cn

Java: Path.of("").toAbsolutePath()
来源：http://mg.huanxung.cn

Go:   os.Getwd()
来源：http://qv.9csxet.cn

Ruby: Dir.pwd
来源：http://ts.colortex.cn

C#:   Directory.GetCurrentDirectory()
来源：http://cc.jianghongdianzi.cn

[M05] 设置退出码
来源：http://mk.panjiajie.cn

Py:   sys.exit(1)
来源：http://ao.huanxung.cn

PHP:  exit(1);
来源：http://sv.szsharing.cn

JS:   process.exit(1)
来源：http://jq.bookmarksfly.cn

TS:   process.exit(1)
来源：http://rn.lnxyls.cn

Java: System.exit(1)
来源：http://ro.asd995.cn

Go:   os.Exit(1)
来源：http://wo.newstarts.cn

Ruby: exit 1
来源：http://qj.shxzskj.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qw.colortex.cn

[M06] 向标准错误输出
来源：http://ln.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://he.hnjuh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://er.asd995.cn

JS:   console.error("err")
来源：http://vu.bookmarksfly.cn

TS:   console.error("err")
来源：http://zi.shtwfgs.cn

Java: System.err.println("err")
来源：http://hg.chemitech.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wm.bjjhwx.cn

Ruby: warn "err"
来源：http://xw.lnxyls.cn

C#:   Console.Error.WriteLine("err")
来源：http://nq.nicolike.cn

[M07] 判断是否为主入口
来源：http://sx.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://wt.szsharing.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ve.shxzskj.cn

JS:   require.main === module
来源：http://cl.huixinmuqiang.cn

TS:   require.main === module
来源：http://mf.bjjhwx.cn

Java: public static void main(String[] args)
来源：http://ts.yuntaijiaju.cn

Go:   func main()
来源：http://dl.shxzukj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jp.nszjky.cn

C#:   static void Main(string[] args)
来源：http://nl.bjjhwx.cn

[M08] 获取系统与运行时信息
来源：http://et.huanxung.cn

Py:   platform.system();  platform.python_version()
来源：http://ph.haigaiapp.cn

PHP:  PHP_OS;  phpversion();
来源：http://qz.wgjwhj.cn

JS:   process.platform;  process.version
来源：http://yk.nszjky.cn

TS:   process.platform;  process.version
来源：http://zk.wgjwhj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gn.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ic.chemitech.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bc.bjjhwx.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xw.colortex.cn

================================================================================
来源：http://uy.521024.cn

N. 数据结构与算法
来源：http://iu.nszjky.cn

================================================================================
来源：http://qp.nicolike.cn

[N01] 二分查找（有序数组）
来源：http://ve.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sn.bjjhwx.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ot.521024.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ah.hnjuh.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fs.muxihuayi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://my.colortex.cn

Go:   sort.SearchInts(arr, x)
来源：http://ts.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ef.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ga.gzmigu.cn

[N02] 排序（工程实践用内置实现）
来源：http://uk.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://zy.shtwfgs.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dw.szsharing.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ak.szxytkj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aq.gzmigu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sp.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://xe.muxihuayi.cn

Ruby: arr.sort
来源：http://sr.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sd.muxihuayi.cn

[N03] 快速排序（分治示例）
来源：http://qi.chemitech.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qz.nicolike.cn

PHP:  // 递归实现，或用 usort
来源：http://zf.muxihuayi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wn.colortex.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gq.szxytkj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sc.yuntaijiaju.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ly.chemitech.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cm.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oj.bjjhwx.cn

[N04] 斐波那契数列
来源：http://ut.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jf.huanxung.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gk.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pk.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zu.nszjky.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xb.521024.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vr.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tv.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qk.9csxet.cn

[N05] 最大公约数
来源：http://uy.colortex.cn

Py:   math.gcd(a, b)
来源：http://xe.bookmarksfly.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fp.hahajie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tz.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uz.panjiajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://es.asd995.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yy.newstarts.cn

Ruby: a.gcd(b)
来源：http://cg.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cx.521024.cn

[N06] 判断回文字符串
来源：http://ma.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://ml.bjjhwx.cn

PHP:  $s === strrev($s);
来源：http://vj.muxihuayi.cn

JS:   s === [...s].reverse().join("")
来源：http://wd.bookmarksfly.cn

TS:   s === [...s].reverse().join("")
来源：http://vf.szxytkj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ow.nszjky.cn

Go:   // 双指针从两端比较
来源：http://ha.521024.cn

Ruby: s == s.reverse
来源：http://px.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lb.huanxung.cn

[N07] 两数之和（返回下标）
来源：http://bg.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bf.shxzskj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vr.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ov.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://dv.shxzukj.cn

Java: // 手写 HashMap
来源：http://fq.hahajie.cn

Go:   // 手写 map[int]int
来源：http://az.bjjhwx.cn

Ruby: // 手写 Hash
来源：http://ra.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cq.huanxung.cn

[N08] 生成全排列
来源：http://cu.gzmigu.cn

Py:   itertools.permutations(arr)
来源：http://cq.9csxet.cn

PHP:  // 手写递归交换
来源：http://dy.haigaiapp.cn

JS:   // 手写回溯递归
来源：http://bb.huixiangedu.cn

TS:   // 手写回溯递归
来源：http://rt.shxzukj.cn

Java: // 手写回溯递归
来源：http://qi.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://ux.jctech888.com.cn

Ruby: arr.permutation.to_a
来源：http://uh.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://pq.panjiajie.cn

[N09] 栈与队列
来源：http://qd.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cs.haigaiapp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iq.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zl.bjjhwx.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yp.huixinmuqiang.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://du.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xr.wgjwhj.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rj.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tf.nicolike.cn

[N10] 链表节点定义
来源：http://rs.shxzskj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cy.shxzukj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kf.gzmigu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cw.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hv.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://ks.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://im.shtwfgs.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xs.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://gi.shxzukj.cn

[N11] 二叉树中序遍历
来源：http://iv.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fo.hnjuh.cn

PHP:  // 手写递归函数
来源：http://pg.shxzskj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yt.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://js.jctech888.com.cn

Java: // 手写递归
来源：http://zh.szsharing.cn

Go:   // 手写递归
来源：http://vm.szsharing.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pg.shxzskj.cn

C#:   // 手写递归
来源：http://xj.chemitech.net.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rw.yuntaijiaju.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fc.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ti.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yk.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qg.hnjuh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nn.gzmigu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hl.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qm.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.gzmigu.cn

================================================================================
来源：http://nw.colortex.cn

O. 并发与异步
来源：http://lo.bookmarksfly.cn

================================================================================
来源：http://im.huixinmuqiang.cn

[O01] 启动一个线程
来源：http://gc.jctech888.com.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pv.shxzukj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dl.shtwfgs.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qs.panjiajie.cn

TS:   // 同 JS
来源：http://dn.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://dd.panjiajie.cn

Go:   go f()
来源：http://hr.yuntaijiaju.cn

Ruby: Thread.new { f }
来源：http://wd.lnxyls.cn

C#:   Task.Run(() => F());
来源：http://ur.newstarts.cn

[O02] 使用线程池
来源：http://dn.yuntaijiaju.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ll.shxzskj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sc.chemitech.net.cn

JS:   // worker_threads 线程池
来源：http://uu.huanxung.cn

TS:   // worker_threads 线程池
来源：http://kk.haigaiapp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tq.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rc.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vj.haigaiapp.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dz.shxzukj.cn

[O03] 加锁保护共享数据
来源：http://kr.huixiangedu.cn

Py:   with lock: shared += 1
来源：http://wg.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://wk.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yh.gzmigu.cn

TS:   // 同 JS
来源：http://lp.hnjuh.cn

Java: synchronized (this) { shared++; }
来源：http://tj.shtwfgs.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tv.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bj.muxihuayi.cn

C#:   lock (gate) { shared++; }
来源：http://mw.huixinmuqiang.cn

[O04] 定义异步函数并等待
来源：http://im.panjiajie.cn

Py:   async def f():⏎    await g()
来源：http://pm.yuntaijiaju.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bp.hnjuh.cn

JS:   async function f() { await g(); }
来源：http://nc.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dn.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wa.szxytkj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oz.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yx.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://we.shxzukj.cn

[O05] 并发执行并等待全部完成
来源：http://xa.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://gd.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ik.shxzukj.cn

JS:   await Promise.all(tasks)
来源：http://xp.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://in.lnxyls.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bj.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://am.colortex.cn

Ruby: threads.map(&:join)
来源：http://ai.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jc.yuntaijiaju.cn

[O06] 使用进程池
来源：http://un.chemitech.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lx.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mw.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://pu.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://qc.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xc.hnjuh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ew.jianghongdianzi.cn

Ruby: // fork 块
来源：http://rk.szsharing.cn

C#:   Parallel.For
来源：http://vs.shxzukj.cn

================================================================================
来源：http://jr.gzmigu.cn

P. 常用工具函数
来源：http://qy.nicolike.cn

================================================================================
来源：http://dj.9csxet.cn

[P01] 生成 UUID
来源：http://af.colortex.cn

Py:   str(uuid.uuid4())
来源：http://md.hahajie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xc.newstarts.cn

JS:   crypto.randomUUID()
来源：http://db.jianghongdianzi.cn

TS:   crypto.randomUUID()
来源：http://ia.muxihuayi.cn

Java: UUID.randomUUID().toString()
来源：http://ph.lnxyls.cn

Go:   // 用 github.com/google/uuid
来源：http://pf.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://mm.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://yi.lnxyls.cn

[P02] MD5 / SHA256 摘要
来源：http://dv.szxytkj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fj.lnxyls.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kw.szsharing.cn


<!-- 参考信息 -->