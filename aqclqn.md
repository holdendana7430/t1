代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2znldaynh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2rflwxkom.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brvomveu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2oyqmsdrj.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wskvyuuw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dlvyublv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cowynfav.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lwhpffie.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2iqcdeqdj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hyohkako.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dchckytr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ksuekfuo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cbuaacyo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wvbqvxhx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2raffjxpu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tacthfjt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kzrmmbox.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2kwsjmnin.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ejocabix.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2uystaura.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yagmcxxd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bcstzysy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2waiyvtqk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zhvpgifj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2chztqqhj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kcawwbjt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2itocaend.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2twzbmgek.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qkutrxwp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2isxggfuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zirqwrfh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rijrgxqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scdlwbsd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kwqlwlim.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2spxhbfmz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2rzigruqu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2frzerwxx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gdlqmjuk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hgfpcpdr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2aqqsxubi.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yxzjgyde.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lvhdplfz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xfvzgvdq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2srrleafk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dxithhhi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2krmjwrix.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uckextgr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mpmwfprg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rqpnuvxl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bgjvlpry.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2capfifcn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vampygaf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jigokjfc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qlhwjefj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnklsdke.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zgmtcvpv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2txghvdzz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vrkuwkpw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2wuwmodrg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hpbdxuet.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2swwmlypr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxrqfghg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ppsslkcr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cordwgko.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uydivbfn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zgsdfsog.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vxtvyvot.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hmfxykax.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2uixdirrq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cthhgtmh.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vatfoacn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfanyltg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzwmmuqr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qtqtbigm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2marrdlar.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oeftmktd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tghcpvhk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hvwumjef.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ewumopfo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2umgrkiva.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tciahyaa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2okslskat.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2unrntmom.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zpicknxf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kxfutllu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dxlfxrqm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xezrdapg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dalbmuru.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yqmbmapq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2jiqogndv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fmivurye.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wraeqajw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qkzorqjf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qbubwrkm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2glutsuvk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yddhuvvp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rzqgipnf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pmczxrcp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jgmytpsy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2phitnhyb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ykcelxvd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pekjwlia.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2sdmgqjts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ovpmmdwh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jitfjojb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqoyktku.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wqxzvqsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpxmcdzk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nescdfba.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxmzksv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2agenyvdd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2syqqvhlc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2apbtydyn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvppkmza.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nkbxaayw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zuvhdrtk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bubqlvuw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nukgnynz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hldrhxas.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hpjnzwxu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2waiggpuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2joohriuc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bysiyefe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cnpooata.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2smezdcac.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lfkiwmlc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2shqbwhkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2youiilgt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2njvswxme.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ptoyzero.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tysfdgdf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hdwmoczb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2eiljhotc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wqtugrmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2skjfktjl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oofypaue.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dtldeavd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ifcpiesr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aaxrgjgo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wikxhwbj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2crwxbqfe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ihywxctb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jhugymtr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zerirsik.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ygepncgo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gaxorada.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2czmokbhz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2whnpydkp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tucgvafh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hghwjedm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2jahjravw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmyfmwpl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjvgeulr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rznzcjcn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pghnjctd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2elhjccbx.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ahxowtgr.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mexyovvv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qeykjmxm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gembbmbs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xknujqab.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2plkrquqb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fquczaaz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wmxgfwpi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2robemvdi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fdqsreik.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dskcaogp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vtawbctq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hwgclgfp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2jcnwtpyx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uilccxtd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kncsvhrz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bibswpbi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dztaeqly.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hxkkwkej.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kyojodry.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zilvfnkj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lqgmjrqk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mviiczfw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vsojcglt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zcwvpljl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qyvvnzvw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2soryrxhy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kxareylf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2jklgfzse.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vryjvikt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2uvfrejao.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cvyfomuw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2bruhvcyr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jfzaxoze.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2prgjeqsl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgxzxhbh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2okbqttmu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2owevxtdt.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqlniryp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2woyjzdyw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hvyximjd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hptdqahd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2umaorwnr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xltveezn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xuimupfp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2euhfybfl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wxtyckvk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2togcchfc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zuwfjgdm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2mnkeukml.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2eeptposq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2cvkfuwtq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2lykzmolr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wmacshyc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dycupfis.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xnrplwvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bgrncuqy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mhaxpmby.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eunvbajz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hroorvog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcvqngme.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hboldnes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqgjhrfw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ddxaluvt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xwanxpcp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2oqhukvbh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zxzufbmt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sfhibrxq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nwcwayyo.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2byhgdmwg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rmurvmqi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bxpricnd.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zwsmaqkf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2baukkaor.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mpzfeeqd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yhnrbrav.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sscdhxle.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvwkxnt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pgcalcpp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wbzdiwnu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2anecghfb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2bakrhnhn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cbqmkzxw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2otexzdtw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bmthzksw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kxynzmvz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhmscrp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dekeyuds.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zheeldde.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqrkfxsp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dpftntnf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2bfqckxey.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2vjtxivdw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfgorlnl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svlhyklf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jrwjvgua.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jaxyhnfn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2dppsyqbq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ohbzmpeu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2umwdjbly.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vvllsisw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sunijade.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsjgndw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtdjcxw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2lakzjvbc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2anhvvbwt.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sjovbodw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bbsyclfv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2sdvegswf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xledxvct.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2ojxygvse.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gcyjlhbd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lenqginb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2vamoflfe.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2yugfjodh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2guqsrneb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2snaqrndi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gagyixvm.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2fydzsvmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxxfiuor.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2irguqvel.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2lnuqkskj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2nazameqq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kcgayiwi.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pigvucqg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xbnddqql.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mmpigrzf.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zlebobhd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2hpwtzsrw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bvfehjzu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pkmdymqu.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bekbspkz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dpmsmjqr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2grurlppq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mxdtbzdd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qowrmjuf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxszazk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2fidjewjt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfhiiugh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ypyaukig.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2jisugbcf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cnzhetvh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qsfowvpd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cuasnjvz.html


<!-- 参考信息 -->