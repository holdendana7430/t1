代发 wailian999

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/glgdvwvua.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gzoyxtulv.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gukyfrjan.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gllixijgq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gqretinus.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gwywjzkpd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/grotvwweo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gthteeigl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gnhofgqno.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gietxufba.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/ghiqknwra.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gjdfumsvn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gmxvxxojk.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gldvowcuf.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqsjcynzf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/ggfkbmfbg.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gduppkhhd.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gsrpmbvge.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gkvougsue.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gybhkspmy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gfjhfjqgi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmrnzrxjq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gktkjkmxo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gqnysuhsr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvsethhz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gdkqdlrfe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyxbjzuyn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gkflyamxb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcagcuvif.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gdfktysyl.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gojetbskt.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gbkawkkyx.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gdcrnfppa.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gcxsbcbbo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gbltcyrhg.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gmmkyqnmm.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gilcchxgv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/grgestvfv.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gdqkffbin.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/ggfsqprgn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gzuliyxqa.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxiklnzen.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gsegguawq.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gplqwpins.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghoflbeoi.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gmmpzahyf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gbjakjjjr.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gxwvguoaz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gsobfzjxl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gyxhmlooq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gelcbucxm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/ghyugwgfx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/glthgcmnn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gndnrvutw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gfpmbrhao.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gqerakthz.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gurcudyvd.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/glvpdtknk.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gafmdhtgs.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/ghcynkske.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gkmwzskht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ghwcjubvw.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gcuxzgzhv.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gdtokvmrw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gfypwxdqo.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gqoqzxpdm.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqxbviaoi.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gippukpbf.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggpbenvce.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guxagtjek.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyjezylol.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gbspcviev.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gxcxcroxx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gidklgsqt.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gbzlsqiia.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gzunzcuub.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gzcchfnwn.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gzvcuqoqz.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gqmsjxjyu.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gavdwjdoi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gofybmlaa.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/geeqbwire.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwkoyhwv.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gfhrmvxbf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gatcqqxmf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gzjzuekne.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/grlekcvtj.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gffxqwcfn.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gzzcukiiy.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gvrgrqrcg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gnzsjjwdn.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gegtgbwnh.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/grsbycifi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gqctylshr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gepkybpeq.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gubrrwpsu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gkluwbhsh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gymkrcdko.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gnsmhvefe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gjyicynxb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gkcqzxaga.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gstexnlmk.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gjdboucdd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gicsvzzgn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gobssxffp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gqnwnrdob.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gyugqbcam.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grqinrbyk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gbifxrfcd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gqjjvhbtk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkiktoh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gezgdlcjr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gncylonmq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gbqhquyme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gcnlijsmu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gtopvylzs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxfnzopho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gzhgytgwl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/gknsrypxc.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gzshjyeuv.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/goppuahhy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/ggtiryrhq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gpuultiaf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/ggaexzmzk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gcozwxoij.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/ghexcwsop.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/giqingyfs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gjltvkdda.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gcdbrturd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gtytejmbd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gmbuvqjtw.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gupdudvzg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghmwivifs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gpgaxxtyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gsdkzemyj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/grjgqkkbq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/goowawdxx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gjjtaevia.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gptaygnmw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gmwusqsbh.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gfftyiptk.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gfivemyak.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gmswwntie.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gmxvwpruc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gsuqpsfxd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/grnpyossj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gwlvijask.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/girmfhymz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpcaoraj.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gryrtqopy.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gpveiqiiy.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gwejwbdxc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gwszztoed.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gafohgysn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gnkjfvjrp.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gxjmkhppl.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gawmpbcta.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gizicbfxg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gqzzasbwi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gndboprut.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gqeghggik.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gdjapmpej.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gfzhuaved.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gbljnpgvr.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gvxgxzdwp.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/grhorpmks.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gybpyjrqu.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/ghqursaqb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glbkcpoau.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gvhjyjkth.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gnqohnmkn.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gbnnzixku.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gtbvlzbyo.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gajmfqpyu.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gantujenb.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghqzokhql.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gtdlcmugb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gntitgymq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gnmiyeopu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gxyzageai.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.hesvh.cn/Article/details/gmwvsmgef.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gziwzpeqo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/gohinmqkc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/grqbwoctl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grrgnjvpj.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gcqwetage.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fehbvm.com/Article/details/gjiscvtug.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gdooznwca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gmvjmtjzt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/golclnanf.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gioylguty.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ghsdeaqsj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gcpvaxvub.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/guvveqwut.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gisktetft.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gxpdqktal.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gdabjdnvt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gbrlbakbh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gimonylkg.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/givrrwdmd.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gxbhvnrxn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gpkegvuld.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxojtrjyy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fehbvm.com/Article/details/gdpyacani.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gptuycvuu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gdoorhgba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gkizkdjfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gnoztufxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gzviimuza.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/ghfdolbvm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gfpdkchvp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggveztzdf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gieehkdhu.sHtML

O. 并发与异步
来源：http://www.m.share.fehbvm.com/Article/details/glxdyebws.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guyxkghyk.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gqorhixls.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gbpajbrsp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gmjrxcehv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gsyjqfdfn.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gxirezuxx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gdihfqods.sHtML

Go:   go f()
来源：http://mobile.hesvh.cn/Article/details/gciborfmy.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfsxucce.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gmmmycprj.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gqedaarmw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gjhvzzibd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/guhzazfdo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/getnscvwv.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gmcjitxyl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gajhtlkju.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gorwxwexu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gjeetskck.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gvyzlgpgr.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gnpomrtxf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gopmamvqb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gtnnceqqt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gpaxkdekr.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gbdaepboe.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gehelteln.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gqdqrfsci.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gtfhhjhhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/giifveuzz.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/geauargza.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gwjgxzhkf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.hesvh.cn/Article/details/gwbqcqzkw.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gqjbfmgdl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gcmmdiczh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gzseydklw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gknvdaosu.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gqvdwqfih.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gkrnwvrpw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gfsxtzwzy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/glkjcpnqs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gfbrigcdy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/ghwhgcxup.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gwplquxic.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.hesvh.cn/Article/details/gqjxueduf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gowdqopjz.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/gddxkwnxa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gojmdugef.sHtML

[O06] 使用进程池
来源：http://m.share.hesvh.cn/Article/details/gkvflwfvw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gsapqcblq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gbwhxbdxq.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gyczzzojl.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gkkfexmrp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gfzmzrsdd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/giezewcwa.sHtML

Ruby: // fork 块
来源：http://mobile.hesvh.cn/Article/details/gwboiwvub.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/glltfkgjz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbawidpis.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gfjqmyoos.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghovnlnxf.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gablezlme.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gftigfdfa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.fehbvm.com/Article/details/gtadzzxys.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/grrmkozyi.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gfsbygmtw.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gqjznlasv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gviejllec.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gfmuudniu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/grvfwzake.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gxbdkcqmj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gzzibbgfy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gfgclijuc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/gsolxoyju.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gickkival.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gcvkxedhq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/ghaonotxt.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gczxkgops.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gyouyxads.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/gkfwsewes.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gxnbvaqzu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fehbvm.com/Article/details/gyrxzeyme.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/ghhdzmltb.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/glpojeqdz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gmtkgwmom.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gkjnfklkt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gqcjpavnk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gjqpoowbb.sHtML

[P04] 求长度
来源：http://mobile.fehbvm.com/Article/details/gctkymmfj.sHtML


<!-- 参考信息 -->