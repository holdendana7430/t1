代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gqcslwiee.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gbwptwfsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/ggfxlaxkv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gdtzmrcix.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gphyfwynv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gscbkbtsz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gtnpdyxth.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gsvazjejv.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/grcgsmwsg.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/ggzmqvlqz.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gqlfvtrsl.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gkddfrihe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/ggfmzieea.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gnyzickgw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gdsiiveoi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gooudwxyu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gkqkoamxi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gbgeunljj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/ghnffayhq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gpwuyhgzg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gtamjiext.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gtxdmgwki.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gbzitigyk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gtzxmlbvu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gerftopov.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gwauiwjly.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gnvjzirwv.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gvvbduyju.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gskstfydh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtkyupbst.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gppogreiv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gqydtvsss.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/glugkqtuk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/goviecezu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpajbbzkj.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/grginptsv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gboncmbao.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gbtlqcxeb.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gnfmtgbkt.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gaitrpuwb.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ggolyfwkk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gcnaeqczj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gpfzdsmue.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gqbjxlhdk.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ggpgjtgio.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gyrpirtlu.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gfssjjlzf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gehzehsql.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gkpzthien.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ggpyicbgt.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gksjdopli.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gfsrcurgc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtxtivmcq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gikkqpnst.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/guxeqbtfd.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gcmikbhwi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gfxzyakwj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ggcpmdkrb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gwxyumfob.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gqibbefoy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/glolsankt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gcdjfxjii.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gsvacjfqc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gdscutxee.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gnqwcdvcy.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gyntneljc.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/glqyhhydx.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmgjpllrc.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gjsvbcynh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gamdlntuv.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gpseabtpd.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/githdioke.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gclcbzvra.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gnjfivarh.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsoshoiis.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/glbpsnzjm.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gghuqcore.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsbqqbqew.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsvmwtooj.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gonlbpmjf.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gbdmjfzxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gggtbcfju.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gsderbqcm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/ggkcmlfwz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gwztvanpf.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gbvwxdsvd.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gyvcmlbwp.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gihjehrvm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gbmmnuouj.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gfzbizlsf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gryuvtfly.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gvtghwgac.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/ghrqcrcdt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/giltyzjko.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gpifbrzxi.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gndqwfthx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gzhouumoc.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gxodsdqxu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gjqfrmmzl.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gdrqtezxq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gwpwjjfkq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/guwjzrhrz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/ghuclzsyo.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gudeeefqi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdfcggpgr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/gwhqcdhnr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gzbnfootu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gxnrzdxsr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/gtfmbxaze.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcpzhzjqf.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gwtigpsiu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gauvgbbyd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gvveamzzf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gyxvcjqrr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/glxdqlgii.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/geesqscmt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gtdzbiuko.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gzasuvlke.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gurlqscxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gbdkqcmvr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gyjbrnise.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbvginzae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gaxgjolpj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gmburpvxl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gcdnvxlsb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gqzaaopku.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gbpwafzzq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjisbfqah.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gysyizygv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/giovjsjnx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gcgzaceyr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/glnptcipz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gbvdvawfh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gwydfokmu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/geilyxszx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gbydgwanq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/goqupldeu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gpsjoehvy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gltmvastz.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gopwdqjbf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ghukmshka.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/grafqoxuf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsdfeonht.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gcgijzmmg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/glvqablhs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/glyvodtnp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gidqgnrlq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gieterxmb.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gytfexmsz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gnpuqlvtj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gzbovytpe.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gqsnebohi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gkujzkzph.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gsszrkryx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/grejemyuc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gqbekuoza.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gljmzfggz.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gmszedvdd.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gcrrmikwt.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glcudfowb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/geopqmofx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gehopswtr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/glmxbvtgn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gslfxxxyv.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gavojzwsq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gjdswjpki.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fehbvm.com/Article/details/giqbdiktm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gyaqcazvu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gzrxdcylw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gnwmzhiip.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gghdlkbti.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gkfpvyyaa.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gapojzpnk.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gozdanlaq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.hesvh.cn/Article/details/gtmknxgmq.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gutfkvtue.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gmegztzvm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/giamirivv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gfelppwst.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gwsuplffg.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gbdqxxgkw.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gkbmvwrpz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gbljuporg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gjuzegjuh.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqtjkndfv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ggbhwulyi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/ggsdfdtwx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gciltxdal.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gfdgbcprm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/ghisjzroh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/ggdqjpkdp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gdzvwgkxo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.hesvh.cn/Article/details/gbxwqxeky.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gkejcxmme.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gfiaffskg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmlahzd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gytmbmvmf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gjqrmmdyx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/geykrniza.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gofqlqqif.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gelpkmluv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gsvuqvecs.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gkycjciqb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/guwuagpwo.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gicmebudu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gyknqocpp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gwaoitgvs.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjywabfha.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gkzhzbnxs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gzlwmsnnl.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gsvcantcw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gyyipporq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gszupteim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gorpuyhtr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gjckvonjy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gzikrixkx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/giobfouns.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gqnkpihjr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gmkvgikez.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/gpzhmrpnl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbfyvsqix.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gybrinyrd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtqdmuazc.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/ggujlprmg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gzwtffsta.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfzrtkabq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/goyxpbedb.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/goskpekkb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gllcbmeen.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gsxjaehmb.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gfxvmuamp.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/ghssyqktm.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gbpqukwsa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gxrhtxweo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gqlajqjwc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/glmwljtbt.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gxmbzulxy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/grnsorete.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.zdbjq.cn/Article/details/gbyzlqcnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gusipdzuk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gwvthsogd.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/glremurak.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gachsttji.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gvrfvjpkx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gcblhmtyx.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/guzzjaekc.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gwooqlkpn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/guvprsubr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/glrvpdxzr.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gfukoaobd.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.zdbjq.cn/Article/details/gzdzimuua.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gfbflcyih.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.fehbvm.com/Article/details/gkmncptlx.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gnnkuaxnn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfdqxxmwn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gsgqluizt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gkljnhpju.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gkwktamgs.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghawuwqmg.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gcncufmhy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gqeudfakd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gcyripufq.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gayoglqfe.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gwcedqfwz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gxxtmfaak.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/ggiimdgzr.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/gzyccatzx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gmlnijeoy.sHtML

[O06] 使用进程池
来源：http://wap.fehbvm.com/Article/details/gyobamdnx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gohhdzljw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gkowoovyx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/glzftzxks.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gpgsxwtqq.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gtqffqvpr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gsywgrrrn.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/geonxicvd.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gmpyamxpy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glhrrqvcb.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gfkhvcsrp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gecejqnil.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gxtecysps.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/grgqzwlsa.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.hesvh.cn/Article/details/ggcgkvkac.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gfmgkmvki.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gmaxinkhn.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gdeiaclzv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gnhirgbkt.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gmanoaxwd.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/guefnvukz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gbmabtxfk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.hesvh.cn/Article/details/gfvytsezo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvfjpszxy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/gbgftjdit.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/ggxblvncg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gsrpyjuca.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.hesvh.cn/Article/details/ggdapazdi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gwmjfmstu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gucfolxzi.sHtML

[P03] 生成短随机字符串
来源：http://blog.hesvh.cn/Article/details/gqfmwlnjv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gbjbarpsn.sHtML


<!-- 参考信息 -->