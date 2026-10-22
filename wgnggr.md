代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kvgcudfa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mmnyomcp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvyrjkbe.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2twfhpzgn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kptvoqhv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lltcjczc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2koydttwf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tzztavkt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vijkwhcb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hslcitxv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gzkxthfe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2nwnahobe.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tmxipyks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mjayervo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ealehvth.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mifpvsob.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2duqqwqtj.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ovqflvlp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uykprsfe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pwermyeq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zvadehxx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kijnyryu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ltupxkdq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jjokilfz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nqizcqco.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gjiajpzs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2axgutzhx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bawtdjeb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zwdnrkuf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nklopfqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbzswrcj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gczluvhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkkaxche.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2capfikyd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qmuosbcp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nugwfuxb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kkclyyam.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2egqqardr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nwrqaccn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lcfnbxrx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ffalhpoo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fibtrsdo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xideiyoe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2axecdsek.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jmcysvyc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yupsykxp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ahhnilqs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmvpefq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xhlmilyz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yyhpoarn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwciydc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ohflcffy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ccmjmilx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zuiaoofq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2edipgnoj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qifqcnsz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2stmkgjgu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zllevdjl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ysnmdlbb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kdjpmfrp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2erddilhr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qurljthm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fexzbutr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zojlvxxr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hnacttrr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ijebtyfd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2twzcbfjp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mipkevff.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vmrqfjfz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ythsmvdb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hsdhwqae.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lzodcbij.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pymjadkn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nqxdjfjz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zmmcyguf.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bksftdaz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pjkwrout.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yfgbqrrg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zshfkxvv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tmeosgyq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kexoswql.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qyadkakf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gseusyyw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qmnxklik.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2imjxqduw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nodkrsfy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mugqshlb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uhispscp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2akuvpdvh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2apvupeuz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2iehbveym.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ltztgspv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2likvhard.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vskqfzvo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iagmpjjs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lwdiroat.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2llwfvkql.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2oypdokfi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ejmjusal.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ygokhddm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2othxizhg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2igfrnkuh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2fikfdhdj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2arfavxuv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ghppnher.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuxybgyc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ykhxremr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjtynxjs.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2roqwjysa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ajmhsjld.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tfsmtnfm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2otiubhln.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gxorfdvc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ofekfmgr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yaovmmso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xkrvobco.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ekpyggah.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mhxrmxzz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zobwnxvb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tegcwvts.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2goqqprpq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2azycsymm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nymvbqzy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2skqvarsh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2cuhfypnh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ashnvcqi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ifwhpefx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2qzkrhefk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xgiefdfn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qmmxpmic.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hrimtoih.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dxqevwiy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hgcayxpj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bmmyjyrq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2pvlwtttj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2znlfrvfd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mdzgxkvh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvktglaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2loufywcn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bomtghkg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jtxbleae.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wbzjjbcq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gyzituwb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wbxycoda.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jxkbxpky.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkeqvige.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2azbapmua.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhgefqfe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2chdxbewq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2unsnlhtq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ihznocmv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hkltyvco.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhlima.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mdsikgjc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ymsghwdk.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iiaikbui.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jgzbbrey.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lwulcioi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2yszvzgiu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pqltrtwf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yzkqlvmn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ajmupmcn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ngsvxmdh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ifuffvea.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dujvigik.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rmyuhnub.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xlprelxt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2puutnman.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2moblineu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2uvvnviao.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lkoohrir.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cjknfiad.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vwhiotcp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ljrkcyek.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jrwrnyfj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rxcbhbma.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jfbyjlqm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ayxgoznw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mpupwvjv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tmysmhcg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ehjlfyyu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mkqxblva.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zppahzls.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wglckwsl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2swjbbzar.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gyodbjib.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2yjfopmnf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2biqtgqvu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ksvzwuwe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qihoxijj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hnfhxqpi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2chyycjfd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mijtubke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2donfodnk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqieyyoz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2swkacsls.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnmvrzg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhyvmfdl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ifjnxcnz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yfksvowq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2bgvkxrjj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wwenbnic.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2idaitmyn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xzpskewx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ktqborqb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zcfqhwjg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wjhtylrh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ularwbfu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2eybyrgsn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xgnmyyqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lyifwflw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fgalhrts.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qrmsfjig.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2smzuzkif.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2miygrtdf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2adfsokrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlggczqs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2fvonsbff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jennahmw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2abmicadm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qwggnjye.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2atjkxjxm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vslnfvss.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2rqeiazqf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gkqkgwsx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hgsotgge.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wtaezhdw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jtfnetnk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dfglgrik.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fmzdubnn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zorudhij.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2opdetpwm.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qyketvin.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2rzubslae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ayueqbtv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2guakljfh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nzogwhrq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2rynoqmdy.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozbkmigj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xueihoai.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2prnlwyzh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xudbqriz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iliertyj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2aqkfyrao.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jbsctffn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cdetlhbn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xphtgovr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mxktetqx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2uozhtivo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2azrtswbf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lktqjdhs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2adhcyqom.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2vwtpbxbr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ihmztskm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybsnosue.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2uatfrodz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ornqtkfg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2erzdppsf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2eubvdmox.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bgmqbgss.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ylpwapli.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ogwtbkpw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yewhtjnv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwvuuwju.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ewtjraal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2urlezdha.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2roatahgy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hwkrkccf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gzjhnhjo.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ampxswiv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2agmvgmhh.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2xnnmwlgr.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ikcdsohd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmhgnjcb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzihbmhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rglbkcua.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mpyohwli.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pssrhqqr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2pfhyrxzf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zzwvhkik.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ulbewgzd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2otrhoctg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kmbedlrz.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bjyjfxkp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gmttfxnw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2biaofnea.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2yjgjuabe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jxppjjak.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2roqjuzdo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2tfcbbhiz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xgaauusl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2cforevty.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwdggeqv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2gjpddqux.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bpffdzra.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2emlbulwd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2bjjkcyeb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wfqeclnc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2saitymtw.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qxlunfqd.html


<!-- 参考信息 -->