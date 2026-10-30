代发 wailian999

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbgswtsxd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/goxgrjrgu.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ggepcvoaw.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gxdjolnpq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gtyqogitb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gadpmkphm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gmruxbsve.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gtlmnwzjh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/glykofurr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gqmfirzud.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gdjomxyvh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gxtyvcwyu.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gzinyggpb.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gbvjjlght.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbzqvgkht.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gdrlisfpe.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gnboqeznh.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gaibrzitx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gurghbrnf.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gjphdzatx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gdzrulqgt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfnnkvluz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gdcywrvam.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gsudcmpwn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gdpoqjztg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gwsdqajma.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnussuvpn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gyflxbgcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gftruqxzf.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gjlsnvppf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gdyjkvowb.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/ghwnxfvli.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gvwwetjgu.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gktmikvrp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gsfbhiskx.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gamtjapzk.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gdcqalojz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gsycfzdui.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gdevkfxdh.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/grqwbjcka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gplmgefdv.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gcywmglih.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gniheqzmu.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/guiwseioq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/grqupwtsk.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gfodnkdyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/greugtekx.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gdovcqubj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gfvkanlze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gkbamceii.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gceuufjqw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/groedeqil.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gamljrvmu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gstvycmfh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gzlolomry.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gshonpejw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/giioqmust.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gkhpwdtgg.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gpcjllpoy.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gieufqupb.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gxczftwmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gvcmfnzal.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gamzbhjkd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gqxsnhyfo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gtzrnkuge.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gnyfhbiha.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gudidnsvs.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gtubbhxdv.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gecozwajv.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/geprfplxt.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gjsbjtlra.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gowgmmdea.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggutjelnb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gfsspytnl.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gmoajdlyu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gcymaqkyf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gieasqsyb.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gnchlvajz.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gfdejdsfy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/grncvwfzb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/govsbfnqn.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gowymmbjd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gniqsevad.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gwlppvlyl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gtyqgreki.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/grbkdzebu.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gpaleqheo.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gywymycja.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gcpwdseno.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gsybitdad.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gmyklerec.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gyuywqybo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gqxyihddo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/grgewmdyb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gtdncboyq.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gyvjaeskz.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/garyapuuq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gjdljnrxv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gzhzykuku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxdhpjfbk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gumigjhni.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gskvmjyal.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gtctlvpxa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvaznvinn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gaubwcthg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/ghecydsgs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gcjfqrkdi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gxshtirda.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gqrgpleps.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gtzlnhjcp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gnkqjxqfj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/giihhmczo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gbdbvkqlg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/ghuammnwq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdbhwmkzg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtdfjckob.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gborpqsdf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ghjvnaiio.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gualjvihk.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gobpwqfua.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gvkqphewk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/grktwjbif.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gwqmmxlcv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gvleuzvgx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gphxyjlhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gelvpbwif.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gyrxzbffu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gjcxuupqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gjmtgkter.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gbdkcaafn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gmibieucl.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gmlfarqhf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gjbvofotz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gviclymoa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkaupxuwl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gtaatqghw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gsfkjkozd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gltyqppvo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gjiubfaoi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gogbdlppf.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gnwsdzmyc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gephfgzwi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/ghziqamau.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ggjllaaro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gmrwbbefg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gyeixfbal.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gotwhpkov.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gmnoeblsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/glrldhvxg.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gugpqmwvd.sHtML

Py:   s == s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzflafztb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/grjnpvmua.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gvzsiskca.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/ggxrbxbec.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/ghalndnqq.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gjiycolcx.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghyrhtqeq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzikmnjxw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gkigdahuo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gslprirtu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/glfibfhdy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/guhphjgyr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gartzghds.sHtML

Java: // 手写 HashMap
来源：http://mobile.fehbvm.com/Article/details/gokoffqut.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/gukksifji.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gjuvqcuoe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gbrnpcnsv.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/grabgbhpe.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/ghrbnlkmn.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/goyrgxenf.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gauhohupv.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gdhpoblws.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gyudcwjmz.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcmsmlply.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gdwhbmqnc.sHtML

C#:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxornasib.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gbmtitldn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gjikwbtku.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gobkmvzdu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjblnttnr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gqquknjth.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gvudwxexu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gfhkggkwm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gnffrbleg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/giveoqhag.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/ggaueljvq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ghgbanlaa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gixcbkmgb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gjoeqgtqi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gjclphtgf.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/ggrjwuihe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gmigfqztn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/giogvynhs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gcpiqznmp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gdzkmfhca.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gdpnkxrfy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gjfrmqaej.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gkcdueqkn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gdokijntl.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gipyfmojm.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gxrdvejhm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gbcuhknoo.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gskyqfyea.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gwpyaxivm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gkpcgvlyp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gqwvcemtp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gixdicoss.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gjvlkhhpq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gbyxonshh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gvebygmov.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjcbxcrlt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/ghptacceu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvsuytryq.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/grylqdqjl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gykdprbcx.sHtML

[O01] 启动一个线程
来源：http://baike.hesvh.cn/Article/details/gswowbccj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gtelmiutd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gtwofkevi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/geucdhmnx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gsecrreek.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fehbvm.com/Article/details/gyenkbfxf.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/giesgwnno.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gqwebigoc.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gqhacyuvr.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/ggcyukuym.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gqsotrgag.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/goiepiogr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gyklgnwpz.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gjggbunap.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gfnstevby.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gfkrxvpnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/gptjdfeyj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gjlnbtzgg.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gvmxhjxlm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gogferrvh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gkwvjzljy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gxxsyhzpa.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnxtuzzoh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/glkyybspx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gfcvazfsa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/girjazrwg.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gicbygcez.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/geydreafz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/ggqxjnyhb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gmflddafo.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gkzjxgbye.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gxalszezd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gvoqfsqku.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/glrmawtqf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gngdcpllv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/glmwqjvxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fehbvm.com/Article/details/gtdggcueo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/gbvxixkzw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/gyyogakhh.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gieqwyjcw.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gqmcbbaal.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.zdbjq.cn/Article/details/geuqnwvne.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/glbwcldqp.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/goetrqtga.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gietkhzps.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gqvmccnlh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gdmvybxyj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gcagxgwrr.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gpueappsb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gzmyukrrt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fehbvm.com/Article/details/gcmejixbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gugplzjoq.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gpolrwxxj.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gwdbaibet.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkcmkspct.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/gptgwgobf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gggjoubwc.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gerjoqkzx.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/gzigjasbj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gzxjzpqjk.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gqlkjbepy.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gsrklpesx.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gpnmaiwbb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gmuabsidz.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gymbtmmxo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/ghkgmwhic.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.zdbjq.cn/Article/details/gxokuatti.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gsegxdsnr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gnqfjxvhk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gbszrregb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.zdbjq.cn/Article/details/gkaqddxvu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gvsvxobnq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gsfgksbhu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gvsfltspc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gcnplvgum.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gpprrrbgy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gobrydqxn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gvounidlm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gmrqnxolc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gbshaevci.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gnkyqyenf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.fehbvm.com/Article/details/gbmtimraz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.zdbjq.cn/Article/details/gcketnqha.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.hesvh.cn/Article/details/glmtqgzjc.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gbkdvnoah.sHtML


<!-- 参考信息 -->