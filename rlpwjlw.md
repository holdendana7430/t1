代发 wailian999

[L03] 设置自定义请求头
来源：http://ef.wgjwhj.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ey.huanxung.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vc.shtwfgs.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wh.muxihuayi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://of.panjiajie.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cb.lnxyls.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://so.jctech888.com.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sb.bookmarksfly.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://zy.yuexingan06.cn

[L04] 设置超时
来源：http://st.wgjwhj.cn

Py:   requests.get(url, timeout=5)
来源：http://uq.jianghongdianzi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uc.hahajie.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pa.9csxet.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sp.colortex.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://by.asd995.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bb.huixiangedu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yi.yuexingan06.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mz.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://bc.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qr.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bt.nicolike.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zt.9csxet.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://nc.hahajie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rk.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zy.9csxet.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xc.shtwfgs.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uq.jctech888.com.cn

[L06] 解析响应为 JSON
来源：http://kd.shtwfgs.cn

Py:   resp.json()
来源：http://zn.shtwfgs.cn

PHP:  json_decode($body, true);
来源：http://ov.lnxyls.cn

JS:   await resp.json()
来源：http://wh.yuexingan06.cn

TS:   await resp.json()
来源：http://kz.9csxet.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vg.yuntaijiaju.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pe.nicolike.cn

Ruby: JSON.parse(resp.body)
来源：http://jd.shxzskj.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vr.shxzukj.cn

[L07] 处理 HTTP 状态码
来源：http://hd.shxzukj.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tn.wgjwhj.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://be.shxzskj.cn

JS:   resp.ok;  resp.status
来源：http://vc.shtwfgs.cn

TS:   resp.ok;  resp.status
来源：http://gq.panjiajie.cn

Java: resp.statusCode()
来源：http://il.newstarts.cn

Go:   resp.StatusCode
来源：http://ai.lnxyls.cn

Ruby: resp.code.to_i
来源：http://gi.colortex.cn

C#:   (int)resp.StatusCode
来源：http://wf.hnjuh.cn

[L08] 并发请求多个地址
来源：http://po.jctech888.com.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://az.bookmarksfly.cn

PHP:  curl_multi_init() 系列
来源：http://ho.shxzskj.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nd.wgjwhj.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yy.yuntaijiaju.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fp.shtwfgs.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wp.hahajie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cy.colortex.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ll.huixiangedu.cn

================================================================================
来源：http://zo.chemitech.net.cn

M. 命令行 / 进程 / 环境
来源：http://cr.muxihuayi.cn

================================================================================
来源：http://iu.newstarts.cn

[M01] 读取命令行参数
来源：http://tr.gzmigu.cn

Py:   sys.argv[1:]
来源：http://sa.huixiangedu.cn

PHP:  $argv;  $argc;
来源：http://nc.jianghongdianzi.cn

JS:   process.argv.slice(2)
来源：http://yn.shxzskj.cn

TS:   process.argv.slice(2)
来源：http://xl.hahajie.cn

Java: args 数组（main 方法参数）
来源：http://sw.yuexingan06.cn

Go:   os.Args[1:]
来源：http://wo.9csxet.cn

Ruby: ARGV
来源：http://wh.hahajie.cn

C#:   args 数组（Main 方法参数）
来源：http://uf.newstarts.cn

[M02] 读取环境变量
来源：http://qz.yuexingan06.cn

Py:   os.environ.get("HOME")
来源：http://hx.chemitech.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xe.huanxung.cn

JS:   process.env.HOME
来源：http://xh.jianghongdianzi.cn

TS:   process.env.HOME
来源：http://ka.muxihuayi.cn

Java: System.getenv("HOME")
来源：http://lx.shxzukj.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jj.gzmigu.cn

Ruby: ENV["HOME"]
来源：http://ap.yuntaijiaju.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sp.wgjwhj.cn

[M03] 执行外部命令
来源：http://fe.bookmarksfly.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dy.shxzukj.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ab.hnjuh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ph.shxzskj.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://of.chemitech.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://of.bjjhwx.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gb.chemitech.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ad.szsharing.cn

C#:   Process.Start("ls", "-l");
来源：http://js.haigaiapp.cn

[M04] 获取当前工作目录
来源：http://ih.shxzukj.cn

Py:   os.getcwd()
来源：http://yh.shtwfgs.cn

PHP:  getcwd();
来源：http://nb.nszjky.cn

JS:   process.cwd()
来源：http://wf.gzmigu.cn

TS:   process.cwd()
来源：http://su.521024.cn

Java: Path.of("").toAbsolutePath()
来源：http://nl.newstarts.cn

Go:   os.Getwd()
来源：http://va.shxzukj.cn

Ruby: Dir.pwd
来源：http://wy.huixinmuqiang.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fm.hahajie.cn

[M05] 设置退出码
来源：http://pa.jianghongdianzi.cn

Py:   sys.exit(1)
来源：http://uq.haigaiapp.cn

PHP:  exit(1);
来源：http://dy.hnjuh.cn

JS:   process.exit(1)
来源：http://vi.bjjhwx.cn

TS:   process.exit(1)
来源：http://lv.shxzskj.cn

Java: System.exit(1)
来源：http://nm.bjjhwx.cn

Go:   os.Exit(1)
来源：http://my.haigaiapp.cn

Ruby: exit 1
来源：http://jr.jctech888.com.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bq.asd995.cn

[M06] 向标准错误输出
来源：http://yl.panjiajie.cn

Py:   print("err", file=sys.stderr)
来源：http://pm.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dg.panjiajie.cn

JS:   console.error("err")
来源：http://cd.yuexingan06.cn

TS:   console.error("err")
来源：http://fw.yuexingan06.cn

Java: System.err.println("err")
来源：http://ed.huixiangedu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ti.9csxet.cn

Ruby: warn "err"
来源：http://cw.hnjuh.cn

C#:   Console.Error.WriteLine("err")
来源：http://yg.shxzukj.cn

[M07] 判断是否为主入口
来源：http://xb.bjjhwx.cn

Py:   if __name__ == "__main__":
来源：http://oe.asd995.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hu.bjjhwx.cn

JS:   require.main === module
来源：http://ow.haigaiapp.cn

TS:   require.main === module
来源：http://bc.jctech888.com.cn

Java: public static void main(String[] args)
来源：http://kq.jctech888.com.cn

Go:   func main()
来源：http://sv.shxzskj.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ko.shxzukj.cn

C#:   static void Main(string[] args)
来源：http://tf.huixiangedu.cn

[M08] 获取系统与运行时信息
来源：http://ni.chemitech.net.cn

Py:   platform.system();  platform.python_version()
来源：http://pj.wgjwhj.cn

PHP:  PHP_OS;  phpversion();
来源：http://zm.bookmarksfly.cn

JS:   process.platform;  process.version
来源：http://zj.bookmarksfly.cn

TS:   process.platform;  process.version
来源：http://wn.9csxet.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cu.jctech888.com.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yg.jianghongdianzi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jy.yuexingan06.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://im.jianghongdianzi.cn

================================================================================
来源：http://mv.hnjuh.cn

N. 数据结构与算法
来源：http://np.yuntaijiaju.cn

================================================================================
来源：http://dq.yuexingan06.cn

[N01] 二分查找（有序数组）
来源：http://vc.521024.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wr.huixinmuqiang.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ut.colortex.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qp.gzmigu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zy.nicolike.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ld.huanxung.cn

Go:   sort.SearchInts(arr, x)
来源：http://rs.szxytkj.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bm.lnxyls.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zt.9csxet.cn

[N02] 排序（工程实践用内置实现）
来源：http://tf.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://nc.yuexingan06.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qo.panjiajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sn.shtwfgs.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://if.yuntaijiaju.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://aq.9csxet.cn

Go:   slices.Sort(arr)
来源：http://vh.newstarts.cn

Ruby: arr.sort
来源：http://dl.yuexingan06.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bz.bjjhwx.cn

[N03] 快速排序（分治示例）
来源：http://fs.shxzskj.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hg.nszjky.cn

PHP:  // 递归实现，或用 usort
来源：http://pj.bookmarksfly.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zh.yuntaijiaju.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jo.colortex.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qn.lnxyls.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bt.nszjky.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bf.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zr.lnxyls.cn

[N04] 斐波那契数列
来源：http://pq.huixinmuqiang.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qa.asd995.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vx.gzmigu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lb.hnjuh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nm.szsharing.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gq.shtwfgs.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jk.jctech888.com.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fq.huanxung.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ym.shtwfgs.cn

[N05] 最大公约数
来源：http://vu.shxzskj.cn

Py:   math.gcd(a, b)
来源：http://cu.9csxet.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://po.gzmigu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://id.newstarts.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hg.nicolike.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ql.muxihuayi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vb.newstarts.cn

Ruby: a.gcd(b)
来源：http://pg.szxytkj.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://id.shxzskj.cn

[N06] 判断回文字符串
来源：http://fa.bookmarksfly.cn

Py:   s == s[::-1]
来源：http://jf.newstarts.cn

PHP:  $s === strrev($s);
来源：http://dr.nicolike.cn

JS:   s === [...s].reverse().join("")
来源：http://bs.yuexingan06.cn

TS:   s === [...s].reverse().join("")
来源：http://xb.huixinmuqiang.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sx.nicolike.cn

Go:   // 双指针从两端比较
来源：http://fi.yuntaijiaju.cn

Ruby: s == s.reverse
来源：http://gj.jctech888.com.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lg.colortex.cn

[N07] 两数之和（返回下标）
来源：http://lk.szsharing.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xj.wgjwhj.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://go.521024.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://js.hahajie.cn

TS:   // 手写 Map<string, number>
来源：http://rh.jianghongdianzi.cn

Java: // 手写 HashMap
来源：http://kd.jctech888.com.cn

Go:   // 手写 map[int]int
来源：http://ll.haigaiapp.cn

Ruby: // 手写 Hash
来源：http://ef.huanxung.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zi.nszjky.cn

[N08] 生成全排列
来源：http://nk.shxzukj.cn

Py:   itertools.permutations(arr)
来源：http://jb.huixinmuqiang.cn

PHP:  // 手写递归交换
来源：http://ia.jctech888.com.cn

JS:   // 手写回溯递归
来源：http://ts.9csxet.cn

TS:   // 手写回溯递归
来源：http://vn.hahajie.cn

Java: // 手写回溯递归
来源：http://rg.nszjky.cn

Go:   // 手写回溯递归
来源：http://ej.newstarts.cn

Ruby: arr.permutation.to_a
来源：http://qq.yuexingan06.cn

C#:   // 手写回溯递归
来源：http://dg.asd995.cn

[N09] 栈与队列
来源：http://wk.shxzukj.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qv.521024.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kc.muxihuayi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ju.hahajie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ef.yuexingan06.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bl.jctech888.com.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vm.bookmarksfly.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hf.yuexingan06.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zx.huixinmuqiang.cn

[N10] 链表节点定义
来源：http://ck.asd995.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wf.szxytkj.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://jp.nszjky.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fd.yuntaijiaju.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bk.jianghongdianzi.cn

Java: class Node { int v; Node next; }
来源：http://kw.szsharing.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jo.wgjwhj.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://jz.lnxyls.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eo.9csxet.cn

[N11] 二叉树中序遍历
来源：http://nj.shxzskj.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cs.521024.cn

PHP:  // 手写递归函数
来源：http://mi.hnjuh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://th.chemitech.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pf.shtwfgs.cn

Java: // 手写递归
来源：http://qr.nicolike.cn

Go:   // 手写递归
来源：http://op.hnjuh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dt.lnxyls.cn

C#:   // 手写递归
来源：http://vk.lnxyls.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qf.gzmigu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ja.lnxyls.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://su.9csxet.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gu.9csxet.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ba.shxzskj.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vv.huanxung.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://af.nicolike.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ia.wgjwhj.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xg.szsharing.cn

================================================================================
来源：http://ws.lnxyls.cn

O. 并发与异步
来源：http://tn.shxzskj.cn

================================================================================
来源：http://ps.jianghongdianzi.cn

[O01] 启动一个线程
来源：http://rs.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wj.panjiajie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yh.shxzskj.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cu.shxzskj.cn

TS:   // 同 JS
来源：http://mm.hnjuh.cn

Java: new Thread(() -> f()).start()
来源：http://am.wgjwhj.cn

Go:   go f()
来源：http://wx.shtwfgs.cn

Ruby: Thread.new { f }
来源：http://jz.panjiajie.cn

C#:   Task.Run(() => F());
来源：http://ce.521024.cn

[O02] 使用线程池
来源：http://zh.colortex.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://em.wgjwhj.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qv.newstarts.cn

JS:   // worker_threads 线程池
来源：http://be.shxzskj.cn

TS:   // worker_threads 线程池
来源：http://oa.panjiajie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pa.newstarts.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jn.lnxyls.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wx.huixinmuqiang.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ln.szsharing.cn

[O03] 加锁保护共享数据
来源：http://ut.asd995.cn

Py:   with lock: shared += 1
来源：http://vq.huixiangedu.cn

PHP:  // 用 flock() 做文件锁
来源：http://kd.hahajie.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fk.colortex.cn

TS:   // 同 JS
来源：http://gh.szsharing.cn

Java: synchronized (this) { shared++; }
来源：http://xn.wgjwhj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cb.colortex.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://co.shxzskj.cn

C#:   lock (gate) { shared++; }
来源：http://ho.gzmigu.cn

[O04] 定义异步函数并等待
来源：http://tc.9csxet.cn

Py:   async def f():⏎    await g()
来源：http://ez.jianghongdianzi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gv.shxzukj.cn

JS:   async function f() { await g(); }
来源：http://mw.huixinmuqiang.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tj.huanxung.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fn.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bi.szxytkj.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qb.huixiangedu.cn

C#:   async Task F() { await G(); }
来源：http://pc.chemitech.net.cn

[O05] 并发执行并等待全部完成
来源：http://at.huixinmuqiang.cn

Py:   asyncio.gather(*tasks)
来源：http://ds.lnxyls.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pt.521024.cn

JS:   await Promise.all(tasks)
来源：http://ac.muxihuayi.cn

TS:   await Promise.all(tasks)
来源：http://ga.panjiajie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tv.bookmarksfly.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bi.9csxet.cn

Ruby: threads.map(&:join)
来源：http://dn.gzmigu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gt.colortex.cn

[O06] 使用进程池
来源：http://jh.nszjky.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rl.hnjuh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qy.jianghongdianzi.cn

JS:   // child_process / cluster 模块
来源：http://ae.yuntaijiaju.cn

TS:   // child_process / cluster 模块
来源：http://eb.szxytkj.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uf.yuntaijiaju.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ep.521024.cn

Ruby: // fork 块
来源：http://jz.lnxyls.cn

C#:   Parallel.For
来源：http://kc.bookmarksfly.cn

================================================================================
来源：http://kt.bjjhwx.cn

P. 常用工具函数
来源：http://mg.wgjwhj.cn

================================================================================
来源：http://xi.gzmigu.cn


<!-- 参考信息 -->