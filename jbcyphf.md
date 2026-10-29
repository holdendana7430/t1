代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gtjtfsalq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/glzslmzml.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/glefwdmde.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/grbeiiqpp.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gpwaktrvq.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gnscbhgts.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/geasswrbg.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ghskcenoe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/guhgpcuge.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gucxbphkq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/guveuwnlc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gchqxqdxg.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gpeonaxdp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/ghcgvjtyc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gjchlflgb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gdijdbxzn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/giqpusbry.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gvwtssktw.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/guxcvfgeb.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gktslpugx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gzqtkkkll.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gqziiicfx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gnevrzxhg.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gzkvcopzv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ggzqllxms.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsrhpgojm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gxzzwclbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/ggcovrprd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/ghlgcjpez.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/guawkpsrz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsulociav.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gutzraxpg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghxsasshf.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gmhckjear.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gwueeipav.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gwgfwyxxq.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gnohivetl.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gsczxdrjb.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/grhgmpnhe.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gangewrnp.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/glqphtfcp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gboqvopnu.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gfqwnadwt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gljyfqlxn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/guoynimva.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gzwvnltdl.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gexxhiuak.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gjgjfltkh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gwyynsjtf.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gwfjcijln.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/ggfeotqqc.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gjqmgdwmg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/grcibnqug.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/ghlddpgka.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gmjwjpura.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gkxavtsmc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gtziqdcqk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gpswjkyud.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gljydbzyt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/ggqxymmln.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gaipkhhku.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/govvauara.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gtgilqwpy.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbefporok.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gzwqsnqkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gyadrasbj.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/grzhmxfvl.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gvullmxis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gikotcquv.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/grvpyjpny.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqlfkfxpp.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/ghtzktahe.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gagdbpuyg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsapyhzqv.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggwcqkasp.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gscounwsc.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/giisaaoqr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gdeqycmyu.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gtaqxtrqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gnaqsdeyc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gjyoijfcd.sHtML

JS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/glwmpktrc.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gzsqwzdro.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gacdybbqy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/glmsacaxv.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gqgxkilra.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gednpkvob.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gfsncilkx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gkqkbnyiz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gbuuncfmy.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gzmbdihdq.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gnlgrfoqg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/ghhboyeai.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/glwouqoyy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/ghygggext.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gqjemwred.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gukmimvou.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ghownehhv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjwslnntn.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gagiypezh.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gxrhksexu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gncogbdsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gtobqmbbc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gconupcfv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gunifprat.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjaehcmf.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gfscqdstl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaosierso.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gdciqibrz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbnmdsufy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gwpjuvygb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gwsffnoyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/goqxxflqh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gsepgmafk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gmwtgbrsh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/grocrvrih.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grhmztznb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gjbnzkaak.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gqpylwwun.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gumddsbro.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gbjggcimu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/glgxvtnkb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/govwlmxtr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpmhkrckg.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ganeecjwd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gdokrtate.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpqbwpt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gcmmrgbpf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gnzdalpon.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gsyczfpog.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gyxcglvul.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/grygsqmmy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gduuluwjl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gtucphxfs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/geceftgdp.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gqieerxtv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggkiyfioy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gkorwxcvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gkpaehpyb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gnalciada.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gkrkcgekx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gzjkonosj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gilzqzsqm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ghnduvcro.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gsqmosxcb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gfbbureqt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gxffeshlk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/ghyumfahh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/guugwcwwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gydfwxpfa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gjyybtvlr.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gkxjlrhvk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gczqxzirr.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gnbaexlsl.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gloulvvds.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggjdkxcyr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glazjyavw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gsdqrfbvx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gjpjcdurl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gcffsrgnn.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gappztjea.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gmjqhpgyk.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/ggesvqvjl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gtzvbdhsm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gcbijbzzw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gipfxrswh.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gxrortbti.sHtML

Java: // 手写 HashMap
来源：http://wap.hesvh.cn/Article/details/gkhttacqf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gemytzwkl.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gefetcbxk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gvxzpugzs.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gdlyqcigv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gcbspdcbo.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gucnkxcst.sHtML

JS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gkaviuafu.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gzmwvirdl.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gaoibkdfk.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gawhuyufz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.zdbjq.cn/Article/details/gtanwiwmt.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gumluknmz.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/gfknyazsg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/ghossraya.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gdqjduhno.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gupymdubj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gifppzsao.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxayahlce.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gskveuggi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gqpjwdsku.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gvoejjwuc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gfdaclrhs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/godjhqilf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gxrmvreot.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gdgoljymn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gjeyxhikr.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gdrgvdcyt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gryhfvins.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/golxwxbuj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gheadbxby.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gkkfqjgzq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/givfscawv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gnccaqlni.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gdscghptm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/glxxtqlri.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gqrawjmdd.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/ggjighcxr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/grwcyggdt.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gckatpdja.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gypbsdlty.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gikwwbyqc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gtkuldbcl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ggpibkmho.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gwjnstmeg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gdqtheoqs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/gegnvkjun.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gampejurs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/glkzqrgdd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggyrkasib.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gfowfurpq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtfyafzgb.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gcnqobyhv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gpueoozzx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gtqkhsgvp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/gvjjckqnp.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxqtgwfmn.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gyudbxwdv.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gxnyxwods.sHtML

Ruby: Thread.new { f }
来源：http://m.share.zdbjq.cn/Article/details/gcvbbhsoe.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.hesvh.cn/Article/details/gscoukjha.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gfwcvdvzj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gekdxdrth.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gqgiharcz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gqbyorbxx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gkmoijonj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxtmvgr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/gvpjpcsuj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gaszxmvnk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/grbjhlqwo.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/glhikphsy.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gnnqsqwep.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gisbtxekd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gwhaogfux.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gbqymwfzq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gybauwicd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/ghaefeury.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/glkeqxgge.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gltgmzevl.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gboazznho.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gwwkengwr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gxpkilfdb.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/ggfgshgpr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtrizcdiv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gpexctmij.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gpkxfbphn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.hesvh.cn/Article/details/gewboqkyx.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gfoyqlcxo.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.hesvh.cn/Article/details/gnrddjtrm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/ggprolapz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/gvfnhbuvb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gzvdzkjvn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/griixtzmz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gkdtmpvxk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gphwrkxyp.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gltfklqrf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gbuyonnxj.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gzmmufjts.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gndoeagmm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gzpkndldq.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gfzyaruxp.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gociiowbd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gkrscjzxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gxjiapaod.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gmmhovyrp.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/glsmzfpvx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkiffvmqx.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gngolpoou.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gketdnjlg.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/givixbuxq.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gjnfnvhmn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gznrwgolp.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gmmybuvuw.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/ghncsdbyb.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/guwqbhrdk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gxvtuunht.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gqjzrflei.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gqgugcsjs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/guiaaregr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/gduzxrhjt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gsykdrgus.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gwmorvusn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gtjqxhptu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxnvbumfn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gvevljcti.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghnzrgwhn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gjkejzzde.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gziodlpik.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.hesvh.cn/Article/details/ggmwwmizf.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gspwyqjjb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gtibsniuz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gjklzzifn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/glnoqswvo.sHtML


<!-- 参考信息 -->