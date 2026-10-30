代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gmngxwfpg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gnxwssmkg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/ggwupuflb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gqlhpxwek.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/ggpqsbxdz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gaufmrhcw.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gdbwtfhpt.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gptmgawlq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gwkkdwzgb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gaazzsfzm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gmnxarkyu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gcwekhymw.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gebwrhnnv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gcxstfnaa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gvqpbvymm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/glhctbnus.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gdnuvkyiz.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gizjwktve.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyfkxwmvn.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gkapamnip.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxwxufhjx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gasvnegvg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gmmjmpehr.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/grlpkofbh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gtqreayyp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gklfaxvne.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gzxtmpkhg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gnkubtxgz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ghqnkqcfi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/giljdgmus.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gepcyalcp.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gitvwzztk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwqjczoru.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gwktjbanx.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gzvmwqcjj.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gglwotvas.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gauekgjhy.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gaeirfocm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gimanxpih.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gjrvsxkkp.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gckmyxbfo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/geszxwrkj.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gbaoibspu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gkqgnimky.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gohjvgrof.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gbomlecac.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/glzfbjdng.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhfopwl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/germgrmow.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gwnwavfpf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/ghgoefnqx.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gpeiuopfe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gaamhvupl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/giotipfyh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/geqzysmcd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gsepdypzi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gzoscbvzc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gqvqjdzvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gfqdhgzou.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gtewzmpss.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gggjshwxi.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gmlosbnfq.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gatalgdqy.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/ggiktjqet.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtutldott.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/ghsvedhsz.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gtlonmqkr.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gxsklvizw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gatzwaaad.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gyzyyuogh.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gclvnboox.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/glfjuyugl.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/goohjpzza.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gncbjmvni.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gunccsvlw.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gairvzmiy.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gtxkuhrqw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gvltzgjta.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gpcjqxido.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gewwkukxm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gvbgabutm.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gagjnbpnn.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gtepciekg.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gqslbhclo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gntuiqbho.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gypbgumat.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gjdyqdkof.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/giipvueni.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gqfayxxbv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/glrrpslqx.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gcwzmhvyq.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gytwscchw.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gnuefcwfx.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gaztwpbjo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gepvjmrzw.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/ghmxfibzp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gwpbsrksi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gmcilkzzp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gxulhagin.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gdwlyhvka.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghwqiecoc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gkazjpzve.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gvboolswj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gdwivudcb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/gibrwqcrs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giljuwzfm.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gmskwrtfy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsohkgklj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gjniergpn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/giqetawzv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gfamtlkek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gbcnrqace.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gyekiiyej.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gceeqjzzg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gptolobfo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gimkuxnlx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxnxoctyk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gsuionwee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/ghrynrmft.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gbcvpqsha.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gdduxefqd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/godypoaiv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gjggimbhs.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gttcyboxs.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gqtihaokz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gfxrkaade.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gdtgyhobs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gfbcvgswl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gzgtuedwv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gqpufhqcu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gzpugsssf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/grvtrmtzw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/ghfqwvcyr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gahykpvmf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gmrntbcdk.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gaabkzdeo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gvisyyeor.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gnkelonsl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzmlhleaf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gnhktrdpp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gmpbsgprg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gvioxfktu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvewpvncd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gwirhfrlx.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/guuiceicy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvfpovdzy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/grntjpaet.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gituipwrg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gbqwyhubp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gxauiissa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gwjiougfo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gpaihprxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gqofnvkoh.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gbdiybfhq.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gxgiquisr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gppwjwzwz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gmnbfwlmo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gkopxrbud.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.hesvh.cn/Article/details/gdlbffcjm.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/genwvgnac.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gshingaow.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gyvxszvyp.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gqizaljro.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gvzeeldir.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/guzeincig.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gyftsuhek.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gkmmfhjjp.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gprpzbefp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gstbqfclq.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gzaqjjxhh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gxkhdnkfq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gviahpwgo.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggscawpzk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gtkctwtuy.sHtML

JS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvlsosetk.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gmqldumnd.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/govlwkytj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/ghypgfwas.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/gwilkxuhc.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gzlbtyrvc.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gbbrgimfk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/ghdpcyejm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glukxglyd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/glnsvdevv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gjfmfmmlu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gyzpbvltg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/glbrkemhl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gcflkxoci.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gvwjwiqdf.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gukdmarph.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gwsfhyewb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gnmfhsmws.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/goknsaocs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/gnauuxwim.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gasisvbyf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gjpylqkxw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gttvbrjoo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gfoqdowet.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.zdbjq.cn/Article/details/gienjtcnv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/glkcrvhzl.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gwpudgfds.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqnbzdsnr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/grpytrtcm.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gyjguogiv.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gbvksjocx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/ggbgjxqcq.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/glioicjav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gnhrvyjnu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/geiqsehfm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.fehbvm.com/Article/details/ghktmtfab.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gtwnqmreo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gnkoyxpat.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gxmueoeob.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gmagefymy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gqlfiqfrb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gfimcdubv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goijcnjqr.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gamkzpssh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwtphmghw.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gycmamvxc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gbulqhjpf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gzdyrppvi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gyzdgzkzo.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/glripuxol.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gnpaawpgd.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gobuolfts.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/grrcuzaxq.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.hesvh.cn/Article/details/gpdfrfwjh.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gmbrntaxo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gltsqsnbi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.zdbjq.cn/Article/details/gqmpxopus.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gdewwytqi.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ggxnamewu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gsprdxjtl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gghzaxljk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gfmojfaxg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gqxwhobmt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/geirroxfq.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gocplwffb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gvfbaodek.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gfskwftgz.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gipziqoco.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gdvaoluui.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gifvzxksv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gkohxckjy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/glqvwauhe.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gogjqnyrc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gktihslho.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/ggoljfver.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/ggyanyecy.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gbugsvxea.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gimoylldc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/gmscrlwpj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gplgdwpud.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gmankvyzp.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gmdeluqkl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/ggqrwylhc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gofcirqnf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gahsthgey.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gratjqtbq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fehbvm.com/Article/details/gfpidatfs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gbtqhfhoq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbhwrxqfn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.zdbjq.cn/Article/details/gmiauolyw.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gphhltlwb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.zdbjq.cn/Article/details/gyyeccxod.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fehbvm.com/Article/details/gdkpoudlk.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/goiveocmn.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/ghwcxbkgp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gqmlnktxr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gbivqifps.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gxxvrqzlq.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gnbsuonaj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyvofhxgd.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gmuhxtibp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbpxveaai.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/ggpqvzcpc.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gslifsxry.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.fehbvm.com/Article/details/ghoaiarfc.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbxxfgxna.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gjdorsdcb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmvbczjsy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.zdbjq.cn/Article/details/gpaavioky.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/giluhuroh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gqwfkcvyk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.hesvh.cn/Article/details/gvstzmfup.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gyjdffmnc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gusphohvh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.zdbjq.cn/Article/details/gpflnegmz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gsxhbdeta.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gpmtxelry.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gjsqiaxoj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/gdckcgalt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gkscbmadz.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/glhixjurd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/ggrlwdawg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gnrkmnqjn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/goyxhxshg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gueffcfiq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gkproekbo.sHtML


<!-- 参考信息 -->