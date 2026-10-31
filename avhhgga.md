代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yj.jctech888.com.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xe.shtwfgs.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eh.shxzukj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ep.hahajie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lb.521024.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bc.colortex.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ih.huixiangedu.cn

[L06] 解析响应为 JSON
来源：http://ku.szxytkj.cn

Py:   resp.json()
来源：http://ic.9csxet.cn

PHP:  json_decode($body, true);
来源：http://nu.muxihuayi.cn

JS:   await resp.json()
来源：http://fl.bookmarksfly.cn

TS:   await resp.json()
来源：http://mb.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sn.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://id.shtwfgs.cn

Ruby: JSON.parse(resp.body)
来源：http://jp.bookmarksfly.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rw.panjiajie.cn

[L07] 处理 HTTP 状态码
来源：http://vs.nicolike.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ni.9csxet.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ek.yuntaijiaju.cn

JS:   resp.ok;  resp.status
来源：http://er.colortex.cn

TS:   resp.ok;  resp.status
来源：http://fk.jianghongdianzi.cn

Java: resp.statusCode()
来源：http://hr.huanxung.cn

Go:   resp.StatusCode
来源：http://jo.nszjky.cn

Ruby: resp.code.to_i
来源：http://zx.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://fa.haigaiapp.cn

[L08] 并发请求多个地址
来源：http://wh.nicolike.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fd.yuntaijiaju.cn

PHP:  curl_multi_init() 系列
来源：http://vm.muxihuayi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://my.colortex.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lg.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tu.huixinmuqiang.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ji.huixinmuqiang.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jg.bookmarksfly.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zh.gzmigu.cn

================================================================================
来源：http://dk.szsharing.cn

M. 命令行 / 进程 / 环境
来源：http://cq.szxytkj.cn

================================================================================
来源：http://xg.szxytkj.cn

[M01] 读取命令行参数
来源：http://ad.huanxung.cn

Py:   sys.argv[1:]
来源：http://hz.9csxet.cn

PHP:  $argv;  $argc;
来源：http://uw.nszjky.cn

JS:   process.argv.slice(2)
来源：http://yz.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://xi.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://gd.chemitech.net.cn

Go:   os.Args[1:]
来源：http://ru.521024.cn

Ruby: ARGV
来源：http://uf.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://na.lnxyls.cn

[M02] 读取环境变量
来源：http://os.huanxung.cn

Py:   os.environ.get("HOME")
来源：http://tw.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rn.nicolike.cn

JS:   process.env.HOME
来源：http://hr.shxzukj.cn

TS:   process.env.HOME
来源：http://qa.huixinmuqiang.cn

Java: System.getenv("HOME")
来源：http://gs.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://on.wgjwhj.cn

Ruby: ENV["HOME"]
来源：http://fx.wgjwhj.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fb.shtwfgs.cn

[M03] 执行外部命令
来源：http://gk.colortex.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rp.bjjhwx.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://po.bjjhwx.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://tc.asd995.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ot.jctech888.com.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xs.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bu.521024.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ud.nszjky.cn

C#:   Process.Start("ls", "-l");
来源：http://xx.huixiangedu.cn

[M04] 获取当前工作目录
来源：http://hf.szsharing.cn

Py:   os.getcwd()
来源：http://cq.bjjhwx.cn

PHP:  getcwd();
来源：http://hh.bookmarksfly.cn

JS:   process.cwd()
来源：http://fe.bjjhwx.cn

TS:   process.cwd()
来源：http://hm.huanxung.cn

Java: Path.of("").toAbsolutePath()
来源：http://ab.huixiangedu.cn

Go:   os.Getwd()
来源：http://az.lnxyls.cn

Ruby: Dir.pwd
来源：http://wn.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://im.chemitech.net.cn

[M05] 设置退出码
来源：http://kr.521024.cn

Py:   sys.exit(1)
来源：http://vv.hahajie.cn

PHP:  exit(1);
来源：http://fy.gzmigu.cn

JS:   process.exit(1)
来源：http://dc.nicolike.cn

TS:   process.exit(1)
来源：http://ds.bjjhwx.cn

Java: System.exit(1)
来源：http://rp.szsharing.cn

Go:   os.Exit(1)
来源：http://gn.jianghongdianzi.cn

Ruby: exit 1
来源：http://kv.muxihuayi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xy.muxihuayi.cn

[M06] 向标准错误输出
来源：http://nf.huixinmuqiang.cn

Py:   print("err", file=sys.stderr)
来源：http://zz.yuntaijiaju.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tn.lnxyls.cn

JS:   console.error("err")
来源：http://qc.muxihuayi.cn

TS:   console.error("err")
来源：http://dg.nszjky.cn

Java: System.err.println("err")
来源：http://qe.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dz.shxzukj.cn

Ruby: warn "err"
来源：http://vu.shxzukj.cn

C#:   Console.Error.WriteLine("err")
来源：http://wy.hahajie.cn

[M07] 判断是否为主入口
来源：http://kn.asd995.cn

Py:   if __name__ == "__main__":
来源：http://ka.hnjuh.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hs.hahajie.cn

JS:   require.main === module
来源：http://ko.lnxyls.cn

TS:   require.main === module
来源：http://zo.shxzukj.cn

Java: public static void main(String[] args)
来源：http://gi.yuexingan06.cn

Go:   func main()
来源：http://nb.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fe.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://xn.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://xp.jianghongdianzi.cn

Py:   platform.system();  platform.python_version()
来源：http://rr.hahajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://ca.bjjhwx.cn

JS:   process.platform;  process.version
来源：http://bs.chemitech.net.cn

TS:   process.platform;  process.version
来源：http://nk.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oa.hnjuh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xd.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dg.nicolike.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xd.asd995.cn

================================================================================
来源：http://ou.szsharing.cn

N. 数据结构与算法
来源：http://nk.panjiajie.cn

================================================================================
来源：http://fy.521024.cn

[N01] 二分查找（有序数组）
来源：http://uh.nicolike.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ir.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gt.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gk.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://il.chemitech.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ww.hnjuh.cn

Go:   sort.SearchInts(arr, x)
来源：http://tz.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pz.gzmigu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hi.shxzukj.cn

[N02] 排序（工程实践用内置实现）
来源：http://vx.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://ag.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ho.shtwfgs.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aa.asd995.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zn.jianghongdianzi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ug.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://xf.huanxung.cn

Ruby: arr.sort
来源：http://hd.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hf.szsharing.cn

[N03] 快速排序（分治示例）
来源：http://dl.hahajie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uh.shtwfgs.cn

PHP:  // 递归实现，或用 usort
来源：http://vn.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yz.jctech888.com.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tu.asd995.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kj.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://re.521024.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zi.shxzukj.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iy.haigaiapp.cn

[N04] 斐波那契数列
来源：http://rz.muxihuayi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dy.bookmarksfly.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ss.nszjky.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hi.panjiajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eb.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qb.asd995.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gt.chemitech.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lu.yuexingan06.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gm.haigaiapp.cn

[N05] 最大公约数
来源：http://al.huixinmuqiang.cn

Py:   math.gcd(a, b)
来源：http://ps.hnjuh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bn.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xo.nicolike.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kq.newstarts.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ys.colortex.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zd.szsharing.cn

Ruby: a.gcd(b)
来源：http://sq.asd995.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://my.bookmarksfly.cn

[N06] 判断回文字符串
来源：http://kj.asd995.cn

Py:   s == s[::-1]
来源：http://fj.yuntaijiaju.cn

PHP:  $s === strrev($s);
来源：http://ms.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://xm.panjiajie.cn

TS:   s === [...s].reverse().join("")
来源：http://hr.shxzukj.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bi.shtwfgs.cn

Go:   // 双指针从两端比较
来源：http://mb.shtwfgs.cn

Ruby: s == s.reverse
来源：http://tj.shxzskj.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://va.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://fz.nicolike.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hw.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ta.muxihuayi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yr.shtwfgs.cn

TS:   // 手写 Map<string, number>
来源：http://yh.gzmigu.cn

Java: // 手写 HashMap
来源：http://mw.newstarts.cn

Go:   // 手写 map[int]int
来源：http://vi.shxzskj.cn

Ruby: // 手写 Hash
来源：http://zi.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nb.nicolike.cn

[N08] 生成全排列
来源：http://xs.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://lq.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://kq.521024.cn

JS:   // 手写回溯递归
来源：http://hl.shxzukj.cn

TS:   // 手写回溯递归
来源：http://jp.bjjhwx.cn

Java: // 手写回溯递归
来源：http://vx.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://cq.wgjwhj.cn

Ruby: arr.permutation.to_a
来源：http://hn.huixiangedu.cn

C#:   // 手写回溯递归
来源：http://vf.colortex.cn

[N09] 栈与队列
来源：http://up.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ur.chemitech.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ft.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yi.yuexingan06.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sw.wgjwhj.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dg.szxytkj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ht.shtwfgs.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nt.szxytkj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oc.bjjhwx.cn

[N10] 链表节点定义
来源：http://yp.lnxyls.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nt.shtwfgs.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lz.yuntaijiaju.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vx.nicolike.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://db.nszjky.cn

Java: class Node { int v; Node next; }
来源：http://lb.haigaiapp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mk.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ca.szsharing.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dk.yuntaijiaju.cn

[N11] 二叉树中序遍历
来源：http://mh.gzmigu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pt.yuntaijiaju.cn

PHP:  // 手写递归函数
来源：http://ii.szxytkj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jt.hahajie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ym.huanxung.cn

Java: // 手写递归
来源：http://kv.huixinmuqiang.cn

Go:   // 手写递归
来源：http://rh.huixinmuqiang.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kn.szxytkj.cn

C#:   // 手写递归
来源：http://ra.szsharing.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cu.9csxet.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wc.colortex.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fe.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tx.shtwfgs.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lv.bjjhwx.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iw.bookmarksfly.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://no.szxytkj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fd.hnjuh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://te.lnxyls.cn

================================================================================
来源：http://sq.shtwfgs.cn

O. 并发与异步
来源：http://tc.jianghongdianzi.cn

================================================================================
来源：http://sq.asd995.cn

[O01] 启动一个线程
来源：http://fh.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lb.huixiangedu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zt.chemitech.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://go.shtwfgs.cn

TS:   // 同 JS
来源：http://ro.chemitech.net.cn

Java: new Thread(() -> f()).start()
来源：http://pl.newstarts.cn

Go:   go f()
来源：http://qq.chemitech.net.cn

Ruby: Thread.new { f }
来源：http://wn.jianghongdianzi.cn

C#:   Task.Run(() => F());
来源：http://ty.chemitech.net.cn

[O02] 使用线程池
来源：http://sz.521024.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fn.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://su.jctech888.com.cn

JS:   // worker_threads 线程池
来源：http://wg.nicolike.cn

TS:   // worker_threads 线程池
来源：http://pb.colortex.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ft.bjjhwx.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ny.huixiangedu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qo.jianghongdianzi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xc.bookmarksfly.cn

[O03] 加锁保护共享数据
来源：http://av.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://qa.huanxung.cn

PHP:  // 用 flock() 做文件锁
来源：http://nc.colortex.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dn.panjiajie.cn

TS:   // 同 JS
来源：http://mv.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://ll.colortex.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dt.wgjwhj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yt.colortex.cn

C#:   lock (gate) { shared++; }
来源：http://im.huixiangedu.cn

[O04] 定义异步函数并等待
来源：http://qn.chemitech.net.cn

Py:   async def f():⏎    await g()
来源：http://po.huanxung.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hx.hahajie.cn

JS:   async function f() { await g(); }
来源：http://lu.chemitech.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qq.hnjuh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mz.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wd.nicolike.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wv.shxzskj.cn

C#:   async Task F() { await G(); }
来源：http://ab.muxihuayi.cn

[O05] 并发执行并等待全部完成
来源：http://bf.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://yd.gzmigu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qe.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://su.jctech888.com.cn

TS:   await Promise.all(tasks)
来源：http://mp.gzmigu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ud.jctech888.com.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bv.muxihuayi.cn

Ruby: threads.map(&:join)
来源：http://dc.shxzukj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ek.wgjwhj.cn

[O06] 使用进程池
来源：http://da.yuntaijiaju.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yi.nszjky.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yw.panjiajie.cn

JS:   // child_process / cluster 模块
来源：http://ba.bookmarksfly.cn

TS:   // child_process / cluster 模块
来源：http://hr.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ig.9csxet.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vn.huixiangedu.cn

Ruby: // fork 块
来源：http://yp.nicolike.cn

C#:   Parallel.For
来源：http://py.shxzskj.cn

================================================================================
来源：http://tn.9csxet.cn

P. 常用工具函数
来源：http://zq.shxzukj.cn

================================================================================
来源：http://th.yuntaijiaju.cn

[P01] 生成 UUID
来源：http://ki.huixiangedu.cn

Py:   str(uuid.uuid4())
来源：http://sj.szsharing.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zm.yuntaijiaju.cn

JS:   crypto.randomUUID()
来源：http://my.newstarts.cn

TS:   crypto.randomUUID()
来源：http://ij.huixiangedu.cn

Java: UUID.randomUUID().toString()
来源：http://ti.bookmarksfly.cn

Go:   // 用 github.com/google/uuid
来源：http://yn.asd995.cn

Ruby: SecureRandom.uuid
来源：http://do.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://cc.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://sz.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kq.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sa.shxzskj.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sy.muxihuayi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iv.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vc.asd995.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://to.panjiajie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qz.jianghongdianzi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://it.lnxyls.cn

[P03] 生成短随机字符串
来源：http://wn.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xm.asd995.cn


<!-- 参考信息 -->