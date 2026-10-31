代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fn.bookmarksfly.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ri.yuexingan06.cn

[L05] 上传文件（multipart）
来源：http://wz.hnjuh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://os.gzmigu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xm.chemitech.net.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bp.huanxung.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mr.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pd.haigaiapp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dn.asd995.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fu.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://me.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://jx.newstarts.cn

Py:   resp.json()
来源：http://hk.521024.cn

PHP:  json_decode($body, true);
来源：http://dp.shtwfgs.cn

JS:   await resp.json()
来源：http://vt.hnjuh.cn

TS:   await resp.json()
来源：http://pb.shxzukj.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xh.shxzskj.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cy.hnjuh.cn

Ruby: JSON.parse(resp.body)
来源：http://lg.yuexingan06.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fl.szxytkj.cn

[L07] 处理 HTTP 状态码
来源：http://mf.nszjky.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pa.asd995.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cb.9csxet.cn

JS:   resp.ok;  resp.status
来源：http://mr.asd995.cn

TS:   resp.ok;  resp.status
来源：http://jt.wgjwhj.cn

Java: resp.statusCode()
来源：http://tr.9csxet.cn

Go:   resp.StatusCode
来源：http://oe.newstarts.cn

Ruby: resp.code.to_i
来源：http://bk.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://ym.shxzskj.cn

[L08] 并发请求多个地址
来源：http://md.yuntaijiaju.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bv.shtwfgs.cn

PHP:  curl_multi_init() 系列
来源：http://ku.wgjwhj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mf.yuntaijiaju.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ff.wgjwhj.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xp.panjiajie.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qy.haigaiapp.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cw.shtwfgs.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uc.haigaiapp.cn

================================================================================
来源：http://aw.lnxyls.cn

M. 命令行 / 进程 / 环境
来源：http://tp.chemitech.net.cn

================================================================================
来源：http://uh.asd995.cn

[M01] 读取命令行参数
来源：http://hj.lnxyls.cn

Py:   sys.argv[1:]
来源：http://el.jctech888.com.cn

PHP:  $argv;  $argc;
来源：http://qf.bookmarksfly.cn

JS:   process.argv.slice(2)
来源：http://rz.asd995.cn

TS:   process.argv.slice(2)
来源：http://tx.lnxyls.cn

Java: args 数组（main 方法参数）
来源：http://cl.huanxung.cn

Go:   os.Args[1:]
来源：http://kn.521024.cn

Ruby: ARGV
来源：http://ig.shxzukj.cn

C#:   args 数组（Main 方法参数）
来源：http://yk.wgjwhj.cn

[M02] 读取环境变量
来源：http://an.chemitech.net.cn

Py:   os.environ.get("HOME")
来源：http://yz.huixinmuqiang.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ip.shxzskj.cn

JS:   process.env.HOME
来源：http://bc.huanxung.cn

TS:   process.env.HOME
来源：http://gs.jianghongdianzi.cn

Java: System.getenv("HOME")
来源：http://ha.newstarts.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cd.chemitech.net.cn

Ruby: ENV["HOME"]
来源：http://ze.bookmarksfly.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qn.gzmigu.cn

[M03] 执行外部命令
来源：http://nd.nicolike.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uz.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ln.jianghongdianzi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ok.shtwfgs.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://hx.huixinmuqiang.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hu.yuntaijiaju.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xj.nszjky.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dp.lnxyls.cn

C#:   Process.Start("ls", "-l");
来源：http://af.yuntaijiaju.cn

[M04] 获取当前工作目录
来源：http://tu.hahajie.cn

Py:   os.getcwd()
来源：http://jh.jianghongdianzi.cn

PHP:  getcwd();
来源：http://hb.chemitech.net.cn

JS:   process.cwd()
来源：http://kt.bjjhwx.cn

TS:   process.cwd()
来源：http://ug.nszjky.cn

Java: Path.of("").toAbsolutePath()
来源：http://az.yuntaijiaju.cn

Go:   os.Getwd()
来源：http://us.jianghongdianzi.cn

Ruby: Dir.pwd
来源：http://le.shxzukj.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wv.yuexingan06.cn

[M05] 设置退出码
来源：http://qo.hnjuh.cn

Py:   sys.exit(1)
来源：http://oq.shtwfgs.cn

PHP:  exit(1);
来源：http://gm.lnxyls.cn

JS:   process.exit(1)
来源：http://nc.bjjhwx.cn

TS:   process.exit(1)
来源：http://js.gzmigu.cn

Java: System.exit(1)
来源：http://ni.lnxyls.cn

Go:   os.Exit(1)
来源：http://gd.yuexingan06.cn

Ruby: exit 1
来源：http://iu.newstarts.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ta.newstarts.cn

[M06] 向标准错误输出
来源：http://fs.bjjhwx.cn

Py:   print("err", file=sys.stderr)
来源：http://up.nszjky.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://os.yuexingan06.cn

JS:   console.error("err")
来源：http://qs.haigaiapp.cn

TS:   console.error("err")
来源：http://vb.shxzukj.cn

Java: System.err.println("err")
来源：http://ao.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ke.chemitech.net.cn

Ruby: warn "err"
来源：http://ct.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://ym.chemitech.net.cn

[M07] 判断是否为主入口
来源：http://am.521024.cn

Py:   if __name__ == "__main__":
来源：http://va.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vg.chemitech.net.cn

JS:   require.main === module
来源：http://qm.newstarts.cn

TS:   require.main === module
来源：http://ug.huanxung.cn

Java: public static void main(String[] args)
来源：http://ni.shxzukj.cn

Go:   func main()
来源：http://ay.shtwfgs.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nd.haigaiapp.cn

C#:   static void Main(string[] args)
来源：http://ub.nszjky.cn

[M08] 获取系统与运行时信息
来源：http://el.9csxet.cn

Py:   platform.system();  platform.python_version()
来源：http://mp.521024.cn

PHP:  PHP_OS;  phpversion();
来源：http://ex.huixinmuqiang.cn

JS:   process.platform;  process.version
来源：http://ro.bjjhwx.cn

TS:   process.platform;  process.version
来源：http://iy.jianghongdianzi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bs.hahajie.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kb.huixiangedu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oy.nszjky.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://un.haigaiapp.cn

================================================================================
来源：http://iv.asd995.cn

N. 数据结构与算法
来源：http://uv.shtwfgs.cn

================================================================================
来源：http://yx.asd995.cn

[N01] 二分查找（有序数组）
来源：http://tj.hahajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sv.chemitech.net.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yk.chemitech.net.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mn.shxzskj.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://as.bookmarksfly.cn

Java: Arrays.binarySearch(arr, x)
来源：http://sq.shxzukj.cn

Go:   sort.SearchInts(arr, x)
来源：http://bm.bjjhwx.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hp.hahajie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ie.521024.cn

[N02] 排序（工程实践用内置实现）
来源：http://tn.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://la.wgjwhj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cn.huixinmuqiang.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mm.haigaiapp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ct.szxytkj.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bz.huixiangedu.cn

Go:   slices.Sort(arr)
来源：http://kd.hahajie.cn

Ruby: arr.sort
来源：http://gi.bookmarksfly.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kx.chemitech.net.cn

[N03] 快速排序（分治示例）
来源：http://yo.huixiangedu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sq.chemitech.net.cn

PHP:  // 递归实现，或用 usort
来源：http://hs.bjjhwx.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ip.panjiajie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ld.gzmigu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gw.newstarts.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tm.9csxet.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jp.hahajie.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xn.newstarts.cn

[N04] 斐波那契数列
来源：http://bz.asd995.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yw.hahajie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xl.huixinmuqiang.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sh.shtwfgs.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xt.521024.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eu.bjjhwx.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sx.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yz.9csxet.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://th.huixiangedu.cn

[N05] 最大公约数
来源：http://pi.haigaiapp.cn

Py:   math.gcd(a, b)
来源：http://sw.shxzskj.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iv.nszjky.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zs.bookmarksfly.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tq.hahajie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mg.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qd.shtwfgs.cn

Ruby: a.gcd(b)
来源：http://ko.lnxyls.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zv.colortex.cn

[N06] 判断回文字符串
来源：http://ow.yuntaijiaju.cn

Py:   s == s[::-1]
来源：http://hf.gzmigu.cn

PHP:  $s === strrev($s);
来源：http://xr.panjiajie.cn

JS:   s === [...s].reverse().join("")
来源：http://os.wgjwhj.cn

TS:   s === [...s].reverse().join("")
来源：http://bz.nszjky.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mz.huanxung.cn

Go:   // 双指针从两端比较
来源：http://uh.newstarts.cn

Ruby: s == s.reverse
来源：http://lv.gzmigu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ki.shxzskj.cn

[N07] 两数之和（返回下标）
来源：http://pi.shtwfgs.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jb.huixinmuqiang.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rx.huanxung.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rl.hnjuh.cn

TS:   // 手写 Map<string, number>
来源：http://od.lnxyls.cn

Java: // 手写 HashMap
来源：http://vg.chemitech.net.cn

Go:   // 手写 map[int]int
来源：http://ta.nicolike.cn

Ruby: // 手写 Hash
来源：http://lm.shxzskj.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qh.szxytkj.cn

[N08] 生成全排列
来源：http://pw.jianghongdianzi.cn

Py:   itertools.permutations(arr)
来源：http://rz.shxzskj.cn

PHP:  // 手写递归交换
来源：http://zx.asd995.cn

JS:   // 手写回溯递归
来源：http://zf.yuntaijiaju.cn

TS:   // 手写回溯递归
来源：http://gm.shxzukj.cn

Java: // 手写回溯递归
来源：http://kn.wgjwhj.cn

Go:   // 手写回溯递归
来源：http://io.colortex.cn

Ruby: arr.permutation.to_a
来源：http://bg.szsharing.cn

C#:   // 手写回溯递归
来源：http://dh.521024.cn

[N09] 栈与队列
来源：http://gh.shtwfgs.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rc.huanxung.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yb.colortex.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ki.shxzukj.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vk.9csxet.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://am.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nn.huanxung.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xp.chemitech.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ga.jianghongdianzi.cn

[N10] 链表节点定义
来源：http://fn.nicolike.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pj.jctech888.com.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gu.yuexingan06.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ml.521024.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lm.haigaiapp.cn

Java: class Node { int v; Node next; }
来源：http://ea.jctech888.com.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zh.bookmarksfly.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pz.nszjky.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ai.wgjwhj.cn

[N11] 二叉树中序遍历
来源：http://uw.nicolike.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vn.nicolike.cn

PHP:  // 手写递归函数
来源：http://mg.521024.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wu.huanxung.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qt.nszjky.cn

Java: // 手写递归
来源：http://nm.szxytkj.cn

Go:   // 手写递归
来源：http://lg.panjiajie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xz.szsharing.cn

C#:   // 手写递归
来源：http://xt.yuexingan06.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jg.bookmarksfly.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lg.hahajie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tv.haigaiapp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jq.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cu.shtwfgs.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ik.hahajie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hv.shxzskj.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sn.jctech888.com.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vk.hnjuh.cn

================================================================================
来源：http://ts.szxytkj.cn

O. 并发与异步
来源：http://cs.szxytkj.cn

================================================================================
来源：http://uq.shxzukj.cn

[O01] 启动一个线程
来源：http://es.shxzskj.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rj.9csxet.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mq.huanxung.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wi.szxytkj.cn

TS:   // 同 JS
来源：http://iv.hahajie.cn

Java: new Thread(() -> f()).start()
来源：http://ki.huixinmuqiang.cn

Go:   go f()
来源：http://fx.asd995.cn

Ruby: Thread.new { f }
来源：http://ok.newstarts.cn

C#:   Task.Run(() => F());
来源：http://ld.yuntaijiaju.cn

[O02] 使用线程池
来源：http://jn.wgjwhj.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nx.haigaiapp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zr.shtwfgs.cn

JS:   // worker_threads 线程池
来源：http://ao.szxytkj.cn

TS:   // worker_threads 线程池
来源：http://hf.yuexingan06.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ic.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cw.shxzukj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rf.huanxung.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ru.9csxet.cn

[O03] 加锁保护共享数据
来源：http://we.bookmarksfly.cn

Py:   with lock: shared += 1
来源：http://gm.521024.cn

PHP:  // 用 flock() 做文件锁
来源：http://tz.wgjwhj.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://us.bookmarksfly.cn

TS:   // 同 JS
来源：http://qp.bookmarksfly.cn

Java: synchronized (this) { shared++; }
来源：http://nm.huixiangedu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ps.9csxet.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lh.nicolike.cn

C#:   lock (gate) { shared++; }
来源：http://xr.panjiajie.cn

[O04] 定义异步函数并等待
来源：http://xg.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://go.newstarts.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lk.colortex.cn

JS:   async function f() { await g(); }
来源：http://ox.hahajie.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xc.shtwfgs.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xl.szsharing.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://no.shxzukj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wo.jctech888.com.cn

C#:   async Task F() { await G(); }
来源：http://zv.nicolike.cn

[O05] 并发执行并等待全部完成
来源：http://ri.shtwfgs.cn

Py:   asyncio.gather(*tasks)
来源：http://tv.hnjuh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gs.wgjwhj.cn

JS:   await Promise.all(tasks)
来源：http://ps.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://ul.yuntaijiaju.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wt.9csxet.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yb.521024.cn

Ruby: threads.map(&:join)
来源：http://rl.huixinmuqiang.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ug.yuntaijiaju.cn

[O06] 使用进程池
来源：http://sj.muxihuayi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ah.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ld.huanxung.cn

JS:   // child_process / cluster 模块
来源：http://hs.haigaiapp.cn

TS:   // child_process / cluster 模块
来源：http://cx.521024.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ta.gzmigu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oh.shxzskj.cn

Ruby: // fork 块
来源：http://ez.shxzukj.cn

C#:   Parallel.For
来源：http://wl.9csxet.cn

================================================================================
来源：http://xn.nicolike.cn

P. 常用工具函数
来源：http://au.szxytkj.cn

================================================================================
来源：http://lb.jianghongdianzi.cn

[P01] 生成 UUID
来源：http://kp.shxzukj.cn

Py:   str(uuid.uuid4())
来源：http://rm.szxytkj.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xg.szxytkj.cn

JS:   crypto.randomUUID()
来源：http://pw.panjiajie.cn

TS:   crypto.randomUUID()
来源：http://hk.9csxet.cn

Java: UUID.randomUUID().toString()
来源：http://me.szxytkj.cn

Go:   // 用 github.com/google/uuid
来源：http://oa.chemitech.net.cn

Ruby: SecureRandom.uuid
来源：http://ri.szsharing.cn

C#:   Guid.NewGuid().ToString()
来源：http://hu.wgjwhj.cn

[P02] MD5 / SHA256 摘要
来源：http://wg.yuexingan06.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kv.szsharing.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fp.bookmarksfly.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://do.haigaiapp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sb.haigaiapp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oa.9csxet.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sf.wgjwhj.cn


<!-- 参考信息 -->