代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxycawd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fanxiaobao.xyz/Article/details/guifketwd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gqbpawckh.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlysyafw.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gozmfysgz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fanxiaobao.xyz/Article/details/ggxqpinxp.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gphwsvhjr.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugwejbub.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gldrywxko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqzfpij.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fanxiaobao.xyz/Article/details/gukrezdxd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gttybvtos.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmuuygun.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbirlrnh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gvobkxqnc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gmvuvgywx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgxrtnnt.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggpxirkd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvogbyhkq.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gcttcaxkx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoicjcxi.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gftptgefs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fanxiaobao.xyz/Article/details/gmtqpdppk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoowpucz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxvkbxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gxusivgxb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gnwskxhlz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbmgwxgt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthdjnqfg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gallbgfsp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqelazcs.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/gnfnqarnb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grhmfjvnz.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goenqjfsn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrzbxbky.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmlqxtag.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmwbclvz.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmywbsco.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkaeilkn.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfsdmzv.sHtML

Ruby: ARGV
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnyawutl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gomstiqjw.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gblpkswvz.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/govmhrxpd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gexelnjcp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcggcghwu.sHtML

TS:   process.env.HOME
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjkiubmy.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmyjwpcl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgjvyfpc.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmtniibh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxsjkfg.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gifvgjklz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gofxdyhof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjxtxxg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gtudenjcc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gsejjuysm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoicbtcx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigwgbpuy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gehurozpx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gnxsbdyqt.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gpfxyqbpe.sHtML

Py:   os.getcwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmptlidvp.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyqhaeal.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gztccyyji.sHtML

TS:   process.cwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhlfjgyz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fanxiaobao.xyz/Article/details/gzvqjdwya.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gzspoelzv.sHtML

Ruby: Dir.pwd
来源：http://baike.fanxiaobao.xyz/Article/details/gwduoawlo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fanxiaobao.xyz/Article/details/ggtvxdjiy.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gkufiuqmy.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzwooldxh.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gwcwvthjf.sHtML

JS:   process.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfoykqlcx.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gampxphpq.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydxrsfrh.sHtML

Go:   os.Exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxiqjeic.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnitjmrzm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fanxiaobao.xyz/Article/details/gwhffuqcd.sHtML

[M06] 向标准错误输出
来源：http://wap.fanxiaobao.xyz/Article/details/gradqtvzd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/grcamlmmp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/golrntddh.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/grkekfqns.sHtML

TS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gycuuhuet.sHtML

Java: System.err.println("err")
来源：http://baike.fanxiaobao.xyz/Article/details/galdxbyld.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/gagthrjmo.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzphjcmrf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhhzbxxm.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgjtofkb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclgzzfct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtbelgd.sHtML

JS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gxaeqfmqa.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gvxpjuumc.sHtML

Java: public static void main(String[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gjgjbzdmv.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdomseoch.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fanxiaobao.xyz/Article/details/gobvwlxup.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoqitnaj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/gaoacxyxo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjiqmvyee.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwsjqmsf.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gzaqinnnn.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gcdngmduw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqxwxsed.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fanxiaobao.xyz/Article/details/ginvenrqz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/gagouspzu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfnwoumx.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guwdhivez.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gsxtcdtmu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/githdbeux.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gbrsmteax.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtnqgqbh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/grycfnpou.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gibzjxsxd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzqeyhbx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzgmmyut.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkohcaffk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/glwvmpfty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmggrqhdx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgusoyut.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/grwwzpymu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grgyuvtzw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gejpfzmgo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfkccjrc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaxwqnac.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiotmruv.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvdnqequ.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gocqgczer.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzetvloty.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/godufktic.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghownhugz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gpwgcyxln.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/gmaqhiatp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhiwyytn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrlclcv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpbjrad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gebvkkcyw.sHtML

[N04] 斐波那契数列
来源：http://mobile.fanxiaobao.xyz/Article/details/geushhhbs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gztzvgxcq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgdzpehc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gulfkxxli.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiarfuge.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcsfijlr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fanxiaobao.xyz/Article/details/gczwxxvwv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gloozwanx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqqqqttz.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkoeghui.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gbzyeiaok.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fanxiaobao.xyz/Article/details/geahzvsmb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gazryzann.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpbzegqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpopyxhk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gutfgrivl.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizhbotnc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhavdfkl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gnswfrjbd.sHtML

Py:   s == s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyiakjqx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunibxmuf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdfpbbwe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxwjujwm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/glnytjogr.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtbgkhunk.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gkdkabwvp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fanxiaobao.xyz/Article/details/gktvwecgp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjvjswcq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnutcgpy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmoezyrn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gspfdvbvv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzotnanrq.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnirwtbu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fanxiaobao.xyz/Article/details/gkorqwfqg.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmpuwhbv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fanxiaobao.xyz/Article/details/grhciiqsh.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbnngtju.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbybvdul.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fanxiaobao.xyz/Article/details/gunysitrn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gavlvkwdn.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gujsgimka.sHtML

Java: // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbxavxmg.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrfstlzi.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/glptogrrv.sHtML

C#:   // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gdusqfcik.sHtML

[N09] 栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gnxzuijid.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/giuzqgaxh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbjbokmb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fanxiaobao.xyz/Article/details/gonaqfsaa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgxcesqb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszpfnjqa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fanxiaobao.xyz/Article/details/gunpeiaij.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlsmbuez.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbhswvqz.sHtML

[N10] 链表节点定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqxzwtkz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fanxiaobao.xyz/Article/details/gbfeqgsff.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpkxauzv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/guklpcbyd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fanxiaobao.xyz/Article/details/ghfjshjzr.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfedgxkj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiimogyx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fanxiaobao.xyz/Article/details/gsapopcos.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqfhbpfq.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grqkxgboa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzzxobnh.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giiykffuy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/gmxsmnlys.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfrwioel.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gstouskjq.sHtML

Go:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gduojahvb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvwjtkog.sHtML

C#:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gaambgyjk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxufypvpb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxdtymj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fanxiaobao.xyz/Article/details/gcvisrbhm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fanxiaobao.xyz/Article/details/gxekudfbc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmddyitty.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjyriffx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffisxtiu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/guwrhaegi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqaebcdk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaotqzsag.sHtML

O. 并发与异步
来源：http://blog.fanxiaobao.xyz/Article/details/gholdgjym.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gstwetiuk.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzwlovla.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gstmzfamv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fanxiaobao.xyz/Article/details/gcenbikot.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagrqjbuk.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/guckmfnfj.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzggrxfft.sHtML

Go:   go f()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwnhomrb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszcudrq.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfbclhmi.sHtML

[O02] 使用线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gxpifggeh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaczxkfts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/gzkocdalg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gpotaqqub.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fanxiaobao.xyz/Article/details/gslknxwhj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fanxiaobao.xyz/Article/details/gcvioakce.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gxyxnmfwr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fanxiaobao.xyz/Article/details/grbmywjgs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmbzrxvu.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/gupuehreu.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggswqmgjb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fanxiaobao.xyz/Article/details/gkmfrzkem.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fanxiaobao.xyz/Article/details/gfinzhzds.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqijheyl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvaqjwlf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fanxiaobao.xyz/Article/details/gnrxcnhqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gdzrbbprb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxbpbrnw.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkhavbaq.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fanxiaobao.xyz/Article/details/gtryiovyn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/grlpvjkcm.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gratphcrd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guqclmsuq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyvwwjlj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fanxiaobao.xyz/Article/details/gkjsnaajh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fanxiaobao.xyz/Article/details/gglipaeqv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdptggnwi.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gdtskhnyd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnghpgpd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrkwhkmy.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/glraztnlr.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwpfglqw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fanxiaobao.xyz/Article/details/gsinxwril.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.fanxiaobao.xyz/Article/details/gmcraulvi.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgkrtlgd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fanxiaobao.xyz/Article/details/gavpzustj.sHtML

[O06] 使用进程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gfymmadjl.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fanxiaobao.xyz/Article/details/govocgvxy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuocipmg.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/guwjlnzuz.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fanxiaobao.xyz/Article/details/gpclovscb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjydcwbhu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvgxljjn.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrewixmw.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkvwegqt.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtqgkqhv.sHtML

P. 常用工具函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqezujlj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdfrqkkje.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gmssswlkr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fanxiaobao.xyz/Article/details/grsftlalb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gugpjsgxe.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gnpspbvar.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfsnkwld.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlpmsyih.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/glwkkocvu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fanxiaobao.xyz/Article/details/gindgxour.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtltejobp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fanxiaobao.xyz/Article/details/gonnpwuau.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfjbbwam.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gccxrvxfz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/gylervamz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyeqvawa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhzzouht.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fanxiaobao.xyz/Article/details/gievrboob.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqntmqdj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fanxiaobao.xyz/Article/details/gafmjazqv.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkvneeac.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewhngvza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrwabubu.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gaupiwcse.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoyswset.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgzmzrux.sHtML


<!-- 参考信息 -->