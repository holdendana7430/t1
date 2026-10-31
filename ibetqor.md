代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cm.lnxyls.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gr.panjiajie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hb.huanxung.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nx.szsharing.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wb.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://po.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fn.panjiajie.cn

[L06] 解析响应为 JSON
来源：http://ri.huanxung.cn

Py:   resp.json()
来源：http://gm.haigaiapp.cn

PHP:  json_decode($body, true);
来源：http://fb.bookmarksfly.cn

JS:   await resp.json()
来源：http://ep.shxzukj.cn

TS:   await resp.json()
来源：http://ix.jctech888.com.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iv.nszjky.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lw.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://km.wgjwhj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qn.521024.cn

[L07] 处理 HTTP 状态码
来源：http://wm.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mn.hahajie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vn.asd995.cn

JS:   resp.ok;  resp.status
来源：http://dl.huixiangedu.cn

TS:   resp.ok;  resp.status
来源：http://mu.szxytkj.cn

Java: resp.statusCode()
来源：http://ar.bookmarksfly.cn

Go:   resp.StatusCode
来源：http://eg.wgjwhj.cn

Ruby: resp.code.to_i
来源：http://qx.nszjky.cn

C#:   (int)resp.StatusCode
来源：http://ow.nicolike.cn

[L08] 并发请求多个地址
来源：http://sg.haigaiapp.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rl.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://qa.nszjky.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rp.nicolike.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qk.lnxyls.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dq.huanxung.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fn.szxytkj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vj.muxihuayi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iq.chemitech.net.cn

================================================================================
来源：http://yw.gzmigu.cn

M. 命令行 / 进程 / 环境
来源：http://fz.bookmarksfly.cn

================================================================================
来源：http://yi.nicolike.cn

[M01] 读取命令行参数
来源：http://cj.521024.cn

Py:   sys.argv[1:]
来源：http://qr.gzmigu.cn

PHP:  $argv;  $argc;
来源：http://ym.hahajie.cn

JS:   process.argv.slice(2)
来源：http://rx.chemitech.net.cn

TS:   process.argv.slice(2)
来源：http://id.hnjuh.cn

Java: args 数组（main 方法参数）
来源：http://qj.shtwfgs.cn

Go:   os.Args[1:]
来源：http://ef.jctech888.com.cn

Ruby: ARGV
来源：http://vn.gzmigu.cn

C#:   args 数组（Main 方法参数）
来源：http://zb.hahajie.cn

[M02] 读取环境变量
来源：http://ud.newstarts.cn

Py:   os.environ.get("HOME")
来源：http://ml.nszjky.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rn.yuexingan06.cn

JS:   process.env.HOME
来源：http://eo.shtwfgs.cn

TS:   process.env.HOME
来源：http://ys.wgjwhj.cn

Java: System.getenv("HOME")
来源：http://sj.nszjky.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ho.muxihuayi.cn

Ruby: ENV["HOME"]
来源：http://cp.szsharing.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cr.nszjky.cn

[M03] 执行外部命令
来源：http://iw.nszjky.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ak.haigaiapp.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kq.chemitech.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sv.newstarts.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bz.gzmigu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pu.9csxet.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uv.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://th.colortex.cn

C#:   Process.Start("ls", "-l");
来源：http://no.lnxyls.cn

[M04] 获取当前工作目录
来源：http://an.wgjwhj.cn

Py:   os.getcwd()
来源：http://sm.panjiajie.cn

PHP:  getcwd();
来源：http://aq.panjiajie.cn

JS:   process.cwd()
来源：http://df.szxytkj.cn

TS:   process.cwd()
来源：http://fp.panjiajie.cn

Java: Path.of("").toAbsolutePath()
来源：http://cb.chemitech.net.cn

Go:   os.Getwd()
来源：http://tb.szxytkj.cn

Ruby: Dir.pwd
来源：http://dx.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://up.huanxung.cn

[M05] 设置退出码
来源：http://ok.shxzskj.cn

Py:   sys.exit(1)
来源：http://cb.jianghongdianzi.cn

PHP:  exit(1);
来源：http://hx.lnxyls.cn

JS:   process.exit(1)
来源：http://yk.hnjuh.cn

TS:   process.exit(1)
来源：http://ge.haigaiapp.cn

Java: System.exit(1)
来源：http://ou.shxzukj.cn

Go:   os.Exit(1)
来源：http://aa.gzmigu.cn

Ruby: exit 1
来源：http://jn.hahajie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pa.shtwfgs.cn

[M06] 向标准错误输出
来源：http://fs.shxzukj.cn

Py:   print("err", file=sys.stderr)
来源：http://ba.jctech888.com.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xu.yuntaijiaju.cn

JS:   console.error("err")
来源：http://vi.shxzukj.cn

TS:   console.error("err")
来源：http://as.asd995.cn

Java: System.err.println("err")
来源：http://kv.shxzukj.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wh.wgjwhj.cn

Ruby: warn "err"
来源：http://dr.521024.cn

C#:   Console.Error.WriteLine("err")
来源：http://bs.huixiangedu.cn

[M07] 判断是否为主入口
来源：http://uu.yuexingan06.cn

Py:   if __name__ == "__main__":
来源：http://uy.nicolike.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uy.jctech888.com.cn

JS:   require.main === module
来源：http://pn.jianghongdianzi.cn

TS:   require.main === module
来源：http://dz.colortex.cn

Java: public static void main(String[] args)
来源：http://ll.nicolike.cn

Go:   func main()
来源：http://ms.lnxyls.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sw.shxzskj.cn

C#:   static void Main(string[] args)
来源：http://rl.521024.cn

[M08] 获取系统与运行时信息
来源：http://vn.szsharing.cn

Py:   platform.system();  platform.python_version()
来源：http://xp.gzmigu.cn

PHP:  PHP_OS;  phpversion();
来源：http://dz.shxzukj.cn

JS:   process.platform;  process.version
来源：http://am.9csxet.cn

TS:   process.platform;  process.version
来源：http://bi.haigaiapp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zd.9csxet.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mc.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ng.gzmigu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://up.huixinmuqiang.cn

================================================================================
来源：http://ez.wgjwhj.cn

N. 数据结构与算法
来源：http://yk.szsharing.cn

================================================================================
来源：http://to.wgjwhj.cn

[N01] 二分查找（有序数组）
来源：http://ib.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ya.gzmigu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xk.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rk.szsharing.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ew.jianghongdianzi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zm.nszjky.cn

Go:   sort.SearchInts(arr, x)
来源：http://vp.shxzukj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pu.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yg.yuntaijiaju.cn

[N02] 排序（工程实践用内置实现）
来源：http://ib.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ek.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jm.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gc.nszjky.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cq.lnxyls.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rv.muxihuayi.cn

Go:   slices.Sort(arr)
来源：http://xy.muxihuayi.cn

Ruby: arr.sort
来源：http://ah.muxihuayi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://am.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://hr.yuexingan06.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lb.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://th.huixinmuqiang.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cr.yuexingan06.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eo.szsharing.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://st.szxytkj.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lk.szsharing.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ai.nicolike.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ft.muxihuayi.cn

[N04] 斐波那契数列
来源：http://lz.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hn.muxihuayi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ck.hnjuh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qk.yuntaijiaju.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://at.gzmigu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ie.szsharing.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wc.bjjhwx.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yz.gzmigu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bd.hnjuh.cn

[N05] 最大公约数
来源：http://xl.huanxung.cn

Py:   math.gcd(a, b)
来源：http://yv.chemitech.net.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cm.muxihuayi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zy.9csxet.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jp.gzmigu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qs.huixiangedu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wx.huixinmuqiang.cn

Ruby: a.gcd(b)
来源：http://yl.yuntaijiaju.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vh.nicolike.cn

[N06] 判断回文字符串
来源：http://dk.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://kp.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://vl.szxytkj.cn

JS:   s === [...s].reverse().join("")
来源：http://et.gzmigu.cn

TS:   s === [...s].reverse().join("")
来源：http://qo.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pr.shxzukj.cn

Go:   // 双指针从两端比较
来源：http://ac.szxytkj.cn

Ruby: s == s.reverse
来源：http://yq.huixinmuqiang.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sw.szsharing.cn

[N07] 两数之和（返回下标）
来源：http://yy.colortex.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ts.shxzukj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://de.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://al.szxytkj.cn

TS:   // 手写 Map<string, number>
来源：http://ow.panjiajie.cn

Java: // 手写 HashMap
来源：http://my.yuexingan06.cn

Go:   // 手写 map[int]int
来源：http://hr.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://fe.nicolike.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dg.hnjuh.cn

[N08] 生成全排列
来源：http://ho.szsharing.cn

Py:   itertools.permutations(arr)
来源：http://pw.shxzukj.cn

PHP:  // 手写递归交换
来源：http://pn.bjjhwx.cn

JS:   // 手写回溯递归
来源：http://oa.shxzskj.cn

TS:   // 手写回溯递归
来源：http://qq.newstarts.cn

Java: // 手写回溯递归
来源：http://di.nicolike.cn

Go:   // 手写回溯递归
来源：http://ug.521024.cn

Ruby: arr.permutation.to_a
来源：http://bc.shxzskj.cn

C#:   // 手写回溯递归
来源：http://mr.shxzskj.cn

[N09] 栈与队列
来源：http://ls.panjiajie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vo.bookmarksfly.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uc.szxytkj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wi.shxzskj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zr.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ep.chemitech.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ra.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://we.nszjky.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pt.colortex.cn

[N10] 链表节点定义
来源：http://hg.gzmigu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ak.huanxung.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xt.chemitech.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oe.shxzukj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jp.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://dy.asd995.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mf.szsharing.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xl.bookmarksfly.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ab.huixiangedu.cn

[N11] 二叉树中序遍历
来源：http://ey.huixinmuqiang.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mq.szxytkj.cn

PHP:  // 手写递归函数
来源：http://co.jctech888.com.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rt.colortex.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mq.shxzskj.cn

Java: // 手写递归
来源：http://ud.szxytkj.cn

Go:   // 手写递归
来源：http://mg.nicolike.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ov.shxzskj.cn

C#:   // 手写递归
来源：http://cv.muxihuayi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uq.lnxyls.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nn.jianghongdianzi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jz.yuntaijiaju.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lo.gzmigu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ua.gzmigu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rk.nicolike.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://di.nszjky.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ka.huanxung.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://er.gzmigu.cn

================================================================================
来源：http://gd.shxzukj.cn

O. 并发与异步
来源：http://xn.asd995.cn

================================================================================
来源：http://do.huixiangedu.cn

[O01] 启动一个线程
来源：http://vr.hahajie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ys.colortex.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rp.asd995.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sm.shxzskj.cn

TS:   // 同 JS
来源：http://da.panjiajie.cn

Java: new Thread(() -> f()).start()
来源：http://cc.newstarts.cn

Go:   go f()
来源：http://ep.jctech888.com.cn

Ruby: Thread.new { f }
来源：http://mv.hahajie.cn

C#:   Task.Run(() => F());
来源：http://ow.yuntaijiaju.cn

[O02] 使用线程池
来源：http://uw.hahajie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zd.asd995.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ki.bjjhwx.cn

JS:   // worker_threads 线程池
来源：http://df.9csxet.cn

TS:   // worker_threads 线程池
来源：http://zf.bjjhwx.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zh.haigaiapp.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xw.haigaiapp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://br.chemitech.net.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cv.9csxet.cn

[O03] 加锁保护共享数据
来源：http://oz.shxzukj.cn

Py:   with lock: shared += 1
来源：http://fw.muxihuayi.cn

PHP:  // 用 flock() 做文件锁
来源：http://tu.bookmarksfly.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kb.hnjuh.cn

TS:   // 同 JS
来源：http://qv.haigaiapp.cn

Java: synchronized (this) { shared++; }
来源：http://be.shxzukj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zs.chemitech.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://iy.hahajie.cn

C#:   lock (gate) { shared++; }
来源：http://bz.nicolike.cn

[O04] 定义异步函数并等待
来源：http://dn.wgjwhj.cn

Py:   async def f():⏎    await g()
来源：http://jo.bookmarksfly.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qg.lnxyls.cn

JS:   async function f() { await g(); }
来源：http://dk.shtwfgs.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nz.jianghongdianzi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ls.asd995.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kr.muxihuayi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kr.shxzukj.cn

C#:   async Task F() { await G(); }
来源：http://gx.wgjwhj.cn

[O05] 并发执行并等待全部完成
来源：http://zt.yuntaijiaju.cn

Py:   asyncio.gather(*tasks)
来源：http://tt.huanxung.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cu.yuexingan06.cn

JS:   await Promise.all(tasks)
来源：http://dx.hahajie.cn

TS:   await Promise.all(tasks)
来源：http://ff.shxzskj.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nv.asd995.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kw.jianghongdianzi.cn

Ruby: threads.map(&:join)
来源：http://te.wgjwhj.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ep.bjjhwx.cn

[O06] 使用进程池
来源：http://fb.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ub.huixiangedu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://iw.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://np.nicolike.cn

TS:   // child_process / cluster 模块
来源：http://qs.hnjuh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vv.huixinmuqiang.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fi.yuexingan06.cn

Ruby: // fork 块
来源：http://jo.asd995.cn

C#:   Parallel.For
来源：http://wr.jctech888.com.cn

================================================================================
来源：http://fj.shtwfgs.cn

P. 常用工具函数
来源：http://vx.colortex.cn

================================================================================
来源：http://rl.huanxung.cn

[P01] 生成 UUID
来源：http://ay.9csxet.cn

Py:   str(uuid.uuid4())
来源：http://nz.newstarts.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zr.bjjhwx.cn

JS:   crypto.randomUUID()
来源：http://bz.lnxyls.cn

TS:   crypto.randomUUID()
来源：http://zv.huixinmuqiang.cn

Java: UUID.randomUUID().toString()
来源：http://ib.muxihuayi.cn

Go:   // 用 github.com/google/uuid
来源：http://to.yuexingan06.cn

Ruby: SecureRandom.uuid
来源：http://sf.shtwfgs.cn

C#:   Guid.NewGuid().ToString()
来源：http://dy.521024.cn

[P02] MD5 / SHA256 摘要
来源：http://ke.bookmarksfly.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eh.szxytkj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jq.shtwfgs.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ti.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aa.newstarts.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kb.colortex.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zq.shxzskj.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bt.lnxyls.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rf.muxihuayi.cn

[P03] 生成短随机字符串
来源：http://be.chemitech.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pe.asd995.cn


<!-- 参考信息 -->