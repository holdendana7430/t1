代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lv.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fr.huixinmuqiang.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://af.wgjwhj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ck.newstarts.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://st.nicolike.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://np.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jg.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://jq.hnjuh.cn

Py:   resp.json()
来源：http://ye.lnxyls.cn

PHP:  json_decode($body, true);
来源：http://mm.shtwfgs.cn

JS:   await resp.json()
来源：http://ne.szsharing.cn

TS:   await resp.json()
来源：http://qc.gzmigu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zf.nicolike.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://om.lnxyls.cn

Ruby: JSON.parse(resp.body)
来源：http://mh.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ab.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://ds.lnxyls.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lb.bjjhwx.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tq.hahajie.cn

JS:   resp.ok;  resp.status
来源：http://bc.asd995.cn

TS:   resp.ok;  resp.status
来源：http://nt.nicolike.cn

Java: resp.statusCode()
来源：http://wo.haigaiapp.cn

Go:   resp.StatusCode
来源：http://fx.muxihuayi.cn

Ruby: resp.code.to_i
来源：http://mi.hnjuh.cn

C#:   (int)resp.StatusCode
来源：http://zn.nicolike.cn

[L08] 并发请求多个地址
来源：http://an.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://it.huixinmuqiang.cn

PHP:  curl_multi_init() 系列
来源：http://hp.hnjuh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gy.shtwfgs.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lh.521024.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hr.szxytkj.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ub.hnjuh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tm.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zp.shtwfgs.cn

================================================================================
来源：http://ms.9csxet.cn

M. 命令行 / 进程 / 环境
来源：http://wo.hnjuh.cn

================================================================================
来源：http://vb.newstarts.cn

[M01] 读取命令行参数
来源：http://yy.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://un.shxzskj.cn

PHP:  $argv;  $argc;
来源：http://um.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://ob.hnjuh.cn

TS:   process.argv.slice(2)
来源：http://tb.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://mm.asd995.cn

Go:   os.Args[1:]
来源：http://is.bjjhwx.cn

Ruby: ARGV
来源：http://um.haigaiapp.cn

C#:   args 数组（Main 方法参数）
来源：http://lk.nicolike.cn

[M02] 读取环境变量
来源：http://gu.hnjuh.cn

Py:   os.environ.get("HOME")
来源：http://yk.huanxung.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://if.bjjhwx.cn

JS:   process.env.HOME
来源：http://nl.hahajie.cn

TS:   process.env.HOME
来源：http://om.huanxung.cn

Java: System.getenv("HOME")
来源：http://iu.yuexingan06.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nh.yuntaijiaju.cn

Ruby: ENV["HOME"]
来源：http://vq.521024.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zz.nicolike.cn

[M03] 执行外部命令
来源：http://kt.huanxung.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xq.bookmarksfly.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iv.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fj.hnjuh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wx.newstarts.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ut.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dd.szxytkj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://jo.yuexingan06.cn

C#:   Process.Start("ls", "-l");
来源：http://zd.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://qy.newstarts.cn

Py:   os.getcwd()
来源：http://zn.gzmigu.cn

PHP:  getcwd();
来源：http://wy.szsharing.cn

JS:   process.cwd()
来源：http://fn.haigaiapp.cn

TS:   process.cwd()
来源：http://yw.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://kl.jianghongdianzi.cn

Go:   os.Getwd()
来源：http://ad.nszjky.cn

Ruby: Dir.pwd
来源：http://cq.nszjky.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zw.521024.cn

[M05] 设置退出码
来源：http://pk.huixinmuqiang.cn

Py:   sys.exit(1)
来源：http://px.szsharing.cn

PHP:  exit(1);
来源：http://zq.shtwfgs.cn

JS:   process.exit(1)
来源：http://ac.panjiajie.cn

TS:   process.exit(1)
来源：http://zp.muxihuayi.cn

Java: System.exit(1)
来源：http://sd.nszjky.cn

Go:   os.Exit(1)
来源：http://qk.newstarts.cn

Ruby: exit 1
来源：http://rr.lnxyls.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ed.nszjky.cn

[M06] 向标准错误输出
来源：http://sv.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://bs.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kc.jianghongdianzi.cn

JS:   console.error("err")
来源：http://ct.huixiangedu.cn

TS:   console.error("err")
来源：http://cs.gzmigu.cn

Java: System.err.println("err")
来源：http://yk.haigaiapp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zp.bookmarksfly.cn

Ruby: warn "err"
来源：http://sb.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://dy.shxzukj.cn

[M07] 判断是否为主入口
来源：http://zz.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://ex.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lq.panjiajie.cn

JS:   require.main === module
来源：http://th.shxzukj.cn

TS:   require.main === module
来源：http://hb.szsharing.cn

Java: public static void main(String[] args)
来源：http://bp.521024.cn

Go:   func main()
来源：http://si.bjjhwx.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sa.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://qe.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://em.asd995.cn

Py:   platform.system();  platform.python_version()
来源：http://km.szsharing.cn

PHP:  PHP_OS;  phpversion();
来源：http://tr.newstarts.cn

JS:   process.platform;  process.version
来源：http://ys.newstarts.cn

TS:   process.platform;  process.version
来源：http://ux.shxzukj.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tn.panjiajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://eo.shtwfgs.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kx.yuntaijiaju.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ml.jianghongdianzi.cn

================================================================================
来源：http://tw.yuntaijiaju.cn

N. 数据结构与算法
来源：http://cc.huanxung.cn

================================================================================
来源：http://cz.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://qj.shxzskj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nj.yuntaijiaju.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hv.nszjky.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kn.nszjky.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tx.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xb.huixiangedu.cn

Go:   sort.SearchInts(arr, x)
来源：http://zd.521024.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://mg.wgjwhj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sh.bookmarksfly.cn

[N02] 排序（工程实践用内置实现）
来源：http://ic.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ec.huixiangedu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yw.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vz.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ov.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qd.colortex.cn

Go:   slices.Sort(arr)
来源：http://kv.muxihuayi.cn

Ruby: arr.sort
来源：http://rj.huixiangedu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fp.hnjuh.cn

[N03] 快速排序（分治示例）
来源：http://sq.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pt.lnxyls.cn

PHP:  // 递归实现，或用 usort
来源：http://uh.jianghongdianzi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tw.shtwfgs.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jw.muxihuayi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qf.asd995.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ad.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gj.jctech888.com.cn

C#:   // 手写递归，或 Array.Sort
来源：http://we.shxzukj.cn

[N04] 斐波那契数列
来源：http://ml.shxzukj.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jz.huixiangedu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lk.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dp.hahajie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uz.hahajie.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lo.yuexingan06.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bz.521024.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tg.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wb.szsharing.cn

[N05] 最大公约数
来源：http://lz.hahajie.cn

Py:   math.gcd(a, b)
来源：http://ql.shtwfgs.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://na.huixiangedu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ym.colortex.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jk.521024.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mj.nicolike.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kx.szsharing.cn

Ruby: a.gcd(b)
来源：http://ej.jctech888.com.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://la.gzmigu.cn

[N06] 判断回文字符串
来源：http://iv.huanxung.cn

Py:   s == s[::-1]
来源：http://jh.panjiajie.cn

PHP:  $s === strrev($s);
来源：http://nk.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://kv.haigaiapp.cn

TS:   s === [...s].reverse().join("")
来源：http://yb.chemitech.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fa.9csxet.cn

Go:   // 双指针从两端比较
来源：http://mg.shxzskj.cn

Ruby: s == s.reverse
来源：http://gk.yuntaijiaju.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xw.asd995.cn

[N07] 两数之和（返回下标）
来源：http://ex.shxzukj.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nl.nszjky.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ny.jianghongdianzi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dx.yuexingan06.cn

TS:   // 手写 Map<string, number>
来源：http://dq.szxytkj.cn

Java: // 手写 HashMap
来源：http://nu.nicolike.cn

Go:   // 手写 map[int]int
来源：http://su.9csxet.cn

Ruby: // 手写 Hash
来源：http://xb.chemitech.net.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ee.colortex.cn

[N08] 生成全排列
来源：http://xy.hnjuh.cn

Py:   itertools.permutations(arr)
来源：http://lq.yuntaijiaju.cn

PHP:  // 手写递归交换
来源：http://ch.shtwfgs.cn

JS:   // 手写回溯递归
来源：http://nb.bjjhwx.cn

TS:   // 手写回溯递归
来源：http://pq.panjiajie.cn

Java: // 手写回溯递归
来源：http://fo.chemitech.net.cn

Go:   // 手写回溯递归
来源：http://sb.gzmigu.cn

Ruby: arr.permutation.to_a
来源：http://zk.yuntaijiaju.cn

C#:   // 手写回溯递归
来源：http://ji.chemitech.net.cn

[N09] 栈与队列
来源：http://mb.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nn.hahajie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.nicolike.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://og.hnjuh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vh.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://oo.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ay.hnjuh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sv.shtwfgs.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uj.shxzukj.cn

[N10] 链表节点定义
来源：http://qr.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zv.chemitech.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zb.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hx.gzmigu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ki.yuntaijiaju.cn

Java: class Node { int v; Node next; }
来源：http://or.huixiangedu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vk.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dd.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qr.chemitech.net.cn

[N11] 二叉树中序遍历
来源：http://kt.nszjky.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qd.muxihuayi.cn

PHP:  // 手写递归函数
来源：http://ih.lnxyls.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gf.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rb.szsharing.cn

Java: // 手写递归
来源：http://jf.jianghongdianzi.cn

Go:   // 手写递归
来源：http://yo.asd995.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://me.szxytkj.cn

C#:   // 手写递归
来源：http://nr.hahajie.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vu.asd995.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://se.asd995.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lk.nszjky.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://od.colortex.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jp.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hm.colortex.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nn.muxihuayi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rd.521024.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bz.chemitech.net.cn

================================================================================
来源：http://qm.shtwfgs.cn

O. 并发与异步
来源：http://lq.yuntaijiaju.cn

================================================================================
来源：http://da.huixiangedu.cn

[O01] 启动一个线程
来源：http://bb.nicolike.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://li.wgjwhj.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pt.nszjky.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fu.huanxung.cn

TS:   // 同 JS
来源：http://tp.shxzskj.cn

Java: new Thread(() -> f()).start()
来源：http://lz.huixinmuqiang.cn

Go:   go f()
来源：http://ta.colortex.cn

Ruby: Thread.new { f }
来源：http://og.bjjhwx.cn

C#:   Task.Run(() => F());
来源：http://lq.nicolike.cn

[O02] 使用线程池
来源：http://ug.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zq.hnjuh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ts.huixiangedu.cn

JS:   // worker_threads 线程池
来源：http://cc.chemitech.net.cn

TS:   // worker_threads 线程池
来源：http://yu.gzmigu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ud.jianghongdianzi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ms.nicolike.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ir.9csxet.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://db.lnxyls.cn

[O03] 加锁保护共享数据
来源：http://ly.yuntaijiaju.cn

Py:   with lock: shared += 1
来源：http://xa.shtwfgs.cn

PHP:  // 用 flock() 做文件锁
来源：http://ib.newstarts.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cg.asd995.cn

TS:   // 同 JS
来源：http://sd.panjiajie.cn

Java: synchronized (this) { shared++; }
来源：http://bc.521024.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ru.szxytkj.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ze.haigaiapp.cn

C#:   lock (gate) { shared++; }
来源：http://tk.colortex.cn

[O04] 定义异步函数并等待
来源：http://mz.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://zl.nicolike.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sy.chemitech.net.cn

JS:   async function f() { await g(); }
来源：http://ch.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fy.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wo.shtwfgs.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ua.yuntaijiaju.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jv.jianghongdianzi.cn

C#:   async Task F() { await G(); }
来源：http://aj.bjjhwx.cn

[O05] 并发执行并等待全部完成
来源：http://qx.nicolike.cn

Py:   asyncio.gather(*tasks)
来源：http://wt.bookmarksfly.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iu.hnjuh.cn

JS:   await Promise.all(tasks)
来源：http://cx.shxzukj.cn

TS:   await Promise.all(tasks)
来源：http://ul.haigaiapp.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qq.panjiajie.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ek.haigaiapp.cn

Ruby: threads.map(&:join)
来源：http://br.bjjhwx.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://on.newstarts.cn

[O06] 使用进程池
来源：http://uy.jianghongdianzi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nk.bjjhwx.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nb.szsharing.cn

JS:   // child_process / cluster 模块
来源：http://bx.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://yw.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xp.521024.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oz.lnxyls.cn

Ruby: // fork 块
来源：http://yr.jctech888.com.cn

C#:   Parallel.For
来源：http://dy.nszjky.cn

================================================================================
来源：http://ul.hahajie.cn

P. 常用工具函数
来源：http://zl.shxzskj.cn

================================================================================
来源：http://gk.521024.cn

[P01] 生成 UUID
来源：http://jz.521024.cn

Py:   str(uuid.uuid4())
来源：http://st.hnjuh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rc.gzmigu.cn

JS:   crypto.randomUUID()
来源：http://ay.nszjky.cn

TS:   crypto.randomUUID()
来源：http://ht.bjjhwx.cn

Java: UUID.randomUUID().toString()
来源：http://mv.szsharing.cn

Go:   // 用 github.com/google/uuid
来源：http://uc.szxytkj.cn

Ruby: SecureRandom.uuid
来源：http://hl.huixinmuqiang.cn

C#:   Guid.NewGuid().ToString()
来源：http://cj.haigaiapp.cn

[P02] MD5 / SHA256 摘要
来源：http://cz.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tb.shtwfgs.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tu.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hx.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lg.gzmigu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://od.jianghongdianzi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ok.shtwfgs.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ym.huixinmuqiang.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pi.nicolike.cn

[P03] 生成短随机字符串
来源：http://rh.9csxet.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lo.colortex.cn


<!-- 参考信息 -->