代发 wailian999

[L03] 设置自定义请求头
来源：http://zr.hnjuh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fq.wgjwhj.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ug.wgjwhj.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lo.szsharing.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uq.szsharing.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pc.yuntaijiaju.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yk.panjiajie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ki.yuexingan06.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ds.panjiajie.cn

[L04] 设置超时
来源：http://fg.yuexingan06.cn

Py:   requests.get(url, timeout=5)
来源：http://al.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yz.szsharing.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://es.colortex.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://li.chemitech.net.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rr.huixiangedu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bn.newstarts.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rb.gzmigu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ts.huanxung.cn

[L05] 上传文件（multipart）
来源：http://xp.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uz.yuexingan06.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://eb.huixiangedu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ep.lnxyls.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qs.szsharing.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pk.shxzukj.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ll.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ge.bjjhwx.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://om.bjjhwx.cn

[L06] 解析响应为 JSON
来源：http://cm.asd995.cn

Py:   resp.json()
来源：http://jv.shxzskj.cn

PHP:  json_decode($body, true);
来源：http://fw.shtwfgs.cn

JS:   await resp.json()
来源：http://ll.yuntaijiaju.cn

TS:   await resp.json()
来源：http://mh.jianghongdianzi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ea.huixiangedu.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qx.wgjwhj.cn

Ruby: JSON.parse(resp.body)
来源：http://zb.asd995.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ru.muxihuayi.cn

[L07] 处理 HTTP 状态码
来源：http://ol.szsharing.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zh.chemitech.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qd.muxihuayi.cn

JS:   resp.ok;  resp.status
来源：http://wt.lnxyls.cn

TS:   resp.ok;  resp.status
来源：http://dw.panjiajie.cn

Java: resp.statusCode()
来源：http://gi.gzmigu.cn

Go:   resp.StatusCode
来源：http://jj.newstarts.cn

Ruby: resp.code.to_i
来源：http://bu.shxzukj.cn

C#:   (int)resp.StatusCode
来源：http://ic.asd995.cn

[L08] 并发请求多个地址
来源：http://wn.shxzskj.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rm.panjiajie.cn

PHP:  curl_multi_init() 系列
来源：http://ok.jianghongdianzi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://av.gzmigu.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lc.shtwfgs.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ja.yuexingan06.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hl.bookmarksfly.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hl.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ek.bjjhwx.cn

================================================================================
来源：http://gq.jianghongdianzi.cn

M. 命令行 / 进程 / 环境
来源：http://ne.huixiangedu.cn

================================================================================
来源：http://cq.nicolike.cn

[M01] 读取命令行参数
来源：http://hi.huixiangedu.cn

Py:   sys.argv[1:]
来源：http://qq.bookmarksfly.cn

PHP:  $argv;  $argc;
来源：http://pa.jctech888.com.cn

JS:   process.argv.slice(2)
来源：http://ix.shxzukj.cn

TS:   process.argv.slice(2)
来源：http://bk.haigaiapp.cn

Java: args 数组（main 方法参数）
来源：http://lf.wgjwhj.cn

Go:   os.Args[1:]
来源：http://uy.bookmarksfly.cn

Ruby: ARGV
来源：http://pv.shxzskj.cn

C#:   args 数组（Main 方法参数）
来源：http://bd.shxzukj.cn

[M02] 读取环境变量
来源：http://qi.nszjky.cn

Py:   os.environ.get("HOME")
来源：http://it.shxzukj.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wx.huanxung.cn

JS:   process.env.HOME
来源：http://jf.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://sb.haigaiapp.cn

Java: System.getenv("HOME")
来源：http://xs.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wy.huixinmuqiang.cn

Ruby: ENV["HOME"]
来源：http://sc.nszjky.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lw.bjjhwx.cn

[M03] 执行外部命令
来源：http://yt.shtwfgs.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qp.panjiajie.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hh.newstarts.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gd.wgjwhj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://on.huanxung.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bb.shxzskj.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sp.9csxet.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mn.haigaiapp.cn

C#:   Process.Start("ls", "-l");
来源：http://yc.jctech888.com.cn

[M04] 获取当前工作目录
来源：http://tk.jianghongdianzi.cn

Py:   os.getcwd()
来源：http://eq.huixinmuqiang.cn

PHP:  getcwd();
来源：http://df.jianghongdianzi.cn

JS:   process.cwd()
来源：http://bo.hahajie.cn

TS:   process.cwd()
来源：http://ns.shtwfgs.cn

Java: Path.of("").toAbsolutePath()
来源：http://jx.jctech888.com.cn

Go:   os.Getwd()
来源：http://er.hnjuh.cn

Ruby: Dir.pwd
来源：http://ax.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vq.jianghongdianzi.cn

[M05] 设置退出码
来源：http://wo.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://af.nszjky.cn

PHP:  exit(1);
来源：http://fb.bjjhwx.cn

JS:   process.exit(1)
来源：http://hw.jctech888.com.cn

TS:   process.exit(1)
来源：http://rz.huanxung.cn

Java: System.exit(1)
来源：http://gb.newstarts.cn

Go:   os.Exit(1)
来源：http://oz.hnjuh.cn

Ruby: exit 1
来源：http://ue.huixiangedu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fg.jianghongdianzi.cn

[M06] 向标准错误输出
来源：http://jt.szsharing.cn

Py:   print("err", file=sys.stderr)
来源：http://xd.nicolike.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wj.jctech888.com.cn

JS:   console.error("err")
来源：http://uf.nicolike.cn

TS:   console.error("err")
来源：http://ql.wgjwhj.cn

Java: System.err.println("err")
来源：http://zn.colortex.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://on.lnxyls.cn

Ruby: warn "err"
来源：http://ij.szxytkj.cn

C#:   Console.Error.WriteLine("err")
来源：http://gx.wgjwhj.cn

[M07] 判断是否为主入口
来源：http://jw.gzmigu.cn

Py:   if __name__ == "__main__":
来源：http://qa.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eo.huixiangedu.cn

JS:   require.main === module
来源：http://ez.chemitech.net.cn

TS:   require.main === module
来源：http://qu.shxzukj.cn

Java: public static void main(String[] args)
来源：http://ih.gzmigu.cn

Go:   func main()
来源：http://cy.haigaiapp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fn.gzmigu.cn

C#:   static void Main(string[] args)
来源：http://zd.nicolike.cn

[M08] 获取系统与运行时信息
来源：http://ou.huixinmuqiang.cn

Py:   platform.system();  platform.python_version()
来源：http://zq.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://rp.lnxyls.cn

JS:   process.platform;  process.version
来源：http://bp.huanxung.cn

TS:   process.platform;  process.version
来源：http://xa.lnxyls.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://te.szsharing.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ev.nicolike.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rz.shxzskj.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hf.521024.cn

================================================================================
来源：http://tl.jianghongdianzi.cn

N. 数据结构与算法
来源：http://dk.colortex.cn

================================================================================
来源：http://op.colortex.cn

[N01] 二分查找（有序数组）
来源：http://of.newstarts.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yt.newstarts.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rm.huixiangedu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tg.521024.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nn.hahajie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ec.newstarts.cn

Go:   sort.SearchInts(arr, x)
来源：http://wp.yuntaijiaju.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://cl.shtwfgs.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fi.bjjhwx.cn

[N02] 排序（工程实践用内置实现）
来源：http://oa.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://uc.shxzukj.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://za.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eu.jctech888.com.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://yx.hnjuh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vc.bookmarksfly.cn

Go:   slices.Sort(arr)
来源：http://nm.colortex.cn

Ruby: arr.sort
来源：http://dh.jianghongdianzi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://um.shxzskj.cn

[N03] 快速排序（分治示例）
来源：http://uy.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ba.jianghongdianzi.cn

PHP:  // 递归实现，或用 usort
来源：http://if.szxytkj.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wx.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sc.panjiajie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gm.huanxung.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hy.haigaiapp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nm.gzmigu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yn.huanxung.cn

[N04] 斐波那契数列
来源：http://tv.panjiajie.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jk.yuexingan06.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nc.yuntaijiaju.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ao.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://do.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dm.lnxyls.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wf.asd995.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ys.asd995.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ct.colortex.cn

[N05] 最大公约数
来源：http://ba.shtwfgs.cn

Py:   math.gcd(a, b)
来源：http://by.nicolike.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://od.shxzskj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sz.huanxung.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ri.lnxyls.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mm.wgjwhj.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sz.haigaiapp.cn

Ruby: a.gcd(b)
来源：http://sb.hnjuh.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://id.lnxyls.cn

[N06] 判断回文字符串
来源：http://ak.jianghongdianzi.cn

Py:   s == s[::-1]
来源：http://vk.newstarts.cn

PHP:  $s === strrev($s);
来源：http://zm.wgjwhj.cn

JS:   s === [...s].reverse().join("")
来源：http://vf.huixiangedu.cn

TS:   s === [...s].reverse().join("")
来源：http://zm.colortex.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gj.nszjky.cn

Go:   // 双指针从两端比较
来源：http://cj.chemitech.net.cn

Ruby: s == s.reverse
来源：http://mj.9csxet.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://sg.huixiangedu.cn

[N07] 两数之和（返回下标）
来源：http://va.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fk.newstarts.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ji.shxzukj.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ns.newstarts.cn

TS:   // 手写 Map<string, number>
来源：http://ga.gzmigu.cn

Java: // 手写 HashMap
来源：http://vf.521024.cn

Go:   // 手写 map[int]int
来源：http://ir.huixiangedu.cn

Ruby: // 手写 Hash
来源：http://iq.hnjuh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rr.shtwfgs.cn

[N08] 生成全排列
来源：http://hn.lnxyls.cn

Py:   itertools.permutations(arr)
来源：http://mt.bookmarksfly.cn

PHP:  // 手写递归交换
来源：http://dl.newstarts.cn

JS:   // 手写回溯递归
来源：http://bw.wgjwhj.cn

TS:   // 手写回溯递归
来源：http://sb.lnxyls.cn

Java: // 手写回溯递归
来源：http://sg.gzmigu.cn

Go:   // 手写回溯递归
来源：http://yj.bjjhwx.cn

Ruby: arr.permutation.to_a
来源：http://fv.bookmarksfly.cn

C#:   // 手写回溯递归
来源：http://zy.9csxet.cn

[N09] 栈与队列
来源：http://ku.huixiangedu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mm.shtwfgs.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bp.jctech888.com.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qv.yuntaijiaju.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ii.huixiangedu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pe.shtwfgs.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pa.panjiajie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://co.shxzskj.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rv.shtwfgs.cn

[N10] 链表节点定义
来源：http://zz.bookmarksfly.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hs.wgjwhj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xz.szsharing.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bt.shxzskj.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lr.muxihuayi.cn

Java: class Node { int v; Node next; }
来源：http://lu.shxzukj.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hl.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ub.nicolike.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://am.hnjuh.cn

[N11] 二叉树中序遍历
来源：http://pr.szxytkj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xq.yuexingan06.cn

PHP:  // 手写递归函数
来源：http://mt.shxzukj.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sq.muxihuayi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gz.lnxyls.cn

Java: // 手写递归
来源：http://bn.521024.cn

Go:   // 手写递归
来源：http://hi.jctech888.com.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lu.521024.cn

C#:   // 手写递归
来源：http://xe.521024.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://os.chemitech.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qo.521024.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://in.asd995.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hw.jianghongdianzi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vy.bookmarksfly.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yn.521024.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://xd.jctech888.com.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ju.9csxet.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mf.9csxet.cn

================================================================================
来源：http://oj.shxzskj.cn

O. 并发与异步
来源：http://yt.huanxung.cn

================================================================================
来源：http://ky.szxytkj.cn

[O01] 启动一个线程
来源：http://mz.muxihuayi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ek.yuntaijiaju.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ls.521024.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cu.jianghongdianzi.cn

TS:   // 同 JS
来源：http://vi.bjjhwx.cn

Java: new Thread(() -> f()).start()
来源：http://eh.huixiangedu.cn

Go:   go f()
来源：http://ar.asd995.cn

Ruby: Thread.new { f }
来源：http://cb.hahajie.cn

C#:   Task.Run(() => F());
来源：http://jm.asd995.cn

[O02] 使用线程池
来源：http://qh.nicolike.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hj.colortex.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wu.nszjky.cn

JS:   // worker_threads 线程池
来源：http://bj.nicolike.cn

TS:   // worker_threads 线程池
来源：http://tc.9csxet.cn

Java: Executors.newFixedThreadPool(4)
来源：http://iy.huanxung.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ks.muxihuayi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gb.panjiajie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cd.nicolike.cn

[O03] 加锁保护共享数据
来源：http://mz.shtwfgs.cn

Py:   with lock: shared += 1
来源：http://eu.nicolike.cn

PHP:  // 用 flock() 做文件锁
来源：http://sd.huixiangedu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aa.colortex.cn

TS:   // 同 JS
来源：http://mi.bjjhwx.cn

Java: synchronized (this) { shared++; }
来源：http://lq.yuexingan06.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sg.jianghongdianzi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ms.szxytkj.cn

C#:   lock (gate) { shared++; }
来源：http://dq.bookmarksfly.cn

[O04] 定义异步函数并等待
来源：http://fo.huixinmuqiang.cn

Py:   async def f():⏎    await g()
来源：http://dm.haigaiapp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ic.muxihuayi.cn

JS:   async function f() { await g(); }
来源：http://wn.muxihuayi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nv.jctech888.com.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fh.shxzukj.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sa.lnxyls.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tt.nszjky.cn

C#:   async Task F() { await G(); }
来源：http://hp.huanxung.cn

[O05] 并发执行并等待全部完成
来源：http://sp.bookmarksfly.cn

Py:   asyncio.gather(*tasks)
来源：http://mz.521024.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xt.yuntaijiaju.cn

JS:   await Promise.all(tasks)
来源：http://mn.521024.cn

TS:   await Promise.all(tasks)
来源：http://wd.szsharing.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dh.szxytkj.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mo.gzmigu.cn

Ruby: threads.map(&:join)
来源：http://yl.nicolike.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ew.shxzukj.cn

[O06] 使用进程池
来源：http://co.yuexingan06.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dj.haigaiapp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qa.haigaiapp.cn

JS:   // child_process / cluster 模块
来源：http://pg.shtwfgs.cn

TS:   // child_process / cluster 模块
来源：http://qr.nicolike.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ok.jianghongdianzi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://en.chemitech.net.cn

Ruby: // fork 块
来源：http://gq.szsharing.cn

C#:   Parallel.For
来源：http://lz.haigaiapp.cn

================================================================================
来源：http://zl.huanxung.cn

P. 常用工具函数
来源：http://wj.huixinmuqiang.cn

================================================================================
来源：http://ut.szsharing.cn


<!-- 参考信息 -->