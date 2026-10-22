代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2upkcmdjq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2megvhpxo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2fsyebqzc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zztpgpkm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ihensclq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tzehhtnw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ffyaynbo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vtunypls.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qwtwcety.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nfsacdeu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tezauccf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2uqapvncj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2plmtqskp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2svhngvjv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cujabaqr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2fjhsdalu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2siiksiql.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jugwmzui.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bpsubzhc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rkalhzmb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2utxljkwl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2iohrbxwb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dexurogd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qfjyubxx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pvuppmsc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vrjiqonq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2epqvrckb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jlegpmsw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dmsljncv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zqygwsxv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2epivxmeb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2fsoauvph.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kdihnkja.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hsucbcik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rkdylkjn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bhxdkkhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulschdpy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ypybtrgh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mufarvzp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2zofxdvcb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttjgxxbu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lacguzlk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2aabgwjdq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qoyaanxy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ntjwqpst.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gqxgixtx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcwcrdpg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rgggiqqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fqgawxua.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cguxpjdx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rgndqzhf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yvgvpppj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xiedgjby.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vqcbtbyx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yhbymkbc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bnhhkwtg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fkrvlbxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sjvxdojb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbuvirtn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sxeeghfv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fshxakbt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ghtubrpi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kxqthiin.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bzlnzaaj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2kredpdju.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2cmizqpzl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2docqsudz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ibfbkjpo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vnieotze.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zmxyonjm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ckwmggfs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lhemiqxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sndwspwx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xwnrkycl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zrznwmnw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vbdsagve.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlrfzhz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wvatyrfl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uwagvyye.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmrytfsn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pbgeqlzz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2hbwqbokk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2kskkafxk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jauxqfcf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yvehnmgn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osjamhsn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zgycuwds.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2npywgizm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2axnylxnb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dvakvyii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2knyjfzsp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ntawjdgg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2puxaxird.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vctjvvqx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ffuzcbyz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uqkogsja.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xobryabx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mzndlhzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fxybcmiq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kuollgjc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2dcvuekrw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ajaqviep.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dwohosvd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xyspkher.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wqxntviu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ospksftk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2xuhpscnq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ohuycadq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yhswgrzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2govfxrlx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kkhdjtcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quatmamm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xzujvkys.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zeisogji.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lxzkpjkm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2scyvgfhq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2tyxdrssl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2olmequuw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqmxgmws.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2pgfwsoli.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pgwtgpyb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dnhyazji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mrmzprhl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2nscesxef.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ehogrhuj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sxqjhqgk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pqiiqwfd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sqqylkio.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lsxthdsm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qbrplhqw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ijsjlkgm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2unryjgcv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gbpijpmy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dlwwpspk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cdpmdxwj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fmcdhgpe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2odfmkqhs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ekmyepzf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2okqmfkfs.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2snciodfj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zbchiphj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jnhnoepn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xhcvdayo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pikfwgay.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahtsgjzb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2iyfcdpje.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jvpsiiau.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ihhvtgzh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wlysdulc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sehqphhl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kyufoflz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mucfoame.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fgnzoutw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2csmrvoik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzdotfyo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2buejrbbg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2szkkqljo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hnpgzkhm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jsloumsr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rchxrzrh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2axmzmign.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mregtceh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hpokcdev.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ubuaqxfd.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rqulqlhz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tfyamcjn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eaorblgd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kqyetoyu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ycxbhvck.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2plhbtivd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ttgrvdfa.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qediixfc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2otwkozjo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hvlhctsq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2hqxepnsb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wvdfvkkf.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfufjns.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2lmgrwpbw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2smxkpvvp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uopdncqc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nywvpqtz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qyvmenoe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kghhlsql.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2avypchxm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mafporhg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uowhzqix.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tprqetxo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jepewhkf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2oeffysfz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rguiykqh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2mfdevnya.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ocvhihlf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2vfqrqlwy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2tftxtnzq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2pafcramw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjyyfzlm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2poiqxcls.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uuhplero.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2meyrsmtj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2nregjjqx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2egkhtlcc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2jfgsrrjs.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ogbefoyd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2kqfaqmoo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fzxbtwqs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xuwuuhfy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tsvydqzn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nozdtyfi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qbktsvjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mmviawwa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2azcdvtll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2njqxbowh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2odhjxtbt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yfbsppzz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sgdrgaxe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2hufxntll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2omglritx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wtqoocie.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxwvsdr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2rgzdmrin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgcllewu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2mgluomsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftaiespg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dtvcitsk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2sukqerzg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2uxyumxqq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ruuajjcs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dhfworiz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jchvbpgh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ehdeobmq.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvhyofw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sekfvzhx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rgxbucer.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2kjnxdgko.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xlsueupy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uthvdmvm.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2otulvdvf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2pzsikasy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2qggdvdnk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2zixekorv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2pouzsxqj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ooashcjq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2psezanha.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dospnwyv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fuayxndy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ytsitptb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqjclrgi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2kilmeznt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2gymowrev.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxedoykr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ygmtidwq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rzzetqjh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2neyjtknf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuantilb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ziqkrwsw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2bfcdqnbp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2tsuzqdxg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hxmcmnza.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwnragkr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fyoocwoi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ucuidtbf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ibalsnmr.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2mofrohod.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2xcomljru.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fcbwbcna.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hapbeykp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2svkuqhup.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gxycriuv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2aguknibv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2tqisrjle.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxwlljbp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tbjhtiym.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2pmghowry.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2bywvkorz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2oxxgrsab.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rnqplstw.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2rrmyjdro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naiukdhj.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ujmzjkri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agdggysj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2chtnxtyg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2avehwjfc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fjarjbgj.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qhaxrvop.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xholubbc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hyjkkrxv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ykehnnen.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yhdajqcx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2aieueuwf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2fojcrcpj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2trkgxwut.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2tysdljqd.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qjhljxkt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2gfhbpqmf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uwjjzmsv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2srzpchkc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ussuogsu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2lwvfdfqk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2jkpxsjfd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2msxzkilv.html


<!-- 参考信息 -->