代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vf.haigaiapp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sd.panjiajie.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hs.wgjwhj.cn

[L06] 解析响应为 JSON
来源：http://df.shtwfgs.cn

Py:   resp.json()
来源：http://fr.521024.cn

PHP:  json_decode($body, true);
来源：http://sz.szxytkj.cn

JS:   await resp.json()
来源：http://re.szsharing.cn

TS:   await resp.json()
来源：http://qs.bookmarksfly.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://na.shtwfgs.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uq.gzmigu.cn

Ruby: JSON.parse(resp.body)
来源：http://ox.huanxung.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tc.521024.cn

[L07] 处理 HTTP 状态码
来源：http://pi.yuntaijiaju.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vd.szsharing.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ft.haigaiapp.cn

JS:   resp.ok;  resp.status
来源：http://tv.9csxet.cn

TS:   resp.ok;  resp.status
来源：http://mz.lnxyls.cn

Java: resp.statusCode()
来源：http://tf.yuexingan06.cn

Go:   resp.StatusCode
来源：http://al.huixinmuqiang.cn

Ruby: resp.code.to_i
来源：http://sf.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://gb.huixinmuqiang.cn

[L08] 并发请求多个地址
来源：http://cm.huanxung.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ym.bjjhwx.cn

PHP:  curl_multi_init() 系列
来源：http://tl.bjjhwx.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://my.yuexingan06.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iw.shxzskj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dg.gzmigu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pr.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nf.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hh.szsharing.cn

================================================================================
来源：http://kz.szxytkj.cn

M. 命令行 / 进程 / 环境
来源：http://jq.yuexingan06.cn

================================================================================
来源：http://up.jctech888.com.cn

[M01] 读取命令行参数
来源：http://xj.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://dz.szxytkj.cn

PHP:  $argv;  $argc;
来源：http://df.9csxet.cn

JS:   process.argv.slice(2)
来源：http://ao.lnxyls.cn

TS:   process.argv.slice(2)
来源：http://kr.jctech888.com.cn

Java: args 数组（main 方法参数）
来源：http://zz.muxihuayi.cn

Go:   os.Args[1:]
来源：http://qj.asd995.cn

Ruby: ARGV
来源：http://tp.521024.cn

C#:   args 数组（Main 方法参数）
来源：http://fr.yuntaijiaju.cn

[M02] 读取环境变量
来源：http://ly.panjiajie.cn

Py:   os.environ.get("HOME")
来源：http://bg.muxihuayi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pm.panjiajie.cn

JS:   process.env.HOME
来源：http://ju.shtwfgs.cn

TS:   process.env.HOME
来源：http://bv.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://vz.huixinmuqiang.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://am.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://zx.hnjuh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sb.szsharing.cn

[M03] 执行外部命令
来源：http://zp.shxzukj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://od.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mj.huixiangedu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sp.gzmigu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xh.lnxyls.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sk.hahajie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qm.bjjhwx.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ik.panjiajie.cn

C#:   Process.Start("ls", "-l");
来源：http://cs.panjiajie.cn

[M04] 获取当前工作目录
来源：http://vy.chemitech.net.cn

Py:   os.getcwd()
来源：http://ee.haigaiapp.cn

PHP:  getcwd();
来源：http://we.yuntaijiaju.cn

JS:   process.cwd()
来源：http://hr.colortex.cn

TS:   process.cwd()
来源：http://ao.shxzukj.cn

Java: Path.of("").toAbsolutePath()
来源：http://ug.9csxet.cn

Go:   os.Getwd()
来源：http://er.gzmigu.cn

Ruby: Dir.pwd
来源：http://gx.lnxyls.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sx.shxzskj.cn

[M05] 设置退出码
来源：http://vw.colortex.cn

Py:   sys.exit(1)
来源：http://pw.huixinmuqiang.cn

PHP:  exit(1);
来源：http://eq.shxzskj.cn

JS:   process.exit(1)
来源：http://ww.gzmigu.cn

TS:   process.exit(1)
来源：http://xo.bookmarksfly.cn

Java: System.exit(1)
来源：http://ru.9csxet.cn

Go:   os.Exit(1)
来源：http://pw.szsharing.cn

Ruby: exit 1
来源：http://rw.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ut.gzmigu.cn

[M06] 向标准错误输出
来源：http://cd.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://fv.shxzukj.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rn.lnxyls.cn

JS:   console.error("err")
来源：http://rv.nicolike.cn

TS:   console.error("err")
来源：http://il.haigaiapp.cn

Java: System.err.println("err")
来源：http://og.jianghongdianzi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ud.jctech888.com.cn

Ruby: warn "err"
来源：http://yx.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://hq.nicolike.cn

[M07] 判断是否为主入口
来源：http://rt.9csxet.cn

Py:   if __name__ == "__main__":
来源：http://om.shxzskj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fp.jctech888.com.cn

JS:   require.main === module
来源：http://ko.szsharing.cn

TS:   require.main === module
来源：http://dw.yuntaijiaju.cn

Java: public static void main(String[] args)
来源：http://ky.shtwfgs.cn

Go:   func main()
来源：http://ay.hahajie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ln.asd995.cn

C#:   static void Main(string[] args)
来源：http://gv.shtwfgs.cn

[M08] 获取系统与运行时信息
来源：http://gb.shxzskj.cn

Py:   platform.system();  platform.python_version()
来源：http://mx.bjjhwx.cn

PHP:  PHP_OS;  phpversion();
来源：http://kg.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ii.shxzukj.cn

TS:   process.platform;  process.version
来源：http://mz.nicolike.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mk.shxzukj.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vi.lnxyls.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sh.muxihuayi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wd.shxzskj.cn

================================================================================
来源：http://nf.nszjky.cn

N. 数据结构与算法
来源：http://uj.shtwfgs.cn

================================================================================
来源：http://xt.gzmigu.cn

[N01] 二分查找（有序数组）
来源：http://ge.shxzukj.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mx.jianghongdianzi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dh.hahajie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ho.muxihuayi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pa.bjjhwx.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ci.chemitech.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://ga.chemitech.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://md.shxzukj.cn

C#:   Array.BinarySearch(arr, x)
来源：http://we.haigaiapp.cn

[N02] 排序（工程实践用内置实现）
来源：http://pa.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://pn.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ee.haigaiapp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bj.wgjwhj.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yo.panjiajie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jq.jianghongdianzi.cn

Go:   slices.Sort(arr)
来源：http://aw.colortex.cn

Ruby: arr.sort
来源：http://cp.newstarts.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ie.hahajie.cn

[N03] 快速排序（分治示例）
来源：http://np.newstarts.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cd.jctech888.com.cn

PHP:  // 递归实现，或用 usort
来源：http://te.nicolike.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cl.szxytkj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ls.hnjuh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yo.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cg.lnxyls.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yp.lnxyls.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sm.521024.cn

[N04] 斐波那契数列
来源：http://mv.colortex.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bx.nicolike.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zz.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ky.shxzukj.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wq.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fw.yuntaijiaju.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ka.szxytkj.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://by.panjiajie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kq.hahajie.cn

[N05] 最大公约数
来源：http://iz.521024.cn

Py:   math.gcd(a, b)
来源：http://wu.haigaiapp.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://is.chemitech.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://be.haigaiapp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nn.huixiangedu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ne.9csxet.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rm.bjjhwx.cn

Ruby: a.gcd(b)
来源：http://xb.bjjhwx.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vj.lnxyls.cn

[N06] 判断回文字符串
来源：http://yl.shxzskj.cn

Py:   s == s[::-1]
来源：http://oi.szsharing.cn

PHP:  $s === strrev($s);
来源：http://gf.szsharing.cn

JS:   s === [...s].reverse().join("")
来源：http://aq.huanxung.cn

TS:   s === [...s].reverse().join("")
来源：http://ai.muxihuayi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ge.yuntaijiaju.cn

Go:   // 双指针从两端比较
来源：http://ff.huixiangedu.cn

Ruby: s == s.reverse
来源：http://ew.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://al.shxzukj.cn

[N07] 两数之和（返回下标）
来源：http://nu.yuntaijiaju.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hn.yuexingan06.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kw.panjiajie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ni.gzmigu.cn

TS:   // 手写 Map<string, number>
来源：http://nu.hahajie.cn

Java: // 手写 HashMap
来源：http://fp.shtwfgs.cn

Go:   // 手写 map[int]int
来源：http://xi.bookmarksfly.cn

Ruby: // 手写 Hash
来源：http://nr.huixinmuqiang.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ct.shtwfgs.cn

[N08] 生成全排列
来源：http://lj.bjjhwx.cn

Py:   itertools.permutations(arr)
来源：http://dn.wgjwhj.cn

PHP:  // 手写递归交换
来源：http://wv.yuexingan06.cn

JS:   // 手写回溯递归
来源：http://ww.gzmigu.cn

TS:   // 手写回溯递归
来源：http://ms.521024.cn

Java: // 手写回溯递归
来源：http://am.bjjhwx.cn

Go:   // 手写回溯递归
来源：http://hi.huixinmuqiang.cn

Ruby: arr.permutation.to_a
来源：http://tn.szsharing.cn

C#:   // 手写回溯递归
来源：http://gp.nszjky.cn

[N09] 栈与队列
来源：http://cm.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://za.shxzukj.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yz.bookmarksfly.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gs.9csxet.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zn.521024.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mh.huanxung.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mk.huixinmuqiang.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ph.huanxung.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gv.9csxet.cn

[N10] 链表节点定义
来源：http://qd.szxytkj.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nb.colortex.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bj.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qr.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://on.panjiajie.cn

Java: class Node { int v; Node next; }
来源：http://ee.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cs.nicolike.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xt.yuntaijiaju.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zb.nszjky.cn

[N11] 二叉树中序遍历
来源：http://gy.chemitech.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tn.9csxet.cn

PHP:  // 手写递归函数
来源：http://vc.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wm.huixiangedu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ab.shtwfgs.cn

Java: // 手写递归
来源：http://ey.panjiajie.cn

Go:   // 手写递归
来源：http://ct.9csxet.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zk.lnxyls.cn

C#:   // 手写递归
来源：http://jh.szxytkj.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tq.newstarts.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ur.huixinmuqiang.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://am.wgjwhj.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wp.shxzskj.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fm.9csxet.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bp.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rz.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wb.shxzukj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mc.chemitech.net.cn

================================================================================
来源：http://za.hnjuh.cn

O. 并发与异步
来源：http://yh.huanxung.cn

================================================================================
来源：http://go.nszjky.cn

[O01] 启动一个线程
来源：http://pc.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://od.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lu.szsharing.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hy.9csxet.cn

TS:   // 同 JS
来源：http://bj.9csxet.cn

Java: new Thread(() -> f()).start()
来源：http://ai.asd995.cn

Go:   go f()
来源：http://yi.nszjky.cn

Ruby: Thread.new { f }
来源：http://xt.huanxung.cn

C#:   Task.Run(() => F());
来源：http://tu.asd995.cn

[O02] 使用线程池
来源：http://mi.asd995.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rj.szxytkj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vs.haigaiapp.cn

JS:   // worker_threads 线程池
来源：http://mq.jctech888.com.cn

TS:   // worker_threads 线程池
来源：http://tv.szsharing.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dt.muxihuayi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cr.panjiajie.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qy.gzmigu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wd.shxzskj.cn

[O03] 加锁保护共享数据
来源：http://pk.asd995.cn

Py:   with lock: shared += 1
来源：http://gu.shxzukj.cn

PHP:  // 用 flock() 做文件锁
来源：http://rc.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ey.jianghongdianzi.cn

TS:   // 同 JS
来源：http://tg.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://eo.nicolike.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ch.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ol.chemitech.net.cn

C#:   lock (gate) { shared++; }
来源：http://eb.hnjuh.cn

[O04] 定义异步函数并等待
来源：http://en.asd995.cn

Py:   async def f():⏎    await g()
来源：http://hz.muxihuayi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xf.huanxung.cn

JS:   async function f() { await g(); }
来源：http://ij.9csxet.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://py.bjjhwx.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ij.haigaiapp.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xk.bookmarksfly.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rz.bookmarksfly.cn

C#:   async Task F() { await G(); }
来源：http://xf.9csxet.cn

[O05] 并发执行并等待全部完成
来源：http://bt.gzmigu.cn

Py:   asyncio.gather(*tasks)
来源：http://ga.shxzukj.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tj.shxzskj.cn

JS:   await Promise.all(tasks)
来源：http://qq.haigaiapp.cn

TS:   await Promise.all(tasks)
来源：http://mz.nszjky.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jv.bjjhwx.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ld.nicolike.cn

Ruby: threads.map(&:join)
来源：http://yh.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cz.9csxet.cn

[O06] 使用进程池
来源：http://lj.szxytkj.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://be.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xg.muxihuayi.cn

JS:   // child_process / cluster 模块
来源：http://gv.nszjky.cn

TS:   // child_process / cluster 模块
来源：http://ea.muxihuayi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://au.shtwfgs.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://al.bookmarksfly.cn

Ruby: // fork 块
来源：http://rz.szsharing.cn

C#:   Parallel.For
来源：http://fi.bookmarksfly.cn

================================================================================
来源：http://ty.hnjuh.cn

P. 常用工具函数
来源：http://ya.yuexingan06.cn

================================================================================
来源：http://gz.szxytkj.cn

[P01] 生成 UUID
来源：http://lh.shtwfgs.cn

Py:   str(uuid.uuid4())
来源：http://nr.yuntaijiaju.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gz.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://pw.chemitech.net.cn

TS:   crypto.randomUUID()
来源：http://eb.shtwfgs.cn

Java: UUID.randomUUID().toString()
来源：http://pc.jctech888.com.cn

Go:   // 用 github.com/google/uuid
来源：http://cc.nicolike.cn

Ruby: SecureRandom.uuid
来源：http://yw.jianghongdianzi.cn

C#:   Guid.NewGuid().ToString()
来源：http://dl.hnjuh.cn

[P02] MD5 / SHA256 摘要
来源：http://lh.huanxung.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gk.huixinmuqiang.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kg.jianghongdianzi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yk.bookmarksfly.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vx.yuntaijiaju.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ip.muxihuayi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mu.521024.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jk.szsharing.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hc.hahajie.cn

[P03] 生成短随机字符串
来源：http://wk.521024.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zq.szxytkj.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yi.haigaiapp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rp.wgjwhj.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ff.hahajie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gb.szxytkj.cn


<!-- 参考信息 -->