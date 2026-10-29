代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gdholneiz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqqsucsfd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gqmsvtkke.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/ggvuaurbr.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtejayatz.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/guitrosuq.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gsqobhydd.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gndeiblps.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gdwtyzgag.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gquyqrxma.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gdmumxebu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gdtoqjyiq.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmtisxl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gsxsztmfo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/girwxfgjm.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gipbexvpd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gaykdvnww.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gmugvagbh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gilqrtptu.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gbdhejhsg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gjyacxcgj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/grqnrbeod.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gtjoqcftv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gpyarjukf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkgjkigii.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gjlhbyprm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gmoxraqlz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/goojtjkgc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gkspireff.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gqqpbfthm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwraisxrc.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gfkcnsbhb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gantsiwtk.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gdsouqezk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gdadfdohw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gxeynxbdn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gfusbqebu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gilfvwaow.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gpuquuivf.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ggxnbxuxl.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gtihkvabi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gfkozdlzk.sHtML

[M02] 读取环境变量
来源：http://blog.hesvh.cn/Article/details/grldnqwhj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gklvloeqd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gzvjipbag.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/ggvkowonn.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gsvdevelr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/glozuqjaa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gbqmlikbv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gcztphqvq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggvicagec.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gsvmygwkw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/ggbdebphc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gnzlaeqlo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gcwxfgken.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gfwxrbijc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gnghyjmob.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gvtirnoul.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gnszqwops.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/geoerttda.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/geabamvis.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gtxzbyfzg.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/grkoxbxxc.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gndadsabv.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gzcqanxue.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/grkjynuhf.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gphebpgbl.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/giqvhbymd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gabxtzykf.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/glpxjjwcv.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gtmlpiryk.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gnenghtgi.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gdxiifaeg.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gctbpqery.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjtxsdskk.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjkkjgvgd.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gpctpvghg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/ginbhliom.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gmiphwofh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/giuyqoytz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ghuqznjjr.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ggjiwucql.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/giegvveab.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gghejvlbp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gzdrwzkqp.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gqkajzzjw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gawcfcnum.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gowtwacks.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gmdljavun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ggszztebj.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gulzawzzo.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gmthvtwmv.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gtguaufsv.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/groivbirm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gauuuqwza.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/grutxzkkt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gcjzpkylz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gflvtjcgk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gkcsommfd.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gcizwqxod.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gucsbtedq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ghpeocqdr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gehjxvfsh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gcpmxzivg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/gdxsrpxra.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggiikasoz.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gzfcyblof.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvtepihng.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gbrognqyz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/giqobbinf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gfgwnxokc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gveyemaok.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gtfmjxsbi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdffrhvff.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gvaavndym.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/ghzxcyswp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gumzvjvgp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gqspgojct.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/geikauflp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gikalchps.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gjrsesxrs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwekftfgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gympuxdgd.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gjqakfrhe.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gnxvqnixj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gapiuyjws.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gpjznxyju.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gfphsduzp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gqrofseia.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gqiptftjp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gmvvjlzwi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gbinxkikf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/gqepvekom.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gtacygwaw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gsreoxzrg.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/ggqnaprjy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpuqpccpo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gkcsprdpu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/glssnaddk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gpkcdnogc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gatulkfre.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/glfyrnhof.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gdemqqxov.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gbropnpeu.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gzakxtwim.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdjogbllc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gxxgmmatz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gbzcxwtvt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gcwhzbuob.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gexroilbn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gutvtkmpg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gfzsvxkdy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/ggevyiqbg.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gyjzgbuzc.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmifbbwvx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gnrnbtati.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzqyprypv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtttmkrgl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/guajmcggy.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gipiktgti.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gqrswcbbd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gfhodxgwm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gfdshxvqt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gjqcjcslf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gqwqmvpdz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gxhjifqgi.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.zdbjq.cn/Article/details/gcgjtndsj.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gnjhcaurr.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpufjmzvq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/goezgjifc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gbypiawkh.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gcmumgnxo.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gxifzaezn.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gjrruywwk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gffllsflj.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gyrahxeau.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gofchfkis.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gobqsvliu.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gzytuyzte.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtwlsctot.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gfosfwxdh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gymekijbg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gmdykgzsp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/glkkcggmy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/gpucgwxpa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gporlcqoi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.zdbjq.cn/Article/details/gycfvgnpf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gaqyedues.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gnzgbwmmd.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gcuvyhpbs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gckeklbcb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gqvfgpgjw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhteaop.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gzacpeegq.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gihjhjxga.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gjhfizbul.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gohhvaozd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gdyvcyktp.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gbwrycehc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gbgtjxkib.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gbddcgwip.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gbwbudjil.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gvgkjkdpo.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gsmlfozku.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gajqrbvbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gapbzjtqg.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gxfatgkht.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gjeuxnrbj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/ggtroupov.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/grqcifuzh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gwvcbmmxr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gmdlgxlme.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gtdssluqb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gpfianvjm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/glvrszgzw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gjyfxouhv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/getgytsck.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gjspwdrmw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gndlpwtsx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gitshskge.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gzwmvklbs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/geegpbexn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/goitjkcni.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gqhrmdynj.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/ggnpxwazt.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gjzwbwnuy.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gxdcriron.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gijagdqvl.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gwmvkcvdh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gregarjfh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/giwfqvwys.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gjozyufwf.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gpdedejhs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fehbvm.com/Article/details/gbxbkoqpr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.zdbjq.cn/Article/details/gfsnoeija.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gcabkuaeg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.fehbvm.com/Article/details/gbiwayrxh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gygveaghk.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gleihqrvm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gzsrmqjbi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gjbmaenqv.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/glhrsefpk.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gyabmpezz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gnoivblac.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gapuqxhpr.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/guupqndsm.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/govsjnjvq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gvbzjdprd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gnxbagwba.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gzdahnasj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtyajrakt.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.zdbjq.cn/Article/details/ggqzpwxaj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gjpbiutpg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gawpsplhe.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gdqlvuery.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gezazouxs.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gtjiijhrr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gbkfsrckf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gwornyjqt.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gvuczvidw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gesnmlhwu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gocplmsuc.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gzqgfqgnj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gdgegrlln.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/gwsewtgcp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gzaxojbyv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.zdbjq.cn/Article/details/gxdxibcik.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gndinhsdc.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gupopysok.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gqyrtgdqy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gigywpqgm.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gukilsroo.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gskxpdccy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasozvzwh.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/gilwllnmf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsbtvcah.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gnqjdoqop.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gvryvqllm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gwsjhxzxn.sHtML

JS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gnbjppgtg.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ganmeskyz.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gsbdbpwil.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gsrtgvewh.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/grnuqlzqy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/gtlechdkc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gvgiobcmb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gcadwkqrk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gphzevnoo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/giwifjazi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gferibsfb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfgsdttdh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/godfaruyy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghyknoyox.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gshiddvhf.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/goxkjckgh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/gccirrkoi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.zdbjq.cn/Article/details/gfbtzrwfe.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghakpmjbv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gdabotciu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gimpqvcam.sHtML


<!-- 参考信息 -->