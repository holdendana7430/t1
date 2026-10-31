代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pm.9csxet.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cm.jctech888.com.cn

[L05] 上传文件（multipart）
来源：http://wp.haigaiapp.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qb.lnxyls.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://db.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gj.asd995.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bc.521024.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nr.hnjuh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://in.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vw.gzmigu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xe.muxihuayi.cn

[L06] 解析响应为 JSON
来源：http://gv.muxihuayi.cn

Py:   resp.json()
来源：http://rv.nicolike.cn

PHP:  json_decode($body, true);
来源：http://om.shxzskj.cn

JS:   await resp.json()
来源：http://tw.jianghongdianzi.cn

TS:   await resp.json()
来源：http://fp.colortex.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://gn.shxzukj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qr.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://mt.bjjhwx.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gp.asd995.cn

[L07] 处理 HTTP 状态码
来源：http://rg.huanxung.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wu.bookmarksfly.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ne.szsharing.cn

JS:   resp.ok;  resp.status
来源：http://je.huixinmuqiang.cn

TS:   resp.ok;  resp.status
来源：http://tt.huixinmuqiang.cn

Java: resp.statusCode()
来源：http://up.chemitech.net.cn

Go:   resp.StatusCode
来源：http://va.521024.cn

Ruby: resp.code.to_i
来源：http://fv.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://vk.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://qr.newstarts.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xe.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://ce.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sn.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vl.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://om.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zc.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wl.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mj.hahajie.cn

================================================================================
来源：http://mi.nszjky.cn

M. 命令行 / 进程 / 环境
来源：http://pg.yuexingan06.cn

================================================================================
来源：http://lr.szxytkj.cn

[M01] 读取命令行参数
来源：http://qt.huixinmuqiang.cn

Py:   sys.argv[1:]
来源：http://lk.wgjwhj.cn

PHP:  $argv;  $argc;
来源：http://nk.shxzskj.cn

JS:   process.argv.slice(2)
来源：http://ps.521024.cn

TS:   process.argv.slice(2)
来源：http://fn.huixiangedu.cn

Java: args 数组（main 方法参数）
来源：http://sd.shtwfgs.cn

Go:   os.Args[1:]
来源：http://vb.hnjuh.cn

Ruby: ARGV
来源：http://mb.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://ui.newstarts.cn

[M02] 读取环境变量
来源：http://sh.shxzskj.cn

Py:   os.environ.get("HOME")
来源：http://nu.jianghongdianzi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rd.huixiangedu.cn

JS:   process.env.HOME
来源：http://pg.bookmarksfly.cn

TS:   process.env.HOME
来源：http://uk.hahajie.cn

Java: System.getenv("HOME")
来源：http://xy.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://oh.szsharing.cn

Ruby: ENV["HOME"]
来源：http://mx.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://da.colortex.cn

[M03] 执行外部命令
来源：http://ee.bjjhwx.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lw.wgjwhj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://km.nicolike.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fx.shxzukj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ue.hahajie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ha.bookmarksfly.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://us.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uq.nicolike.cn

C#:   Process.Start("ls", "-l");
来源：http://cb.huixinmuqiang.cn

[M04] 获取当前工作目录
来源：http://mc.newstarts.cn

Py:   os.getcwd()
来源：http://ak.chemitech.net.cn

PHP:  getcwd();
来源：http://kh.shtwfgs.cn

JS:   process.cwd()
来源：http://lw.szxytkj.cn

TS:   process.cwd()
来源：http://wv.jianghongdianzi.cn

Java: Path.of("").toAbsolutePath()
来源：http://ch.9csxet.cn

Go:   os.Getwd()
来源：http://ds.bjjhwx.cn

Ruby: Dir.pwd
来源：http://ru.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ne.shtwfgs.cn

[M05] 设置退出码
来源：http://nj.colortex.cn

Py:   sys.exit(1)
来源：http://ph.chemitech.net.cn

PHP:  exit(1);
来源：http://qx.hahajie.cn

JS:   process.exit(1)
来源：http://cw.hahajie.cn

TS:   process.exit(1)
来源：http://ac.gzmigu.cn

Java: System.exit(1)
来源：http://ut.panjiajie.cn

Go:   os.Exit(1)
来源：http://gw.yuntaijiaju.cn

Ruby: exit 1
来源：http://yy.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qi.szxytkj.cn

[M06] 向标准错误输出
来源：http://bj.huanxung.cn

Py:   print("err", file=sys.stderr)
来源：http://ev.yuexingan06.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uh.bjjhwx.cn

JS:   console.error("err")
来源：http://ii.hahajie.cn

TS:   console.error("err")
来源：http://pf.szxytkj.cn

Java: System.err.println("err")
来源：http://rb.huanxung.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ci.bjjhwx.cn

Ruby: warn "err"
来源：http://ez.colortex.cn

C#:   Console.Error.WriteLine("err")
来源：http://dq.shxzskj.cn

[M07] 判断是否为主入口
来源：http://zk.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://ct.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fs.521024.cn

JS:   require.main === module
来源：http://gz.huixiangedu.cn

TS:   require.main === module
来源：http://xc.newstarts.cn

Java: public static void main(String[] args)
来源：http://qx.hnjuh.cn

Go:   func main()
来源：http://im.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qc.yuexingan06.cn

C#:   static void Main(string[] args)
来源：http://yx.szsharing.cn

[M08] 获取系统与运行时信息
来源：http://bu.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://lu.jctech888.com.cn

PHP:  PHP_OS;  phpversion();
来源：http://jm.hahajie.cn

JS:   process.platform;  process.version
来源：http://jj.nicolike.cn

TS:   process.platform;  process.version
来源：http://mw.asd995.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ej.jianghongdianzi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dj.bookmarksfly.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qs.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hy.shxzskj.cn

================================================================================
来源：http://er.shxzukj.cn

N. 数据结构与算法
来源：http://qc.shxzukj.cn

================================================================================
来源：http://ax.yuntaijiaju.cn

[N01] 二分查找（有序数组）
来源：http://fh.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wa.hahajie.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cq.muxihuayi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yo.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ht.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dy.szsharing.cn

Go:   sort.SearchInts(arr, x)
来源：http://mm.shxzskj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ph.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zf.wgjwhj.cn

[N02] 排序（工程实践用内置实现）
来源：http://ib.shtwfgs.cn

Py:   sorted(arr);  arr.sort()
来源：http://rh.szxytkj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pa.lnxyls.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yd.szsharing.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://up.asd995.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aa.9csxet.cn

Go:   slices.Sort(arr)
来源：http://uf.nszjky.cn

Ruby: arr.sort
来源：http://tc.gzmigu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jx.huixiangedu.cn

[N03] 快速排序（分治示例）
来源：http://yo.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hb.521024.cn

PHP:  // 递归实现，或用 usort
来源：http://nr.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dx.jianghongdianzi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wn.wgjwhj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yl.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ct.muxihuayi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zq.bookmarksfly.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ra.muxihuayi.cn

[N04] 斐波那契数列
来源：http://oh.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yi.haigaiapp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gm.521024.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fc.szxytkj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hf.nicolike.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gr.haigaiapp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eu.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://us.shxzukj.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gp.nicolike.cn

[N05] 最大公约数
来源：http://nw.chemitech.net.cn

Py:   math.gcd(a, b)
来源：http://kg.wgjwhj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fr.huanxung.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dw.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qc.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tf.yuexingan06.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ic.jianghongdianzi.cn

Ruby: a.gcd(b)
来源：http://fa.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ek.yuexingan06.cn

[N06] 判断回文字符串
来源：http://tm.yuexingan06.cn

Py:   s == s[::-1]
来源：http://af.szsharing.cn

PHP:  $s === strrev($s);
来源：http://ol.lnxyls.cn

JS:   s === [...s].reverse().join("")
来源：http://dw.shtwfgs.cn

TS:   s === [...s].reverse().join("")
来源：http://iu.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oq.bookmarksfly.cn

Go:   // 双指针从两端比较
来源：http://ar.bjjhwx.cn

Ruby: s == s.reverse
来源：http://ow.colortex.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ro.bjjhwx.cn

[N07] 两数之和（返回下标）
来源：http://uo.yuexingan06.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wb.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iz.hahajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ht.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://do.panjiajie.cn

Java: // 手写 HashMap
来源：http://ck.szsharing.cn

Go:   // 手写 map[int]int
来源：http://uz.9csxet.cn

Ruby: // 手写 Hash
来源：http://du.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gs.lnxyls.cn

[N08] 生成全排列
来源：http://ru.shxzskj.cn

Py:   itertools.permutations(arr)
来源：http://fc.hnjuh.cn

PHP:  // 手写递归交换
来源：http://iy.jianghongdianzi.cn

JS:   // 手写回溯递归
来源：http://qy.colortex.cn

TS:   // 手写回溯递归
来源：http://ww.lnxyls.cn

Java: // 手写回溯递归
来源：http://jc.bookmarksfly.cn

Go:   // 手写回溯递归
来源：http://ll.chemitech.net.cn

Ruby: arr.permutation.to_a
来源：http://hv.asd995.cn

C#:   // 手写回溯递归
来源：http://zb.shxzukj.cn

[N09] 栈与队列
来源：http://jn.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ql.panjiajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pk.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sg.muxihuayi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bf.nicolike.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kj.haigaiapp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://og.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jh.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gh.panjiajie.cn

[N10] 链表节点定义
来源：http://jf.jctech888.com.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hr.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ez.wgjwhj.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fz.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kf.nicolike.cn

Java: class Node { int v; Node next; }
来源：http://qe.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ta.newstarts.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tu.jctech888.com.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://yg.muxihuayi.cn

[N11] 二叉树中序遍历
来源：http://ms.jctech888.com.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cn.huixinmuqiang.cn

PHP:  // 手写递归函数
来源：http://ey.huixinmuqiang.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ui.bookmarksfly.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sp.panjiajie.cn

Java: // 手写递归
来源：http://nm.panjiajie.cn

Go:   // 手写递归
来源：http://kq.bookmarksfly.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dl.nszjky.cn

C#:   // 手写递归
来源：http://bg.bjjhwx.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vg.shxzukj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gl.nszjky.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cs.lnxyls.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bq.bjjhwx.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hx.nicolike.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pk.hnjuh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://to.9csxet.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sy.gzmigu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pb.huanxung.cn

================================================================================
来源：http://fp.shxzukj.cn

O. 并发与异步
来源：http://ie.newstarts.cn

================================================================================
来源：http://om.szxytkj.cn

[O01] 启动一个线程
来源：http://pg.bookmarksfly.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://de.muxihuayi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fn.nicolike.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://es.muxihuayi.cn

TS:   // 同 JS
来源：http://ix.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://wj.hnjuh.cn

Go:   go f()
来源：http://vi.panjiajie.cn

Ruby: Thread.new { f }
来源：http://uy.hnjuh.cn

C#:   Task.Run(() => F());
来源：http://dv.huixinmuqiang.cn

[O02] 使用线程池
来源：http://cn.shxzukj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ny.huixiangedu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mq.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://uq.wgjwhj.cn

TS:   // worker_threads 线程池
来源：http://xn.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://cx.shxzukj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ap.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sa.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yl.shtwfgs.cn

[O03] 加锁保护共享数据
来源：http://ay.asd995.cn

Py:   with lock: shared += 1
来源：http://mr.jianghongdianzi.cn

PHP:  // 用 flock() 做文件锁
来源：http://bj.nszjky.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rk.asd995.cn

TS:   // 同 JS
来源：http://pa.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://yi.szsharing.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jy.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mj.shtwfgs.cn

C#:   lock (gate) { shared++; }
来源：http://wy.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://kq.521024.cn

Py:   async def f():⏎    await g()
来源：http://hy.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fz.jctech888.com.cn

JS:   async function f() { await g(); }
来源：http://ky.jctech888.com.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qi.nszjky.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wq.9csxet.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bp.gzmigu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://pg.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://ya.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://tc.nszjky.cn

Py:   asyncio.gather(*tasks)
来源：http://ya.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ej.huixiangedu.cn

JS:   await Promise.all(tasks)
来源：http://fj.9csxet.cn

TS:   await Promise.all(tasks)
来源：http://rs.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://on.shxzskj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qk.szsharing.cn

Ruby: threads.map(&:join)
来源：http://bt.colortex.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vu.yuexingan06.cn

[O06] 使用进程池
来源：http://qg.shxzukj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://oo.szxytkj.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://la.wgjwhj.cn

JS:   // child_process / cluster 模块
来源：http://uw.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://wu.bookmarksfly.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://et.szxytkj.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ta.newstarts.cn

Ruby: // fork 块
来源：http://mt.szxytkj.cn

C#:   Parallel.For
来源：http://wb.shxzskj.cn

================================================================================
来源：http://cg.9csxet.cn

P. 常用工具函数
来源：http://hn.haigaiapp.cn

================================================================================
来源：http://io.colortex.cn

[P01] 生成 UUID
来源：http://sz.colortex.cn

Py:   str(uuid.uuid4())
来源：http://ng.huixinmuqiang.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ud.9csxet.cn

JS:   crypto.randomUUID()
来源：http://gh.gzmigu.cn

TS:   crypto.randomUUID()
来源：http://os.521024.cn

Java: UUID.randomUUID().toString()
来源：http://jf.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://ou.newstarts.cn

Ruby: SecureRandom.uuid
来源：http://hv.yuexingan06.cn

C#:   Guid.NewGuid().ToString()
来源：http://aa.yuntaijiaju.cn

[P02] MD5 / SHA256 摘要
来源：http://po.chemitech.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fl.newstarts.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xy.lnxyls.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ku.521024.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ld.colortex.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vt.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gk.muxihuayi.cn


<!-- 参考信息 -->