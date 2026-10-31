代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jv.shxzukj.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nv.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vi.yuntaijiaju.cn

[L06] 解析响应为 JSON
来源：http://ws.huanxung.cn

Py:   resp.json()
来源：http://fq.jianghongdianzi.cn

PHP:  json_decode($body, true);
来源：http://yg.muxihuayi.cn

JS:   await resp.json()
来源：http://sc.szxytkj.cn

TS:   await resp.json()
来源：http://ez.haigaiapp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nl.huixinmuqiang.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qn.bookmarksfly.cn

Ruby: JSON.parse(resp.body)
来源：http://pp.nicolike.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://te.shxzskj.cn

[L07] 处理 HTTP 状态码
来源：http://qx.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vi.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rr.lnxyls.cn

JS:   resp.ok;  resp.status
来源：http://dz.nszjky.cn

TS:   resp.ok;  resp.status
来源：http://de.haigaiapp.cn

Java: resp.statusCode()
来源：http://fv.chemitech.net.cn

Go:   resp.StatusCode
来源：http://li.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://ec.huixinmuqiang.cn

C#:   (int)resp.StatusCode
来源：http://wo.asd995.cn

[L08] 并发请求多个地址
来源：http://rf.jianghongdianzi.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xq.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://mk.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nq.bjjhwx.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bj.huixiangedu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jm.nszjky.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nj.bjjhwx.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vr.jctech888.com.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cc.szxytkj.cn

================================================================================
来源：http://kp.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://ip.chemitech.net.cn

================================================================================
来源：http://cj.shtwfgs.cn

[M01] 读取命令行参数
来源：http://nt.bjjhwx.cn

Py:   sys.argv[1:]
来源：http://op.bjjhwx.cn

PHP:  $argv;  $argc;
来源：http://lo.haigaiapp.cn

JS:   process.argv.slice(2)
来源：http://dn.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://rf.nszjky.cn

Java: args 数组（main 方法参数）
来源：http://qk.lnxyls.cn

Go:   os.Args[1:]
来源：http://lu.haigaiapp.cn

Ruby: ARGV
来源：http://mi.szxytkj.cn

C#:   args 数组（Main 方法参数）
来源：http://lp.shxzukj.cn

[M02] 读取环境变量
来源：http://jq.lnxyls.cn

Py:   os.environ.get("HOME")
来源：http://ge.panjiajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://os.asd995.cn

JS:   process.env.HOME
来源：http://yb.bookmarksfly.cn

TS:   process.env.HOME
来源：http://jz.yuexingan06.cn

Java: System.getenv("HOME")
来源：http://kv.szxytkj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hh.asd995.cn

Ruby: ENV["HOME"]
来源：http://df.chemitech.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mb.jianghongdianzi.cn

[M03] 执行外部命令
来源：http://cd.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ro.chemitech.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://uk.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://wg.jianghongdianzi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rw.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oz.huixiangedu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uj.huanxung.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ox.newstarts.cn

C#:   Process.Start("ls", "-l");
来源：http://yr.521024.cn

[M04] 获取当前工作目录
来源：http://fq.szsharing.cn

Py:   os.getcwd()
来源：http://be.nszjky.cn

PHP:  getcwd();
来源：http://sf.huixiangedu.cn

JS:   process.cwd()
来源：http://of.gzmigu.cn

TS:   process.cwd()
来源：http://ic.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://se.nszjky.cn

Go:   os.Getwd()
来源：http://yv.yuexingan06.cn

Ruby: Dir.pwd
来源：http://mg.szsharing.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qh.521024.cn

[M05] 设置退出码
来源：http://vy.lnxyls.cn

Py:   sys.exit(1)
来源：http://md.shtwfgs.cn

PHP:  exit(1);
来源：http://gt.hahajie.cn

JS:   process.exit(1)
来源：http://lk.shxzskj.cn

TS:   process.exit(1)
来源：http://sa.newstarts.cn

Java: System.exit(1)
来源：http://qs.shxzukj.cn

Go:   os.Exit(1)
来源：http://rd.shxzukj.cn

Ruby: exit 1
来源：http://an.panjiajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sz.521024.cn

[M06] 向标准错误输出
来源：http://yv.shtwfgs.cn

Py:   print("err", file=sys.stderr)
来源：http://ti.lnxyls.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yu.huixiangedu.cn

JS:   console.error("err")
来源：http://ex.lnxyls.cn

TS:   console.error("err")
来源：http://fk.colortex.cn

Java: System.err.println("err")
来源：http://kh.nszjky.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vg.panjiajie.cn

Ruby: warn "err"
来源：http://fd.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://mj.hahajie.cn

[M07] 判断是否为主入口
来源：http://iu.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://mp.bjjhwx.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tt.wgjwhj.cn

JS:   require.main === module
来源：http://vf.shxzskj.cn

TS:   require.main === module
来源：http://es.panjiajie.cn

Java: public static void main(String[] args)
来源：http://hl.bjjhwx.cn

Go:   func main()
来源：http://ou.jctech888.com.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eu.nszjky.cn

C#:   static void Main(string[] args)
来源：http://ur.jianghongdianzi.cn

[M08] 获取系统与运行时信息
来源：http://jd.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://fu.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://ml.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://nu.hahajie.cn

TS:   process.platform;  process.version
来源：http://uk.shtwfgs.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oh.bjjhwx.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ed.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cn.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://md.jianghongdianzi.cn

================================================================================
来源：http://vt.hahajie.cn

N. 数据结构与算法
来源：http://zl.newstarts.cn

================================================================================
来源：http://sw.asd995.cn

[N01] 二分查找（有序数组）
来源：http://mh.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ti.521024.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wf.shxzskj.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cx.bookmarksfly.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qs.nszjky.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lt.jianghongdianzi.cn

Go:   sort.SearchInts(arr, x)
来源：http://tj.jctech888.com.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hs.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aq.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://to.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://rw.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hi.gzmigu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gn.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ej.muxihuayi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zt.panjiajie.cn

Go:   slices.Sort(arr)
来源：http://lb.yuntaijiaju.cn

Ruby: arr.sort
来源：http://me.hnjuh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kq.newstarts.cn

[N03] 快速排序（分治示例）
来源：http://hw.shtwfgs.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ts.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://wm.huixiangedu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pc.bjjhwx.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ki.haigaiapp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sn.huixinmuqiang.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fy.shxzukj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yj.chemitech.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://oj.shtwfgs.cn

[N04] 斐波那契数列
来源：http://nf.huanxung.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nf.jianghongdianzi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rb.haigaiapp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jo.9csxet.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oo.huixiangedu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qz.hnjuh.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bb.shxzskj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://id.szsharing.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hp.yuexingan06.cn

[N05] 最大公约数
来源：http://ux.szsharing.cn

Py:   math.gcd(a, b)
来源：http://cj.bjjhwx.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rp.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hi.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mi.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gt.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gf.521024.cn

Ruby: a.gcd(b)
来源：http://pg.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aq.shxzskj.cn

[N06] 判断回文字符串
来源：http://zp.9csxet.cn

Py:   s == s[::-1]
来源：http://ui.jctech888.com.cn

PHP:  $s === strrev($s);
来源：http://su.nszjky.cn

JS:   s === [...s].reverse().join("")
来源：http://rm.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://bb.521024.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qd.muxihuayi.cn

Go:   // 双指针从两端比较
来源：http://qm.hahajie.cn

Ruby: s == s.reverse
来源：http://fp.huixiangedu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xy.chemitech.net.cn

[N07] 两数之和（返回下标）
来源：http://eg.huixinmuqiang.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hb.hahajie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ki.huixiangedu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ft.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://im.lnxyls.cn

Java: // 手写 HashMap
来源：http://fc.huixiangedu.cn

Go:   // 手写 map[int]int
来源：http://kq.huanxung.cn

Ruby: // 手写 Hash
来源：http://zd.haigaiapp.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mw.asd995.cn

[N08] 生成全排列
来源：http://yi.asd995.cn

Py:   itertools.permutations(arr)
来源：http://rc.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://kp.yuntaijiaju.cn

JS:   // 手写回溯递归
来源：http://mn.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://ec.chemitech.net.cn

Java: // 手写回溯递归
来源：http://lw.huixiangedu.cn

Go:   // 手写回溯递归
来源：http://xe.shxzukj.cn

Ruby: arr.permutation.to_a
来源：http://rx.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://wi.shxzukj.cn

[N09] 栈与队列
来源：http://kf.bjjhwx.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ov.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ae.lnxyls.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nm.panjiajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oo.nszjky.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jq.wgjwhj.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dk.asd995.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vx.shxzukj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nr.szsharing.cn

[N10] 链表节点定义
来源：http://jz.haigaiapp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yc.9csxet.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qq.hnjuh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dd.wgjwhj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ig.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://sq.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bf.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mk.huixiangedu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nl.huanxung.cn

[N11] 二叉树中序遍历
来源：http://ef.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qp.huixiangedu.cn

PHP:  // 手写递归函数
来源：http://ur.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wi.gzmigu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://od.muxihuayi.cn

Java: // 手写递归
来源：http://wd.panjiajie.cn

Go:   // 手写递归
来源：http://jc.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oy.jctech888.com.cn

C#:   // 手写递归
来源：http://is.newstarts.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mj.hnjuh.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://os.yuexingan06.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dl.chemitech.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yu.huixiangedu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sb.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bb.panjiajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ji.haigaiapp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://td.jianghongdianzi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zv.panjiajie.cn

================================================================================
来源：http://fj.gzmigu.cn

O. 并发与异步
来源：http://yt.9csxet.cn

================================================================================
来源：http://nf.yuntaijiaju.cn

[O01] 启动一个线程
来源：http://uq.gzmigu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ef.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hl.yuntaijiaju.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://th.yuexingan06.cn

TS:   // 同 JS
来源：http://ul.szsharing.cn

Java: new Thread(() -> f()).start()
来源：http://bk.shxzukj.cn

Go:   go f()
来源：http://gc.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://xq.521024.cn

C#:   Task.Run(() => F());
来源：http://ef.hahajie.cn

[O02] 使用线程池
来源：http://re.chemitech.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jm.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ye.muxihuayi.cn

JS:   // worker_threads 线程池
来源：http://lb.newstarts.cn

TS:   // worker_threads 线程池
来源：http://dp.shtwfgs.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zb.521024.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ov.asd995.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://um.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zc.yuexingan06.cn

[O03] 加锁保护共享数据
来源：http://qf.gzmigu.cn

Py:   with lock: shared += 1
来源：http://pi.newstarts.cn

PHP:  // 用 flock() 做文件锁
来源：http://jl.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ed.huanxung.cn

TS:   // 同 JS
来源：http://sz.yuexingan06.cn

Java: synchronized (this) { shared++; }
来源：http://pf.yuntaijiaju.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mc.haigaiapp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lq.wgjwhj.cn

C#:   lock (gate) { shared++; }
来源：http://jb.chemitech.net.cn

[O04] 定义异步函数并等待
来源：http://af.gzmigu.cn

Py:   async def f():⏎    await g()
来源：http://bp.wgjwhj.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://du.yuexingan06.cn

JS:   async function f() { await g(); }
来源：http://yc.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ue.chemitech.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ge.jianghongdianzi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tv.hahajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://aj.szsharing.cn

C#:   async Task F() { await G(); }
来源：http://fr.yuexingan06.cn

[O05] 并发执行并等待全部完成
来源：http://ud.colortex.cn

Py:   asyncio.gather(*tasks)
来源：http://nl.szxytkj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dt.panjiajie.cn

JS:   await Promise.all(tasks)
来源：http://pq.gzmigu.cn

TS:   await Promise.all(tasks)
来源：http://gh.szxytkj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uo.shxzukj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://na.panjiajie.cn

Ruby: threads.map(&:join)
来源：http://ju.521024.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mt.haigaiapp.cn

[O06] 使用进程池
来源：http://up.gzmigu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kf.lnxyls.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ul.gzmigu.cn

JS:   // child_process / cluster 模块
来源：http://eh.9csxet.cn

TS:   // child_process / cluster 模块
来源：http://ed.huixiangedu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gk.hahajie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lg.panjiajie.cn

Ruby: // fork 块
来源：http://zy.shxzukj.cn

C#:   Parallel.For
来源：http://ta.521024.cn

================================================================================
来源：http://zz.521024.cn

P. 常用工具函数
来源：http://zs.huixinmuqiang.cn

================================================================================
来源：http://ae.huixinmuqiang.cn

[P01] 生成 UUID
来源：http://rx.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://qq.521024.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://li.haigaiapp.cn

JS:   crypto.randomUUID()
来源：http://oo.hnjuh.cn

TS:   crypto.randomUUID()
来源：http://gv.asd995.cn

Java: UUID.randomUUID().toString()
来源：http://ei.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://st.shxzskj.cn

Ruby: SecureRandom.uuid
来源：http://bd.huanxung.cn

C#:   Guid.NewGuid().ToString()
来源：http://mc.asd995.cn

[P02] MD5 / SHA256 摘要
来源：http://nh.nicolike.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wr.yuntaijiaju.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://at.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ax.nicolike.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yj.szsharing.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ne.szsharing.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eu.szxytkj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://os.bjjhwx.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ga.asd995.cn

[P03] 生成短随机字符串
来源：http://un.gzmigu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wh.yuntaijiaju.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kw.huixiangedu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oh.yuntaijiaju.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pg.jianghongdianzi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lv.bjjhwx.cn


<!-- 参考信息 -->