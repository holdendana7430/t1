代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gpeqmphzi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gyymqmrix.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gmahjeciv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gwchmakii.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.fehbvm.com/Article/details/glkvhizbj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/glozwunfh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqgialyth.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gmlvekqwy.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gazllwxfd.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gwvipwucx.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gtflkjtxa.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gsvizsolp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gbtbozctb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gcefvjadx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gzumwkvmq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gabpcvbkh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ghgwqtgpe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gwhisjgqo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gnbsxfjrc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfojrkduh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/ghvszwkcx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gjhrbdvva.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gbcomjfee.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gutjvepya.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gchhrdeen.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gggpxvbjz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/guzhwmcuv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gaalunqit.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtvwsxiav.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gkesiowjn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gddhoqrqi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gtllrzfvt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/ggsfpmiid.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gquzkluzo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvqtbswsl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gwzvutywb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gojtekbhu.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gydizqrun.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggnowqnve.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gzspstxco.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gljrtyrnd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gyyoehuag.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gchoyhgjj.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gpgpbwpxe.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gxirbisew.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gfjvihqbr.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gzuncggob.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gtiiwzkpe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gtcvxbxnp.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gastchidk.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwpbiahmc.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gjtihecyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gzhnlbcab.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gfsjogoif.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/galvadvgq.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gsvqsfivj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/getuuenzm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gqvzhvejq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gpsuzynas.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gdmgpoduk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/ghnjorczq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gqvpipnod.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/ghrbbyjky.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gqvwtdmid.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gjnrplmbj.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gxxmkfktr.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gqfrsttch.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gpxboabme.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gplinwagd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gsvqludxz.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gjqzycecj.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gwhuepjfg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gwgolhnbz.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gpikfzkuw.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gspkejnvu.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gcenseuhu.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/guwxlkkcr.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggbkpwbkd.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzmpyhncx.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gztbmwwvt.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqdffpten.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gxryyewdz.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/ghcxvheja.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gwqvrdczc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gxmtamvjm.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxecyquds.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gdwzkaqid.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/grjwodcex.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gdpfraxub.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gylvxjbmg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/giaixjaqy.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gjzmirole.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/grbmixqzo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gxrodxugj.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gfppcmkvx.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gilncncso.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gsqsarhbj.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gnwdehshy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gmaueqwgk.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gokhwdygj.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gvdcjmarl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/grwamfzbe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gxjrrqsql.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gwygdulmw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gkpafrpte.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gyihgnfoe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gwyahtrnv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gbrbxgbji.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/geeomtojf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghpfntmma.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gcqeyobzd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzdtllv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gtqyacwkb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggtlwgjbh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gbxyjjbmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gngnghdoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gfcilkkdq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/guwlithqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gudzoyvvc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/ggoetkzya.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdphadldm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gmhwdkkeg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjrfbmczs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gtkcqyesx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwtksentj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/giudxvxus.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/girfxdtpw.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/guizvcpzb.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gmplnmonx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/grrignftz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gactafzeh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/grqajdfhf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gpctabghj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gepcjcfwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gwckqnyoy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gcuxkmqai.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/goiltwtuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gbizfisoi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gfohdjqzg.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gbzmzyfhl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gazsxkmog.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gmsfcfdws.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gegvzrdup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gldlhkekr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gzvyhywnv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gwtpghurt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gxhkypwsl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gafxbalnu.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gnvjrvfgw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gsdtjnebl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/govxchqdq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/glembmcrv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gwkmyfkrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gxtafkmcz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gugrchzys.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gsrfzhdrv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gbihmmsnz.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/ggdmutrny.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmobjjxvj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gnkxrfwkl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gicmbdzfj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gqeuhfyst.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gghtqaiqn.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/guzqiiful.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gyhrmepkc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghkfqytwt.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/guczfcbkk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gdhcnhmya.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gwtozlpnh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/ghlaelmip.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gdruonniv.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gsfdmwgoc.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/garibcdmt.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gcfolrdzs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gmwcqrrut.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gwiajseam.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/giyxwosoa.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gekpbynrs.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gifaabckh.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gryahoxhs.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gocbxebko.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/grmteznrp.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gjkjejqhr.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gublargok.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/giyaageye.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gdotiylhl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gyhryoefk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gqkydmrxa.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gnvnokiev.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gkxlqculb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gmckbhbfi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gugozwnki.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glmndidqu.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gdzqoppsw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gilfgjgdj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gmydprcdd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gragxppvb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gmjnxrcpl.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/grrkwdpyd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gvxdvluti.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gunromble.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gexqmnszp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/geahhsxyt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/ghilelzoa.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/gzpsgncwl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gooenayou.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gevbdhisj.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gjpukopne.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gryezvqxl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gtqcwnxvu.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gfcclswkb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ghhyakpkc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gbcrgrrio.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gytgridva.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gedicxsjy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggbeitsdi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/grgnlzrji.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gntssvcar.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gstbnajry.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gglzbxepd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbjolldux.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/gufsrvryt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbzqmekuc.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gsvujqztx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gvidmxnrr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gecpdykfi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gltvnraau.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gwcyvuhce.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.hesvh.cn/Article/details/gejfnvqvw.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gbetnonvc.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gqakbvjfq.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/ggxlqrzcn.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/guzdvmzuz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gxscrziqy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gzpodeqrd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/ggagiwvsp.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gpemqlbeo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpsgenac.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gauvaqkep.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gxznpnbon.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/ghwaqutin.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gswqonaqb.sHtML

Py:   with lock: shared += 1
来源：http://blog.zdbjq.cn/Article/details/gwfyxtjum.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gjqdwbxid.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fehbvm.com/Article/details/gxfjpnfij.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gccqawzvy.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gjinxxuwe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gohcowkjk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/glslwjwsx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gfwouwvmv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gpibhudee.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gbsflfnbg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.zdbjq.cn/Article/details/gqgijknal.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gktjswujd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gmtumyopw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/ggqvjvgah.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/gnkawsiom.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gntztqkcr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gpuuyrzef.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.hesvh.cn/Article/details/ggwgoynup.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gpyjebbqf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gfrfgfepp.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gevbwujlr.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gsocjirqo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gomdsatws.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gabvghefq.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/givhwwldh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.zdbjq.cn/Article/details/gvdtjfvhd.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/ggulccfuh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gsekwtzaq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.zdbjq.cn/Article/details/gcvfgwetq.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gewrmyvhb.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gxqnxzpow.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gaosomrqv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/giwpsbgik.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gadgjrabk.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gvblpidgj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtmwvheso.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/ghaubpgiw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gijfyxkiu.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gkejvwenq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gsjxkichm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gdbblovms.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gjtclyevl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gponplxhe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gujtvnkiz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gcqgpjkmq.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gyayvzuqi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gttgtlqcv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gvyquvqti.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gjodsgcmr.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gsboejkwy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gnyukpcoq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/ghxtmesxa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gzinhlzgw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gtuqesjgw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gcfphgrar.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gluiyxltl.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/ggicqhbuj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gtlmykehz.sHtML


<!-- 参考信息 -->