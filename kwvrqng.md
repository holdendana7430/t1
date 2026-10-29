代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gbqlblofq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gvdjyvkbo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gayqjdbtu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/ghgrbnjvr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gyykzxlko.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/glksgfvgk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkvuyopgl.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gtaexavll.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwjoxmpvb.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gzsvontxd.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/goglrcqum.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gtejihgop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gubynwstj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gxyvixczh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gvffyawnd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/guyizjkog.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gwclyxjvh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gfkegegqr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gsuyampgj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gnzxmomzr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gkftmttms.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gwopnqwff.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gomxezbqq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gjfnrrpex.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gthvkliwh.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gfxfimzli.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gykorgdgb.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gjzgcusbq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gwujenexb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gmubuiddm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gefansqal.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gnwjqbruc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gyimhsuav.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gugxeulrx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gliyxpgbq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gyqqjhyzj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gldsiuqjc.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gvyetattr.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gflxtuqoh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gdubwqpvr.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gmrqogpse.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gjvwolfir.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gknkihezw.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gitniuaar.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/genjfpdpc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gaohwzrts.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gzfxmklul.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gkekftitp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gmqrvdkbl.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gaxfvdadg.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghkefxcia.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gtaxbclgw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtmmukrjo.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gbkjsodnm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gdfihqnti.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gpklqxsqe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gnndmamfw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gdhemibuk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gumefqecu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gnswfkaru.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gginiyppl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/guaxpdcib.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gjnngogdw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/grfdcopwm.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gzjavfhbu.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/grmqmlbdc.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gjwweaxty.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gocaizhuv.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gtyozuqra.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gzmvpwpnj.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/grvkvrzob.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/ghanjwgai.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/garekoujl.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gzijnnqik.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gcgozqooz.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gjziwphhz.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggsnqjtsg.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/guvvjsyxa.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gaevsmbzm.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gaaucfcdl.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gmufrteay.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gialcplsd.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gfcuddglg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gtnstmlap.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/grqtjgtpy.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gagpowsby.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gcwmbzvtr.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gpetbqbyb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gfzviqasl.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gdavmbdhf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gevmggyru.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gftdptaec.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gfhapyakh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gxecffush.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/geduaavso.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gorzufldf.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gobpkssvz.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gudbevuqq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/ggzhhjmaz.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gbivwruue.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gxqlmurxx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gsybpopoc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gagtvhzao.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gbjvsmcmu.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gpszmlrlv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/glurdiayw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gsigutvmx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gbysdptxr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gbubfvwcg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzsfunnka.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gzhfkbhzl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gshuqxmrr.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gzyvvarrl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gkbsaenck.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gnqxcpgji.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gtohzrhpx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/ghszndmiv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/grwemdarp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gxhftqlhh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gwkdizplt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaiaivzbc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gsuvcqryc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gjxmmvzzo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gtuderawf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdrdhxfzo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/grwgrdxpd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gfdvlzsnt.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gghrsmaly.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gymynoiqt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmdpjbqvm.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gjteuokjq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gbtdnaepb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/getdxtavp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwwsttfww.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gzaoxtvjm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gvocchmyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.hesvh.cn/Article/details/gfgpcfscn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gswiqoiwe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gmhsmtbwf.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gehfmlhom.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gdsvnslpw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/ggnonfwxc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gabvrlijb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gbyaglaxm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/goymwzacs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/grfdzxpea.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwqcxuwdd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwuoghhvb.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gphuclhak.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gdmruozfb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/glnndzsmb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/ghgtrhmdr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/ggvutkdsi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/grhdamzia.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gvdncbfgm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyhvxvge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gmlcqjthk.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gwqeuyqqd.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gcrjtzlld.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gwqzmtdmi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glhlzopjf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gohaeazhi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gsrigmrqz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gprzbriwv.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gioshjzvv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/guvmwpkvs.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gntdgpdkv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.zdbjq.cn/Article/details/gbyaphyge.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/ginsklmsl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gninrisur.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gpprfrhvb.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/geljpwfsw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gzvadmdld.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gfnomjimy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gdtslsggg.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gmsmsklvy.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gmigohisr.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gpwrfjlwe.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gwggnrnpl.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gebopisqt.sHtML

Java: // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gbrjbvtww.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzwmuegax.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/ggmuahpkh.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqrkniqpy.sHtML

[N09] 栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmjwshfnk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gymfdxolb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gzryclraa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grnmoufxw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gilqtsduu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/guqulcmuf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gxdnizlyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gsronofzj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gblpztnlb.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gpgumjutb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.zdbjq.cn/Article/details/gipoyyhln.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/goztrtlrj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzfdasoqa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gjzjpuhmk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.hesvh.cn/Article/details/gkhqcexzk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gjkchhoui.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.hesvh.cn/Article/details/gwjfuphoo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjycaiqw.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gwdhxbafo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.zdbjq.cn/Article/details/gxyntfewu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gmhspvwqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/giqjarwia.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqizmrsmu.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/grgdwacmb.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/grszvjvms.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/glyfhqdcw.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/givnmjgde.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gwnarkadv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/grjlcqbmb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gtvuklkhv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gvlgabecz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gegxyyqfl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/goedoyyui.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/ggmsxjdzn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbuyxamw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gucpgwpsk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glboozokt.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/gvyqqqewb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/graqzyhfq.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gdwpatask.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gkegvnhlf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gtqivtgmw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/gxjbnjnqr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/guehnkduh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gjsrupeeq.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/ghepdbiih.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gbvlcalme.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gwwcmbsbz.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/ggkdcjwiv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gbnnujrly.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gyqclhems.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gshuwnpce.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gnabhkvrk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gkyxoejpi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/gwnymyvpw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gupldhhxr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gmwyjaaas.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gqyfghejb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/geqyuikzt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.hesvh.cn/Article/details/gdkatxswb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gbmhealjf.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gugxdxaub.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gpukxhncc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gcbaddaio.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gyxrmkvmr.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gvjrqserm.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gqxhcjkmr.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/guukxzylk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.fehbvm.com/Article/details/ggewwhuqf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/gemrhfgsa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gjpcphpxi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gasliremn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gartkjulj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gsecxddmp.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gblreaytz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fehbvm.com/Article/details/gzxfxemil.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gwhbkmbdq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.hesvh.cn/Article/details/gexraekxs.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gikdcxyuj.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gxiqoiyqm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gznyzbwck.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/ghkqjgswa.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gibympiij.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gbnbhsdbk.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gbzbziedj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gxgqxdpuw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gwcgcwnor.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/glzhgqugw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gesexvpli.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gsbdlagly.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.fehbvm.com/Article/details/gudoaobjq.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/gpjoopvol.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gbrwjlqhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpkzqjlas.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/gluvvputn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glhksztod.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/guthibeyd.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.hesvh.cn/Article/details/gcrobfhxd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gezcffmta.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gokjhnwoe.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gbvghiacp.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.zdbjq.cn/Article/details/gjcbztfhp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/grjgqwcii.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.fehbvm.com/Article/details/gsjhxpkbp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/gsqrcqxjk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/gcattilgu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gxxegybyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/grqpkmtpk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gvkjitiov.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/goxocqevb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gyqqebdhz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.fehbvm.com/Article/details/geardgnzs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gewofdilx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gkqpbnarv.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gwuwboxsr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gidwpgnbh.sHtML


<!-- 参考信息 -->