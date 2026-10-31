代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ib.huixiangedu.cn

JS:   await fetch(url)
来源：http://nb.hnjuh.cn

TS:   await fetch(url)
来源：http://ux.huixiangedu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://si.hahajie.cn

Go:   resp, err := http.Get(url)
来源：http://fo.haigaiapp.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://lq.lnxyls.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uz.jctech888.com.cn

[L02] 发送 POST JSON
来源：http://um.jctech888.com.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vq.hahajie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uz.yuntaijiaju.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ak.huanxung.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kv.9csxet.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ro.hnjuh.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://iu.lnxyls.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cv.hahajie.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ku.lnxyls.cn

[L03] 设置自定义请求头
来源：http://ng.panjiajie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hr.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dn.hahajie.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oa.shtwfgs.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fz.yuntaijiaju.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yq.asd995.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rg.hnjuh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pf.wgjwhj.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jb.chemitech.net.cn

[L04] 设置超时
来源：http://ed.asd995.cn

Py:   requests.get(url, timeout=5)
来源：http://gl.9csxet.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tx.huanxung.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wg.shtwfgs.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lf.shxzskj.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zu.gzmigu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rc.colortex.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fr.lnxyls.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qu.yuntaijiaju.cn

[L05] 上传文件（multipart）
来源：http://zr.521024.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yg.newstarts.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gm.newstarts.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ru.wgjwhj.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://di.bjjhwx.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://me.asd995.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xw.shtwfgs.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pf.yuexingan06.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hr.yuexingan06.cn

[L06] 解析响应为 JSON
来源：http://ei.shtwfgs.cn

Py:   resp.json()
来源：http://ld.chemitech.net.cn

PHP:  json_decode($body, true);
来源：http://ov.jctech888.com.cn

JS:   await resp.json()
来源：http://ym.hnjuh.cn

TS:   await resp.json()
来源：http://cc.muxihuayi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ch.bjjhwx.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gl.chemitech.net.cn

Ruby: JSON.parse(resp.body)
来源：http://li.nszjky.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ue.jianghongdianzi.cn

[L07] 处理 HTTP 状态码
来源：http://co.9csxet.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://yw.nszjky.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://js.hnjuh.cn

JS:   resp.ok;  resp.status
来源：http://se.gzmigu.cn

TS:   resp.ok;  resp.status
来源：http://ok.muxihuayi.cn

Java: resp.statusCode()
来源：http://li.lnxyls.cn

Go:   resp.StatusCode
来源：http://vs.gzmigu.cn

Ruby: resp.code.to_i
来源：http://fk.szsharing.cn

C#:   (int)resp.StatusCode
来源：http://em.hahajie.cn

[L08] 并发请求多个地址
来源：http://qy.huixinmuqiang.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ky.newstarts.cn

PHP:  curl_multi_init() 系列
来源：http://mp.yuexingan06.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hq.9csxet.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aj.bookmarksfly.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://fg.muxihuayi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lu.szsharing.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ur.wgjwhj.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bu.huixiangedu.cn

================================================================================
来源：http://ma.yuexingan06.cn

M. 命令行 / 进程 / 环境
来源：http://jn.huixinmuqiang.cn

================================================================================
来源：http://jh.hahajie.cn

[M01] 读取命令行参数
来源：http://nb.bookmarksfly.cn

Py:   sys.argv[1:]
来源：http://sr.asd995.cn

PHP:  $argv;  $argc;
来源：http://sj.chemitech.net.cn

JS:   process.argv.slice(2)
来源：http://tz.huixinmuqiang.cn

TS:   process.argv.slice(2)
来源：http://an.jianghongdianzi.cn

Java: args 数组（main 方法参数）
来源：http://je.9csxet.cn

Go:   os.Args[1:]
来源：http://gu.hahajie.cn

Ruby: ARGV
来源：http://kh.9csxet.cn

C#:   args 数组（Main 方法参数）
来源：http://qn.szsharing.cn

[M02] 读取环境变量
来源：http://cd.shxzukj.cn

Py:   os.environ.get("HOME")
来源：http://uf.bookmarksfly.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eq.newstarts.cn

JS:   process.env.HOME
来源：http://wp.huanxung.cn

TS:   process.env.HOME
来源：http://ly.shxzskj.cn

Java: System.getenv("HOME")
来源：http://nl.nicolike.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uv.panjiajie.cn

Ruby: ENV["HOME"]
来源：http://oa.colortex.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nc.hnjuh.cn

[M03] 执行外部命令
来源：http://cg.panjiajie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vd.nicolike.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zv.9csxet.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://va.szsharing.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tx.jianghongdianzi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yq.haigaiapp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://cy.shxzskj.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lj.huixinmuqiang.cn

C#:   Process.Start("ls", "-l");
来源：http://cl.hahajie.cn

[M04] 获取当前工作目录
来源：http://qa.muxihuayi.cn

Py:   os.getcwd()
来源：http://tr.lnxyls.cn

PHP:  getcwd();
来源：http://qx.szsharing.cn

JS:   process.cwd()
来源：http://bd.nicolike.cn

TS:   process.cwd()
来源：http://xz.muxihuayi.cn

Java: Path.of("").toAbsolutePath()
来源：http://sh.haigaiapp.cn

Go:   os.Getwd()
来源：http://op.panjiajie.cn

Ruby: Dir.pwd
来源：http://ll.bjjhwx.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nj.gzmigu.cn

[M05] 设置退出码
来源：http://zc.muxihuayi.cn

Py:   sys.exit(1)
来源：http://zp.szsharing.cn

PHP:  exit(1);
来源：http://bt.9csxet.cn

JS:   process.exit(1)
来源：http://cg.521024.cn

TS:   process.exit(1)
来源：http://tl.521024.cn

Java: System.exit(1)
来源：http://mk.lnxyls.cn

Go:   os.Exit(1)
来源：http://as.hahajie.cn

Ruby: exit 1
来源：http://ia.asd995.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uf.bjjhwx.cn

[M06] 向标准错误输出
来源：http://bv.newstarts.cn

Py:   print("err", file=sys.stderr)
来源：http://ka.hahajie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zt.nszjky.cn

JS:   console.error("err")
来源：http://er.jctech888.com.cn

TS:   console.error("err")
来源：http://re.yuexingan06.cn

Java: System.err.println("err")
来源：http://zl.panjiajie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hs.asd995.cn

Ruby: warn "err"
来源：http://rd.huixinmuqiang.cn

C#:   Console.Error.WriteLine("err")
来源：http://tc.szsharing.cn

[M07] 判断是否为主入口
来源：http://tp.chemitech.net.cn

Py:   if __name__ == "__main__":
来源：http://ie.szxytkj.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kl.wgjwhj.cn

JS:   require.main === module
来源：http://di.haigaiapp.cn

TS:   require.main === module
来源：http://jn.gzmigu.cn

Java: public static void main(String[] args)
来源：http://pn.521024.cn

Go:   func main()
来源：http://ry.chemitech.net.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yx.panjiajie.cn

C#:   static void Main(string[] args)
来源：http://xl.521024.cn

[M08] 获取系统与运行时信息
来源：http://lw.hnjuh.cn

Py:   platform.system();  platform.python_version()
来源：http://jd.shxzskj.cn

PHP:  PHP_OS;  phpversion();
来源：http://zb.huixiangedu.cn

JS:   process.platform;  process.version
来源：http://uu.muxihuayi.cn

TS:   process.platform;  process.version
来源：http://dv.newstarts.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uv.huixinmuqiang.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://do.yuexingan06.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dm.huanxung.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nh.huixiangedu.cn

================================================================================
来源：http://hd.muxihuayi.cn

N. 数据结构与算法
来源：http://vh.huixinmuqiang.cn

================================================================================
来源：http://gq.asd995.cn

[N01] 二分查找（有序数组）
来源：http://kx.panjiajie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hf.shtwfgs.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xz.newstarts.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xd.newstarts.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ma.jctech888.com.cn

Java: Arrays.binarySearch(arr, x)
来源：http://by.521024.cn

Go:   sort.SearchInts(arr, x)
来源：http://jh.huixiangedu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sj.szsharing.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ov.szxytkj.cn

[N02] 排序（工程实践用内置实现）
来源：http://rm.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://lv.gzmigu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vq.hahajie.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mg.jianghongdianzi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sk.haigaiapp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xz.521024.cn

Go:   slices.Sort(arr)
来源：http://uu.nicolike.cn

Ruby: arr.sort
来源：http://on.colortex.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://sd.shtwfgs.cn

[N03] 快速排序（分治示例）
来源：http://jd.nszjky.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gw.colortex.cn

PHP:  // 递归实现，或用 usort
来源：http://db.gzmigu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mo.shxzskj.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sa.shxzukj.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tg.jctech888.com.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gm.colortex.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hr.colortex.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vz.colortex.cn

[N04] 斐波那契数列
来源：http://lf.nszjky.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eg.colortex.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://az.chemitech.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://up.521024.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://it.jctech888.com.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mi.panjiajie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://an.yuntaijiaju.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pq.bjjhwx.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nn.huixiangedu.cn

[N05] 最大公约数
来源：http://sp.huixiangedu.cn

Py:   math.gcd(a, b)
来源：http://mk.szsharing.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zm.shxzukj.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ti.wgjwhj.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mz.asd995.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ch.huixinmuqiang.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uz.jctech888.com.cn

Ruby: a.gcd(b)
来源：http://tn.9csxet.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zh.chemitech.net.cn

[N06] 判断回文字符串
来源：http://ym.newstarts.cn

Py:   s == s[::-1]
来源：http://vb.haigaiapp.cn

PHP:  $s === strrev($s);
来源：http://ek.shxzukj.cn

JS:   s === [...s].reverse().join("")
来源：http://mz.newstarts.cn

TS:   s === [...s].reverse().join("")
来源：http://jx.panjiajie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lo.szsharing.cn

Go:   // 双指针从两端比较
来源：http://zg.jctech888.com.cn

Ruby: s == s.reverse
来源：http://ct.jianghongdianzi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://co.lnxyls.cn

[N07] 两数之和（返回下标）
来源：http://yb.chemitech.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gg.gzmigu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mc.szsharing.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pu.yuntaijiaju.cn

TS:   // 手写 Map<string, number>
来源：http://bg.521024.cn

Java: // 手写 HashMap
来源：http://ew.bookmarksfly.cn

Go:   // 手写 map[int]int
来源：http://iu.newstarts.cn

Ruby: // 手写 Hash
来源：http://qy.9csxet.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ax.bookmarksfly.cn

[N08] 生成全排列
来源：http://pg.muxihuayi.cn

Py:   itertools.permutations(arr)
来源：http://ig.jctech888.com.cn

PHP:  // 手写递归交换
来源：http://co.9csxet.cn

JS:   // 手写回溯递归
来源：http://xn.bookmarksfly.cn

TS:   // 手写回溯递归
来源：http://bz.wgjwhj.cn

Java: // 手写回溯递归
来源：http://ex.shxzukj.cn

Go:   // 手写回溯递归
来源：http://rh.muxihuayi.cn

Ruby: arr.permutation.to_a
来源：http://do.shtwfgs.cn

C#:   // 手写回溯递归
来源：http://nj.yuntaijiaju.cn

[N09] 栈与队列
来源：http://ed.nicolike.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wc.hnjuh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gl.shxzskj.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sf.jctech888.com.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xt.bjjhwx.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sc.huixiangedu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ap.bjjhwx.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ic.hnjuh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fs.bjjhwx.cn

[N10] 链表节点定义
来源：http://yx.newstarts.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://or.521024.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qt.newstarts.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://sf.muxihuayi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ky.szxytkj.cn

Java: class Node { int v; Node next; }
来源：http://yn.panjiajie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yv.lnxyls.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://aw.chemitech.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jf.jianghongdianzi.cn

[N11] 二叉树中序遍历
来源：http://kf.muxihuayi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tf.haigaiapp.cn

PHP:  // 手写递归函数
来源：http://zc.haigaiapp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ce.nszjky.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tl.521024.cn

Java: // 手写递归
来源：http://vj.haigaiapp.cn

Go:   // 手写递归
来源：http://el.chemitech.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cc.haigaiapp.cn

C#:   // 手写递归
来源：http://ce.bookmarksfly.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ok.jianghongdianzi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ts.szsharing.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://au.colortex.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xh.hnjuh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bm.panjiajie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hg.yuexingan06.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ap.szsharing.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rj.panjiajie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nb.hnjuh.cn

================================================================================
来源：http://kc.shxzukj.cn

O. 并发与异步
来源：http://nj.huanxung.cn

================================================================================
来源：http://fu.lnxyls.cn

[O01] 启动一个线程
来源：http://di.yuntaijiaju.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cv.jctech888.com.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://og.colortex.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lh.szxytkj.cn

TS:   // 同 JS
来源：http://su.shxzukj.cn

Java: new Thread(() -> f()).start()
来源：http://qy.hnjuh.cn

Go:   go f()
来源：http://ri.bjjhwx.cn

Ruby: Thread.new { f }
来源：http://bo.bookmarksfly.cn

C#:   Task.Run(() => F());
来源：http://if.shxzukj.cn

[O02] 使用线程池
来源：http://nc.hnjuh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wt.bjjhwx.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zq.hnjuh.cn

JS:   // worker_threads 线程池
来源：http://ax.lnxyls.cn

TS:   // worker_threads 线程池
来源：http://je.huixiangedu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ts.yuexingan06.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ho.9csxet.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gi.yuexingan06.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ky.huixinmuqiang.cn

[O03] 加锁保护共享数据
来源：http://th.wgjwhj.cn

Py:   with lock: shared += 1
来源：http://zs.shxzskj.cn

PHP:  // 用 flock() 做文件锁
来源：http://af.521024.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nf.newstarts.cn

TS:   // 同 JS
来源：http://tk.muxihuayi.cn

Java: synchronized (this) { shared++; }
来源：http://vj.szxytkj.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xl.hnjuh.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://um.521024.cn

C#:   lock (gate) { shared++; }
来源：http://mo.lnxyls.cn

[O04] 定义异步函数并等待
来源：http://op.szxytkj.cn

Py:   async def f():⏎    await g()
来源：http://ad.521024.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fs.szsharing.cn

JS:   async function f() { await g(); }
来源：http://bo.nszjky.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pl.hahajie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nn.huanxung.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ec.panjiajie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oa.panjiajie.cn

C#:   async Task F() { await G(); }
来源：http://lu.hahajie.cn

[O05] 并发执行并等待全部完成
来源：http://os.newstarts.cn

Py:   asyncio.gather(*tasks)
来源：http://bz.muxihuayi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mk.muxihuayi.cn

JS:   await Promise.all(tasks)
来源：http://tj.huixinmuqiang.cn

TS:   await Promise.all(tasks)
来源：http://fa.nicolike.cn


<!-- 参考信息 -->