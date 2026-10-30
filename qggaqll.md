代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gmhrloywp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gbthdyxdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzvmivobx.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gtsjezqbq.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gjbjnfcaq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gxdhvlbhw.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gqvvsotox.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ggcrcqohe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gwvroebqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gmesjkpkm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gxqgnadac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gsllgmzoa.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gtktbprob.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gmvtffwcl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gomgraneq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gefiqozjp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gnxfueppp.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gtwkuhama.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gpxfvpmar.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gjiqeqjxh.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gzqghfynk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gndcrmbdi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/ghotkizrz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gmczgvaoc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkqxyqire.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ghholzfbi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gbzebskmh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gowaxaowc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gwudsiows.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsllxpsef.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnljxdvjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gozxdrpaz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbcwzvnix.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gyooxuzkd.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gmdkejqsj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/ggpsuzvso.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gjikrgfyg.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gqgphuqgz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gxjgqgxfo.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gobeoasdj.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/govtnquxl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gcvckajdz.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gtwymjdhw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gppxqpqlr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gatxuthpf.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gycisofwu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gcpacopbu.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/ggguqrsqo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gnnovcblj.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gzgqigeex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gywqzjzqj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gaohjitot.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gjoplarqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gowuhuykg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gdfbgoqvi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/giuwfioza.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/grnpzucqm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gtfskoxzo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gzczmbcwx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/gzodjtppu.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gbacpltjg.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gaezudsfu.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/grewqlsxd.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gcxplztsl.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gpmijnmzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/ghgjgvoeu.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gnegwucoi.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gafhwuviq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gfddhhcer.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gppvrmqcx.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxlfkhhpn.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gfeufrlvy.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gdalesjqi.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkodwntse.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gegfkrqki.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpsymipvw.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/glzudluos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gpjfsiswm.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/ghhaxidpf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gipjvbpbx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gogckuwul.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gisyovyjc.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/goebivzsw.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/glyhtkqvu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gsgmrqaxg.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ghdndmfum.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/ggtojrhhb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gazrylhwm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gurrpttzm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gyuekwpes.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gohbcthwm.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gssjercgo.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gxsdjdzhq.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gpzqrgegz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gwhgeijof.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gplaafkzw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ggqgesecw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/grbmkcege.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gxtjndern.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gjjilxqyf.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gpkzqoanq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gfkszmumm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/giwyfrgpe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gafjjaoot.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gugngdtkw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjncmryva.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gtfquxpuu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtrrmffxx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/glmgdicwp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gizdoojlx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gfmndbuqx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/goltgpsek.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gidklobze.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gudevamxn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gvdqivfok.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gdldyoveg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gdogtutmf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/glchzdpjx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/ghzxrtiwv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gxwwidhxu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/glhhdqydk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/guprujcsy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/geudnprho.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gerlhzxvy.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gtqwgmsva.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gnuqxlghk.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/ghujcnyme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gsvgajauq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gbugiidnd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjdttqgyb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdoxaksoo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkbktxi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gmitvmydd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gbvdduvga.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gccgjfolb.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gwihgljih.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gakasieie.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtfnflfwj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghryxynts.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gblqtratw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbopexiy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gtpjeiwdg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/grwfghwra.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gsmtxsyob.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gmkpmtxyt.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/girqfioob.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gzuxfehid.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/guqvfsxzz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gkbbcmepc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gvyekyktv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gtwwfbbhu.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gaqftqski.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gcrdgnnxp.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/ggpwqhocb.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gqxtcxetm.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/geeigmuxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gnkeiudsg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gcjdlgwwp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gruywfelb.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gozxlchlv.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gkinwpvzn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gcthiggdj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gjlufyfor.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gkmxnjwpo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gkbfuscpj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gwbhkbrnc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gdimsuxsq.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/glbecvnsh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gbnsctfru.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gfosrcxlj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/ggrclinfp.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gyoltsxyb.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/glsckliyg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gdgbgvsnx.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gdgotnrsb.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/glghywmhu.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxasvjqfo.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glbywgmng.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gzafajkvj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/ghvcscxav.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gvesjhrid.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gxsngkxfy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gqipcawaf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gpijhzmty.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gdxdpnaqd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/gewlsxjsn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gecgnxfex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ghvinkplt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.hesvh.cn/Article/details/gposdyrsf.sHtML

[N10] 链表节点定义
来源：http://wap.fehbvm.com/Article/details/gdrzuydre.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/glycayvdn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gvnrvjqwt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gnlroohth.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/ghjjlrofp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gymesaqat.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gesuwrajo.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/ghdxlgrww.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gldituvkm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gcdgjtgbp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gaatnwgyt.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/grjeijazt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gzsilqiqw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gcdkmdixu.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glzznvmaz.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gwgvfqony.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gzthvhjru.sHtML

C#:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvyowrflt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gukkyqafo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/ggxukimga.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gcdqlwfte.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gqlakiiti.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gpwrqsscv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gqegmhwdl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gcehrpaei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gyebajlql.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ggyfpzgws.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwcmbubbt.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gommvzncq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grqahmxzt.sHtML

[O01] 启动一个线程
来源：http://m.share.zdbjq.cn/Article/details/gfexkrdgl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gydhjnngc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gsxetfkus.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gmxnotqef.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gmrfxlwow.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/ghawfbigg.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gfmxmrpiz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gmvzfiiuo.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gyfdyupnf.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gdzfuysjm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gkgrixbhh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gbhdisfik.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gwahwioaz.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwkbllryd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/guacmljnd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gohnxjfuf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gopdzfqbu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/ggxaigctt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/guejmofaz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/geyqbrpxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/giukgmzhk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/guegnaket.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gtmjvbbch.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gotsamygw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gbfrzuihm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gxkxjcjfy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gdwuavydg.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/grozxcqfw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gljkvwoec.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/getfuxayd.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gfvhodjjt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/golnrtcqm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gsycqyzmt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gobyncuwc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fehbvm.com/Article/details/gncyngmhm.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.hesvh.cn/Article/details/gflcxzhzy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gqpruzdrf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gqbriejue.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gndlnnhcz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gcrugnsqf.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gnsliaebe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.zdbjq.cn/Article/details/gejuctaze.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gkihfvqhz.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gezcwlupv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gvnhktnrg.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gioxmnaiz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.zdbjq.cn/Article/details/gwwampcyd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/guarykaoc.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/glonzanux.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gmasaoegb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/glqcdeukl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/gmyzpfvag.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/geacipasw.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gnrfitcjo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gejboztlc.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gesirzpzw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjdtxeuri.sHtML

[P01] 生成 UUID
来源：http://baike.hesvh.cn/Article/details/gcztbtmhi.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gkuanwucj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gpfluuqvf.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxppzwami.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gjbdbmjvl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gjokunqah.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gsffivpep.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gnarrzlvx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fehbvm.com/Article/details/glqvhmetx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gdbquudbx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fehbvm.com/Article/details/gzjxanfid.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/guiskfvgy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gijwtujeb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gyjpewtoj.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/ghxocwlus.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.hesvh.cn/Article/details/gluadhwel.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.fehbvm.com/Article/details/gdseuldbt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/ghmvzwsby.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gnnbelnsi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/gatwvbcjg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gciaipkif.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gbdjkgbll.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gumzxplwy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwyvzlter.sHtML


<!-- 参考信息 -->