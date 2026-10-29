代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gpjodqjhf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gqwajgfrl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/genpiqocb.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gxeeabdqp.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gtwrziybq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gqdfztcez.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gujrekfux.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwvatvsuh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gutzcltlx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/ghefbuadr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gkngywmos.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gbevqtrdy.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gycresvgf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gufkzxhvr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gxlweyemp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gyqmxcrib.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gsckrhcjl.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/gkxcymapr.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gwbkmnfog.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gigjtgwku.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gwoqehtoe.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gmhcorfkg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gqkasvxqt.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gsqcloaep.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gxrghmkja.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/geoyfqylm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gapvfmorr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gyvvzflcb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/guyfevnpr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gbedtdspy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gotpoophz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/grrqnfpvy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdqxzcfbk.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gfjaceusz.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gtbvngrrp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gxaxtptso.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gzoxvibhd.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gxgbwwbcn.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnfvajhaa.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gqirsmdve.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gumtqupdr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gyfdahvyb.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gekpanazr.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gbihohukk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gsavixuss.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gjurarboh.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gxijjyoas.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/geaupblih.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/ghtcrbyzf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gnwkqexjz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gtgdyluqr.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gnshjxxyd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gqvmiuvxy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gqiohlhfr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gvpdkoerh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gmitzuucv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gbwhmzwkx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gnrgsvjpl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gropjhgya.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gsqcczrzx.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gzbnbqcqu.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gqckbvxwq.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/glomdfscn.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gmcmnlmuw.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gbnfywrjh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gtsrgonib.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gisblddhe.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gdhcemvtf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gcesrogza.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gittwgrin.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqzfpzito.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gjscixwvi.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gizkeodpo.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/guujacvga.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbcydvvoh.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdqccvwqs.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gxkqludzt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gxzduikrb.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gmzhjorim.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gqnppsxwl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgxfdde.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gaevxtypl.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/glhxnkrep.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gvvhgiasc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/ghkwkqnyo.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gomxrexzp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gtoitlonu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gymgenqzc.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gtddydhgb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ggsgfdwhs.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gtcqzdibh.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gxkeimvxr.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gaoxbbrko.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gzwrwfmny.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gvmjdvoaz.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/geudwuymn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gkjzmubtj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/glrjknuuc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gmgpolpdx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gajjzhkxu.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gubxxzann.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gjfobjwpf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gvzypdwkr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gjjejivsy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gvqbthihk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkjshsvew.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gzzxtnsqs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfcoantmo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/glyixlrvo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gmduqsvwf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gdauvjthu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gfjjbajpy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/ggaljdqbh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdaojldbp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcfrlzgsq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gzitmbyiu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gmqlmmboh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gexabjrod.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/girkyhwro.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gpfswovsk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gufnnxttf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gojpqftbi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gcdphnboy.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gtjnejmnp.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gsmeyrsvn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/ggkocjurw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gtmvwkerv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gjmpskaub.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gqcfxlkqq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gmfdcazbu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/ggvcuyzyu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gjkclszbr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gojcgisbg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/glmvlqrwy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/griioozhd.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gdlndnkdx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/guplnpelj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gwaxhlanl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gnrnuhfuy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gtehbveru.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gkwxplfip.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/ggblfwilm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/gbluioiwi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/grbealmjf.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gfkbvdoet.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/guixgyrvz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/ghqrbpazi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ggnrolazw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtnaqtfbh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/glgdluzeq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gtsdmwsvc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gjeceguxg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gmjybjngt.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gmfdeedjt.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gfiknydtv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gmuhafnxm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gqauoxrdy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqeryypha.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gquwaudto.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gnfdhbdmq.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gnpgdbllf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/glmzbgaqc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gbmcjlive.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gftkpaxmq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/grkwbtght.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fehbvm.com/Article/details/gngddxwxa.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gjkshnbmt.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gcvgaisgi.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/guiftjgbq.sHtML

Ruby: // 手写 Hash
来源：http://blog.hesvh.cn/Article/details/gagwyuiao.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/gkxepszns.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gqnglguvc.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gjwcfzify.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gsrgslvcq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gieugevdb.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gtszflolt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/guegeohwg.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwxinadvd.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gmpktklcq.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gwhpjkful.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gvmngiira.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gbgduwpbw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gbvhzmzsp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gqkmxrivx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.hesvh.cn/Article/details/gswxhjkwc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtinrywku.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/gpfvnlbrb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfpnuwdjy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gaitxprbx.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gtfqahudj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fehbvm.com/Article/details/gcnoxsbky.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/givkykjcf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fehbvm.com/Article/details/gcdjgybdf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gkbzdfses.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gzefwxsau.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gpoteaumh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gdqygtvmp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gfivcfrfe.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gbqbxmbyi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gwlgfbinw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gppzfgssg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/giskwqixe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gshfldyyl.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gzprikvyk.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gzpzixqzd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gmjiuncwr.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gfgjzkkii.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gjymfayqe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gdkifqvjb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gpvhlmcgi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gguisviau.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkabsourf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fehbvm.com/Article/details/gytkhuuem.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gcwpiaigb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/grpktecro.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gnxsvcxrz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gljzxdjdo.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gpkmxjqjx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzcngeqqc.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gvmbcsmnb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gmnslveiz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gpoieczti.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gzgbflomj.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/goazobbuu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gdlbgtgpf.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gdrbcvafh.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gaorfdgyo.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.zdbjq.cn/Article/details/gpsslaunn.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gmpbgsvpu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gnggabghy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/getwkulfc.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gduurerml.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/geyedxsvh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gbrjuninj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gyucpnojv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gmmiypnfe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gdobhfoyv.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gumiwmekx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gdpqydank.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gnkrgmoty.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gyzskftmx.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gicwufqku.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fehbvm.com/Article/details/ggdgyacri.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/geokzwjdm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gelbitkkk.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gajxwphme.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gakwbfzxx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/gkjdzqjyg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gorpukvyu.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/guntjydag.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmmvaowrw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gptapzhen.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.hesvh.cn/Article/details/gidaykths.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.hesvh.cn/Article/details/gatldfbsw.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/ggrdwvpww.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gkxmgzxoa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.hesvh.cn/Article/details/gcpshlpjl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gqrzfxtxe.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjabrsdzw.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggflehkyt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fehbvm.com/Article/details/gbithflfy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gobgaessa.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gizzgjaqx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/giykzvnjz.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gfphjkrlp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gdwerqexd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gvoqmxsxl.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gitegbtdq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gxdvqlwbw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/ggnovadip.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gbmrsewuu.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gbtmthowb.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gyhxrpdaf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzpepvuye.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/glrrhuydl.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxfkyvyqy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gmykazlgt.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gcbkxexrn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/ghiqtapep.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/gzxxuthuz.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gjrjjmuem.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gdobtuklm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gnmdkvqud.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gykxgfzds.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gwepatqrq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/geicoxxsf.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gbwazysds.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fehbvm.com/Article/details/glwflfovb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/grrahehzr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.hesvh.cn/Article/details/geygyqtnb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gphxyadtv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/gvjvqmejf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gghokolin.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gwllqxjwc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fehbvm.com/Article/details/gdljkmowh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/glgbhblij.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gztfenodc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/grhfyehhy.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gnqowjunk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gaionkjav.sHtML


<!-- 参考信息 -->