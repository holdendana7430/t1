代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uk.hnjuh.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yo.9csxet.cn

[L05] 上传文件（multipart）
来源：http://jr.jctech888.com.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wn.jctech888.com.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fk.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vj.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jc.szxytkj.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vk.shxzskj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dw.gzmigu.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lc.chemitech.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hw.huanxung.cn

[L06] 解析响应为 JSON
来源：http://bj.521024.cn

Py:   resp.json()
来源：http://wt.gzmigu.cn

PHP:  json_decode($body, true);
来源：http://bz.muxihuayi.cn

JS:   await resp.json()
来源：http://cs.huixinmuqiang.cn

TS:   await resp.json()
来源：http://eh.lnxyls.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pe.newstarts.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://up.jctech888.com.cn

Ruby: JSON.parse(resp.body)
来源：http://cf.hahajie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xc.newstarts.cn

[L07] 处理 HTTP 状态码
来源：http://vn.jctech888.com.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kr.szxytkj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rt.newstarts.cn

JS:   resp.ok;  resp.status
来源：http://rx.hahajie.cn

TS:   resp.ok;  resp.status
来源：http://np.wgjwhj.cn

Java: resp.statusCode()
来源：http://se.szxytkj.cn

Go:   resp.StatusCode
来源：http://rh.hahajie.cn

Ruby: resp.code.to_i
来源：http://fq.shxzskj.cn

C#:   (int)resp.StatusCode
来源：http://uo.colortex.cn

[L08] 并发请求多个地址
来源：http://lh.shtwfgs.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wi.colortex.cn

PHP:  curl_multi_init() 系列
来源：http://nj.szsharing.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lf.shxzskj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xu.szsharing.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vr.bjjhwx.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ke.shxzukj.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gk.chemitech.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cl.colortex.cn

================================================================================
来源：http://sn.bjjhwx.cn

M. 命令行 / 进程 / 环境
来源：http://at.shxzukj.cn

================================================================================
来源：http://nd.hnjuh.cn

[M01] 读取命令行参数
来源：http://wa.asd995.cn

Py:   sys.argv[1:]
来源：http://df.nszjky.cn

PHP:  $argv;  $argc;
来源：http://nv.nszjky.cn

JS:   process.argv.slice(2)
来源：http://je.hahajie.cn

TS:   process.argv.slice(2)
来源：http://om.bookmarksfly.cn

Java: args 数组（main 方法参数）
来源：http://gb.asd995.cn

Go:   os.Args[1:]
来源：http://bm.panjiajie.cn

Ruby: ARGV
来源：http://va.lnxyls.cn

C#:   args 数组（Main 方法参数）
来源：http://ox.chemitech.net.cn

[M02] 读取环境变量
来源：http://ki.asd995.cn

Py:   os.environ.get("HOME")
来源：http://jl.hahajie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cn.muxihuayi.cn

JS:   process.env.HOME
来源：http://no.chemitech.net.cn

TS:   process.env.HOME
来源：http://gx.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://rz.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mm.colortex.cn

Ruby: ENV["HOME"]
来源：http://zc.hahajie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bz.shxzukj.cn

[M03] 执行外部命令
来源：http://wi.wgjwhj.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ii.521024.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cc.asd995.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ye.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://jj.nicolike.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fw.shtwfgs.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://oy.jctech888.com.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kp.wgjwhj.cn

C#:   Process.Start("ls", "-l");
来源：http://tc.shxzskj.cn

[M04] 获取当前工作目录
来源：http://qr.bookmarksfly.cn

Py:   os.getcwd()
来源：http://lp.yuntaijiaju.cn

PHP:  getcwd();
来源：http://sw.panjiajie.cn

JS:   process.cwd()
来源：http://li.haigaiapp.cn

TS:   process.cwd()
来源：http://tr.chemitech.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://lr.newstarts.cn

Go:   os.Getwd()
来源：http://zg.yuntaijiaju.cn

Ruby: Dir.pwd
来源：http://ee.521024.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bb.panjiajie.cn

[M05] 设置退出码
来源：http://iv.szxytkj.cn

Py:   sys.exit(1)
来源：http://oz.nicolike.cn

PHP:  exit(1);
来源：http://pu.muxihuayi.cn

JS:   process.exit(1)
来源：http://cs.huixinmuqiang.cn

TS:   process.exit(1)
来源：http://av.szsharing.cn

Java: System.exit(1)
来源：http://sd.lnxyls.cn

Go:   os.Exit(1)
来源：http://rd.szsharing.cn

Ruby: exit 1
来源：http://qw.9csxet.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gf.521024.cn

[M06] 向标准错误输出
来源：http://xi.hahajie.cn

Py:   print("err", file=sys.stderr)
来源：http://ge.jianghongdianzi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://if.yuexingan06.cn

JS:   console.error("err")
来源：http://li.chemitech.net.cn

TS:   console.error("err")
来源：http://fz.haigaiapp.cn

Java: System.err.println("err")
来源：http://bg.521024.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://js.wgjwhj.cn

Ruby: warn "err"
来源：http://pm.nicolike.cn

C#:   Console.Error.WriteLine("err")
来源：http://ij.huanxung.cn

[M07] 判断是否为主入口
来源：http://dn.shxzskj.cn

Py:   if __name__ == "__main__":
来源：http://gj.hahajie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tb.szsharing.cn

JS:   require.main === module
来源：http://rv.haigaiapp.cn

TS:   require.main === module
来源：http://xi.yuexingan06.cn

Java: public static void main(String[] args)
来源：http://lq.colortex.cn

Go:   func main()
来源：http://aw.huixinmuqiang.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xf.jctech888.com.cn

C#:   static void Main(string[] args)
来源：http://lg.newstarts.cn

[M08] 获取系统与运行时信息
来源：http://rr.panjiajie.cn

Py:   platform.system();  platform.python_version()
来源：http://oj.panjiajie.cn

PHP:  PHP_OS;  phpversion();
来源：http://dw.jctech888.com.cn

JS:   process.platform;  process.version
来源：http://md.hahajie.cn

TS:   process.platform;  process.version
来源：http://vf.szsharing.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ps.lnxyls.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oz.asd995.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ed.newstarts.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ks.521024.cn

================================================================================
来源：http://am.huixiangedu.cn

N. 数据结构与算法
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://jo.9csxet.cn

[N01] 二分查找（有序数组）
来源：http://ai.chemitech.net.cn

Py:   bisect.bisect_left(arr, x)
来源：http://iq.wgjwhj.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tu.9csxet.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gz.shtwfgs.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://et.521024.cn

Java: Arrays.binarySearch(arr, x)
来源：http://td.wgjwhj.cn

Go:   sort.SearchInts(arr, x)
来源：http://ts.jianghongdianzi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xc.chemitech.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pj.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://it.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://rl.nszjky.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dw.yuexingan06.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gt.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ck.9csxet.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bg.hnjuh.cn

Go:   slices.Sort(arr)
来源：http://mh.jctech888.com.cn

Ruby: arr.sort
来源：http://ft.wgjwhj.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://of.haigaiapp.cn

[N03] 快速排序（分治示例）
来源：http://xg.shxzukj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bt.gzmigu.cn

PHP:  // 递归实现，或用 usort
来源：http://td.shxzukj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kq.shxzukj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ud.nicolike.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bq.chemitech.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nv.wgjwhj.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rd.nszjky.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mg.colortex.cn

[N04] 斐波那契数列
来源：http://qf.jianghongdianzi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lr.gzmigu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wj.wgjwhj.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://im.asd995.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fn.newstarts.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xq.huixinmuqiang.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jc.yuexingan06.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iq.nicolike.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oa.jctech888.com.cn

[N05] 最大公约数
来源：http://hs.9csxet.cn

Py:   math.gcd(a, b)
来源：http://va.yuexingan06.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fc.lnxyls.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hu.asd995.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jh.jctech888.com.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tr.521024.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tf.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://wq.gzmigu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jr.shxzskj.cn

[N06] 判断回文字符串
来源：http://dk.521024.cn

Py:   s == s[::-1]
来源：http://ls.huixiangedu.cn

PHP:  $s === strrev($s);
来源：http://so.bookmarksfly.cn

JS:   s === [...s].reverse().join("")
来源：http://cf.szsharing.cn

TS:   s === [...s].reverse().join("")
来源：http://fd.hnjuh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iz.jianghongdianzi.cn

Go:   // 双指针从两端比较
来源：http://hm.nicolike.cn

Ruby: s == s.reverse
来源：http://so.chemitech.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://el.haigaiapp.cn

[N07] 两数之和（返回下标）
来源：http://tp.muxihuayi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ep.bookmarksfly.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tv.shtwfgs.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nm.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://ou.hahajie.cn

Java: // 手写 HashMap
来源：http://uf.haigaiapp.cn

Go:   // 手写 map[int]int
来源：http://rc.muxihuayi.cn

Ruby: // 手写 Hash
来源：http://jm.huixiangedu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://od.jianghongdianzi.cn

[N08] 生成全排列
来源：http://xo.newstarts.cn

Py:   itertools.permutations(arr)
来源：http://kq.muxihuayi.cn

PHP:  // 手写递归交换
来源：http://pd.huanxung.cn

JS:   // 手写回溯递归
来源：http://ls.colortex.cn

TS:   // 手写回溯递归
来源：http://js.muxihuayi.cn

Java: // 手写回溯递归
来源：http://pt.521024.cn

Go:   // 手写回溯递归
来源：http://fp.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://bu.nicolike.cn

C#:   // 手写回溯递归
来源：http://fu.muxihuayi.cn

[N09] 栈与队列
来源：http://ro.muxihuayi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tx.colortex.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nj.nszjky.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ln.lnxyls.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://an.szsharing.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fc.nszjky.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hg.gzmigu.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tm.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ws.haigaiapp.cn

[N10] 链表节点定义
来源：http://hy.nszjky.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gw.hnjuh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cp.jctech888.com.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dr.jctech888.com.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rn.huanxung.cn

Java: class Node { int v; Node next; }
来源：http://xa.shxzskj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vp.hnjuh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jy.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://da.szsharing.cn

[N11] 二叉树中序遍历
来源：http://hl.jianghongdianzi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sf.hahajie.cn

PHP:  // 手写递归函数
来源：http://gc.bjjhwx.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://te.wgjwhj.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://td.huixinmuqiang.cn

Java: // 手写递归
来源：http://zw.huanxung.cn

Go:   // 手写递归
来源：http://tu.muxihuayi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://os.gzmigu.cn

C#:   // 手写递归
来源：http://dw.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vh.shxzskj.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uv.chemitech.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ks.hahajie.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wg.huanxung.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gi.jctech888.com.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gx.haigaiapp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nx.hahajie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://av.haigaiapp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://af.bjjhwx.cn

================================================================================
来源：http://hz.yuntaijiaju.cn

O. 并发与异步
来源：http://vn.huixinmuqiang.cn

================================================================================
来源：http://zq.panjiajie.cn

[O01] 启动一个线程
来源：http://vn.bjjhwx.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fb.huanxung.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jl.szxytkj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qx.shxzukj.cn

TS:   // 同 JS
来源：http://bz.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://og.hahajie.cn

Go:   go f()
来源：http://mg.bookmarksfly.cn

Ruby: Thread.new { f }
来源：http://hp.muxihuayi.cn

C#:   Task.Run(() => F());
来源：http://fh.bookmarksfly.cn

[O02] 使用线程池
来源：http://ka.jianghongdianzi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xc.huixinmuqiang.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ov.szxytkj.cn

JS:   // worker_threads 线程池
来源：http://zl.newstarts.cn

TS:   // worker_threads 线程池
来源：http://bw.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qr.szxytkj.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wz.szxytkj.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kw.shxzukj.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wy.bjjhwx.cn

[O03] 加锁保护共享数据
来源：http://ff.haigaiapp.cn

Py:   with lock: shared += 1
来源：http://qk.gzmigu.cn

PHP:  // 用 flock() 做文件锁
来源：http://cs.lnxyls.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ro.chemitech.net.cn

TS:   // 同 JS
来源：http://oo.asd995.cn

Java: synchronized (this) { shared++; }
来源：http://br.nszjky.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wy.newstarts.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://be.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://yl.wgjwhj.cn

[O04] 定义异步函数并等待
来源：http://sd.bjjhwx.cn

Py:   async def f():⏎    await g()
来源：http://sg.hahajie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ig.gzmigu.cn

JS:   async function f() { await g(); }
来源：http://un.huanxung.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kc.colortex.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mn.shxzskj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yg.chemitech.net.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kc.gzmigu.cn

C#:   async Task F() { await G(); }
来源：http://rb.hnjuh.cn

[O05] 并发执行并等待全部完成
来源：http://zm.jianghongdianzi.cn

Py:   asyncio.gather(*tasks)
来源：http://af.newstarts.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ei.jctech888.com.cn

JS:   await Promise.all(tasks)
来源：http://zu.panjiajie.cn

TS:   await Promise.all(tasks)
来源：http://vl.hnjuh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jr.jianghongdianzi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kp.lnxyls.cn

Ruby: threads.map(&:join)
来源：http://ad.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lv.nicolike.cn

[O06] 使用进程池
来源：http://kp.nicolike.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cp.yuexingan06.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ly.nicolike.cn

JS:   // child_process / cluster 模块
来源：http://vt.hahajie.cn

TS:   // child_process / cluster 模块
来源：http://st.szsharing.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hl.jctech888.com.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://es.9csxet.cn

Ruby: // fork 块
来源：http://yw.asd995.cn

C#:   Parallel.For
来源：http://sa.huixinmuqiang.cn

================================================================================
来源：http://xk.huanxung.cn

P. 常用工具函数
来源：http://kw.yuexingan06.cn

================================================================================
来源：http://ti.nicolike.cn

[P01] 生成 UUID
来源：http://mq.yuntaijiaju.cn

Py:   str(uuid.uuid4())
来源：http://vt.9csxet.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hq.hahajie.cn

JS:   crypto.randomUUID()
来源：http://wu.newstarts.cn

TS:   crypto.randomUUID()
来源：http://jc.yuexingan06.cn

Java: UUID.randomUUID().toString()
来源：http://nh.huixiangedu.cn

Go:   // 用 github.com/google/uuid
来源：http://bo.521024.cn

Ruby: SecureRandom.uuid
来源：http://xq.nszjky.cn

C#:   Guid.NewGuid().ToString()
来源：http://rf.huixinmuqiang.cn

[P02] MD5 / SHA256 摘要
来源：http://va.colortex.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ym.shxzukj.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zz.jctech888.com.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qq.9csxet.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hr.szxytkj.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://af.huanxung.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ea.gzmigu.cn


<!-- 参考信息 -->