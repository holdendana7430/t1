代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://iq.jianghongdianzi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zh.521024.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lt.haigaiapp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pi.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ko.huixiangedu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oe.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rw.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://vi.yuntaijiaju.cn

Py:   resp.json()
来源：http://qy.szsharing.cn

PHP:  json_decode($body, true);
来源：http://jy.haigaiapp.cn

JS:   await resp.json()
来源：http://jc.shtwfgs.cn

TS:   await resp.json()
来源：http://cb.panjiajie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zv.wgjwhj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vw.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://nm.lnxyls.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ei.hnjuh.cn

[L07] 处理 HTTP 状态码
来源：http://tx.hnjuh.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xy.521024.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://td.szxytkj.cn

JS:   resp.ok;  resp.status
来源：http://da.colortex.cn

TS:   resp.ok;  resp.status
来源：http://co.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://yw.szxytkj.cn

Go:   resp.StatusCode
来源：http://hh.asd995.cn

Ruby: resp.code.to_i
来源：http://ys.haigaiapp.cn

C#:   (int)resp.StatusCode
来源：http://sv.hahajie.cn

[L08] 并发请求多个地址
来源：http://it.521024.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ka.jianghongdianzi.cn

PHP:  curl_multi_init() 系列
来源：http://fy.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wa.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yh.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pb.9csxet.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ww.wgjwhj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ke.jianghongdianzi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jk.huanxung.cn

================================================================================
来源：http://lb.yuntaijiaju.cn

M. 命令行 / 进程 / 环境
来源：http://zg.szxytkj.cn

================================================================================
来源：http://sy.colortex.cn

[M01] 读取命令行参数
来源：http://mi.9csxet.cn

Py:   sys.argv[1:]
来源：http://bb.nicolike.cn

PHP:  $argv;  $argc;
来源：http://te.lnxyls.cn

JS:   process.argv.slice(2)
来源：http://xq.asd995.cn

TS:   process.argv.slice(2)
来源：http://ng.huanxung.cn

Java: args 数组（main 方法参数）
来源：http://de.haigaiapp.cn

Go:   os.Args[1:]
来源：http://ix.panjiajie.cn

Ruby: ARGV
来源：http://rp.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://uw.muxihuayi.cn

[M02] 读取环境变量
来源：http://cz.asd995.cn

Py:   os.environ.get("HOME")
来源：http://pw.yuntaijiaju.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zp.nszjky.cn

JS:   process.env.HOME
来源：http://qj.chemitech.net.cn

TS:   process.env.HOME
来源：http://od.panjiajie.cn

Java: System.getenv("HOME")
来源：http://bw.szsharing.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iu.lnxyls.cn

Ruby: ENV["HOME"]
来源：http://oy.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hm.muxihuayi.cn

[M03] 执行外部命令
来源：http://ir.huixinmuqiang.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ax.huixiangedu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://en.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dt.521024.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://fr.bookmarksfly.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qo.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://yt.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wx.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://mp.chemitech.net.cn

[M04] 获取当前工作目录
来源：http://qt.shxzskj.cn

Py:   os.getcwd()
来源：http://cy.shxzukj.cn

PHP:  getcwd();
来源：http://fc.nszjky.cn

JS:   process.cwd()
来源：http://zx.521024.cn

TS:   process.cwd()
来源：http://qz.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://vl.shxzskj.cn

Go:   os.Getwd()
来源：http://ke.lnxyls.cn

Ruby: Dir.pwd
来源：http://cw.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://op.colortex.cn

[M05] 设置退出码
来源：http://pp.yuntaijiaju.cn

Py:   sys.exit(1)
来源：http://da.yuntaijiaju.cn

PHP:  exit(1);
来源：http://kv.shtwfgs.cn

JS:   process.exit(1)
来源：http://ks.jianghongdianzi.cn

TS:   process.exit(1)
来源：http://pc.huixiangedu.cn

Java: System.exit(1)
来源：http://sv.yuntaijiaju.cn

Go:   os.Exit(1)
来源：http://ya.jctech888.com.cn

Ruby: exit 1
来源：http://oo.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wv.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://hh.jianghongdianzi.cn

Py:   print("err", file=sys.stderr)
来源：http://ih.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dx.bjjhwx.cn

JS:   console.error("err")
来源：http://gv.hahajie.cn

TS:   console.error("err")
来源：http://xa.huanxung.cn

Java: System.err.println("err")
来源：http://fr.bookmarksfly.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bf.newstarts.cn

Ruby: warn "err"
来源：http://od.shtwfgs.cn

C#:   Console.Error.WriteLine("err")
来源：http://dg.jianghongdianzi.cn

[M07] 判断是否为主入口
来源：http://rq.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://py.yuexingan06.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jt.szsharing.cn

JS:   require.main === module
来源：http://sn.shtwfgs.cn

TS:   require.main === module
来源：http://js.colortex.cn

Java: public static void main(String[] args)
来源：http://gg.bjjhwx.cn

Go:   func main()
来源：http://vu.521024.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ez.szsharing.cn

C#:   static void Main(string[] args)
来源：http://we.huixinmuqiang.cn

[M08] 获取系统与运行时信息
来源：http://nx.szxytkj.cn

Py:   platform.system();  platform.python_version()
来源：http://lt.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://rz.szxytkj.cn

JS:   process.platform;  process.version
来源：http://lh.jianghongdianzi.cn

TS:   process.platform;  process.version
来源：http://da.szxytkj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mc.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fv.haigaiapp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://so.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://oh.szxytkj.cn

================================================================================
来源：http://sh.lnxyls.cn

N. 数据结构与算法
来源：http://rm.bjjhwx.cn

================================================================================
来源：http://lh.szxytkj.cn

[N01] 二分查找（有序数组）
来源：http://it.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nq.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ro.hnjuh.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qq.nicolike.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wl.haigaiapp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wj.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://py.panjiajie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wi.hnjuh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ow.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://dl.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://ez.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ib.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://oq.yuexingan06.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sy.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pz.nicolike.cn

Go:   slices.Sort(arr)
来源：http://ko.huixinmuqiang.cn

Ruby: arr.sort
来源：http://vt.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hq.szxytkj.cn

[N03] 快速排序（分治示例）
来源：http://hz.haigaiapp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mu.9csxet.cn

PHP:  // 递归实现，或用 usort
来源：http://ph.9csxet.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mt.lnxyls.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qa.521024.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zb.521024.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pi.jianghongdianzi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bw.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ls.gzmigu.cn

[N04] 斐波那契数列
来源：http://qa.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kx.jctech888.com.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jq.yuexingan06.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gd.colortex.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bb.haigaiapp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uf.9csxet.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ir.shxzukj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sq.shtwfgs.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://do.yuexingan06.cn

[N05] 最大公约数
来源：http://hg.hahajie.cn

Py:   math.gcd(a, b)
来源：http://nb.shxzukj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ng.colortex.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nj.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tm.chemitech.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fv.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mm.wgjwhj.cn

Ruby: a.gcd(b)
来源：http://wy.newstarts.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ry.wgjwhj.cn

[N06] 判断回文字符串
来源：http://ar.huixinmuqiang.cn

Py:   s == s[::-1]
来源：http://um.9csxet.cn

PHP:  $s === strrev($s);
来源：http://ko.gzmigu.cn

JS:   s === [...s].reverse().join("")
来源：http://ud.szxytkj.cn

TS:   s === [...s].reverse().join("")
来源：http://ab.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uh.huixiangedu.cn

Go:   // 双指针从两端比较
来源：http://ct.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://kl.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tj.521024.cn

[N07] 两数之和（返回下标）
来源：http://kz.newstarts.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zl.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iu.huixinmuqiang.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://do.huixiangedu.cn

TS:   // 手写 Map<string, number>
来源：http://nm.panjiajie.cn

Java: // 手写 HashMap
来源：http://zb.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://dc.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://oa.panjiajie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://hs.colortex.cn

[N08] 生成全排列
来源：http://mg.nicolike.cn

Py:   itertools.permutations(arr)
来源：http://js.szsharing.cn

PHP:  // 手写递归交换
来源：http://to.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://tq.hahajie.cn

TS:   // 手写回溯递归
来源：http://mp.nszjky.cn

Java: // 手写回溯递归
来源：http://zt.haigaiapp.cn

Go:   // 手写回溯递归
来源：http://vd.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://yr.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://ri.yuexingan06.cn

[N09] 栈与队列
来源：http://nc.wgjwhj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://po.bjjhwx.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ip.hahajie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://md.gzmigu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fq.bookmarksfly.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sb.newstarts.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bm.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mk.yuntaijiaju.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://en.bjjhwx.cn

[N10] 链表节点定义
来源：http://hz.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uz.haigaiapp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vt.bookmarksfly.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iz.panjiajie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yv.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://iv.bookmarksfly.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mq.9csxet.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ao.shtwfgs.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ip.9csxet.cn

[N11] 二叉树中序遍历
来源：http://nt.yuexingan06.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://em.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://gf.muxihuayi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ib.haigaiapp.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vx.nicolike.cn

Java: // 手写递归
来源：http://kh.huanxung.cn

Go:   // 手写递归
来源：http://da.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nf.huixiangedu.cn

C#:   // 手写递归
来源：http://ye.asd995.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nr.jctech888.com.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://di.bookmarksfly.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oh.yuexingan06.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fr.521024.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nk.shxzukj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pj.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ah.shxzukj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rw.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nw.huixinmuqiang.cn

================================================================================
来源：http://dt.bookmarksfly.cn

O. 并发与异步
来源：http://gg.huixiangedu.cn

================================================================================
来源：http://kq.jctech888.com.cn

[O01] 启动一个线程
来源：http://pm.colortex.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ya.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://te.bookmarksfly.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sc.newstarts.cn

TS:   // 同 JS
来源：http://th.muxihuayi.cn

Java: new Thread(() -> f()).start()
来源：http://tp.haigaiapp.cn

Go:   go f()
来源：http://sc.hahajie.cn

Ruby: Thread.new { f }
来源：http://sk.jctech888.com.cn

C#:   Task.Run(() => F());
来源：http://vd.yuntaijiaju.cn

[O02] 使用线程池
来源：http://db.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pl.lnxyls.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tj.szsharing.cn

JS:   // worker_threads 线程池
来源：http://fg.shtwfgs.cn

TS:   // worker_threads 线程池
来源：http://mj.huixinmuqiang.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jg.9csxet.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nu.shxzskj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vq.yuntaijiaju.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cg.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://hf.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://jt.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://jl.gzmigu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cm.nicolike.cn

TS:   // 同 JS
来源：http://zk.newstarts.cn

Java: synchronized (this) { shared++; }
来源：http://xa.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ou.shtwfgs.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bm.nszjky.cn

C#:   lock (gate) { shared++; }
来源：http://ce.nicolike.cn

[O04] 定义异步函数并等待
来源：http://yj.haigaiapp.cn

Py:   async def f():⏎    await g()
来源：http://lb.nszjky.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jb.asd995.cn

JS:   async function f() { await g(); }
来源：http://nz.huixiangedu.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ho.panjiajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pl.chemitech.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eo.jianghongdianzi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yh.9csxet.cn

C#:   async Task F() { await G(); }
来源：http://zd.bookmarksfly.cn

[O05] 并发执行并等待全部完成
来源：http://yb.9csxet.cn

Py:   asyncio.gather(*tasks)
来源：http://kd.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://su.huanxung.cn

JS:   await Promise.all(tasks)
来源：http://tv.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://hd.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xg.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vo.yuntaijiaju.cn

Ruby: threads.map(&:join)
来源：http://an.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gj.hahajie.cn

[O06] 使用进程池
来源：http://oo.asd995.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wq.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bs.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://ul.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://wc.haigaiapp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sy.haigaiapp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kg.newstarts.cn

Ruby: // fork 块
来源：http://fm.shxzskj.cn

C#:   Parallel.For
来源：http://ay.newstarts.cn

================================================================================
来源：http://ed.jianghongdianzi.cn

P. 常用工具函数
来源：http://qz.haigaiapp.cn

================================================================================
来源：http://nc.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://uy.bjjhwx.cn

Py:   str(uuid.uuid4())
来源：http://on.jctech888.com.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lu.nszjky.cn

JS:   crypto.randomUUID()
来源：http://ep.bookmarksfly.cn

TS:   crypto.randomUUID()
来源：http://ns.jianghongdianzi.cn

Java: UUID.randomUUID().toString()
来源：http://rg.yuntaijiaju.cn

Go:   // 用 github.com/google/uuid
来源：http://rb.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://rc.shxzskj.cn

C#:   Guid.NewGuid().ToString()
来源：http://go.shtwfgs.cn

[P02] MD5 / SHA256 摘要
来源：http://hf.shxzskj.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yn.huanxung.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jk.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sh.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lm.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://we.lnxyls.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vc.huixinmuqiang.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ij.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pe.bjjhwx.cn

[P03] 生成短随机字符串
来源：http://ey.szsharing.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ay.shxzukj.cn


<!-- 参考信息 -->