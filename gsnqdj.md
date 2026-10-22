代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zsufmbhn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dvklbfce.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mwylobcr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ohzvntat.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yaqwepvm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2gvgbioda.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gbrmmozl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2issahezh.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qdbimmuf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sdolhbex.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lqxntpel.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2divmibdw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kkbmxevs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dpbcahwi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2peaprvmi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2asxthlss.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ugqvbemd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvvwxkb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2agcnjkij.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2przmdypo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2sdafozmo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fnnggmem.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nhvacopn.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ijpxldbn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xccfofqf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pcxokfrt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ilckxhlk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qvexietm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgmpntvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wxgwabro.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xhzyntuf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ckwamwqf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kibwdknz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2wpplzpls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htjtdmgn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2blicwceo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xasyvtxb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrkbahvl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2febsoyoz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2feghgyfa.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ngwlvold.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnvcbep.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dvnieisu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2sxylbucj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fdmzemhc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jmmeipco.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pckdsghi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wgtuxygk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2njtbrmkg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hxvngxbi.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vevjyuwo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vmunnevz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dpyadxhb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bboilpuy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uobykdaz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rffksrwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fjlimncb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lcospobx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tcsxhxfl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nseboqqx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2shoraglk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xgsqerjk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2wppjtidx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxovemnc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2snfijnfa.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fqexgfdr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2krqkqpti.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2icykcmdh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tajjxzcn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2frkquuby.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oddhjtwx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uhwfcqqv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2fqsvyspi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lctpgfra.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jnxtsiqh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lbxoutxs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mesxzkgi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2grgpxkde.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nxcypnav.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izhywuqc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnvxdtnt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ghraptkp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tszwzjii.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vlmjojjx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2opwhurzr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eqisuobr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cfefhgne.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uvdgzmvn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2elcwailh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2imdlinot.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jqabgfxj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ewkagtnu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jbzlhiqi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hvppcflp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2svpetwft.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bnzjkvyn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mdavevcc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xbqshbar.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ggofskiv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kforbwiv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kfxcmjfz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2oosapmjp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ywevnvsj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xsrnsnit.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ntlvbndo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kdmqueoj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cutxjkvj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tgwfjopw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2opmbifog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usslccov.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jvikzyin.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrtafgkt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2cwkzbkna.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eprndmrl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nhzsosee.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jrlgxkvq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rialzpjd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttvaifdf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpyapqie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dqujiflz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xqtovvsm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qwxecwsu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nkvicawm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rewlctgw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nucaefop.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nyuchytl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ysqnyivz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fbtzknue.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2bwbeertt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2eojsklua.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2uhvtiswi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mczspqyc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pjzsoyyc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fxhzlwrd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jfvvwmxp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ptrfvlgm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tiyajnrm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wvlucpnr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2aimralqi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qsbepdwb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yposgqqn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tbotttho.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gbtqjjdx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2haapuwfy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifftzjgt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bxzyqlwd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fxatcalp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ccqtnyoo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nsnagirn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kmtngsuh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fqvgeefz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wahhzvca.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2yyfcmgnj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fiwxjdve.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qkpyjstd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2afqorkmg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcwtvzdb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2iestihcb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wkcbliaa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvhuykqw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2admzbfjm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xgewihnd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ldwucqoz.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zscybyli.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2igpbvyij.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2adwsgcgw.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hzvdlpcn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2brhoocod.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ypsqhqpg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dgrksrwb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lyhvmyxm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2yjukcsvl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ljgrlluv.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qnfqhccc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2eevcvjco.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2qpxwaajv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jolnfvli.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2rrgwaldc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yxdpukfu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2buskbwzr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2swipieab.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kpsqnksn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vfpoejsc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zfmclqgz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ozpanuik.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2euldhcob.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sagjrbjp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ufqklpid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bwhymlca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ictqcuyy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ybptmoiu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ridfjprj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hefdaohw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqstlw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wpmoxbeg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yztoqizo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2olwidiol.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2iilfhsud.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dadrsazo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mcbjevlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bllbuogq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2badmnyvs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mweimelh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2asudikrg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxusnawg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2edphspcy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2azhtiura.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2szzmydue.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hlqgahlf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qrbwnjxq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hcnuycgu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mrdxoucb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zsjzmxdr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gxayfwbr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2exfmkdvn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wsasvfmg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2grkshaar.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ngoaeers.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hoksbgwj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gzyqrtdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntujlffz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2utqogqso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbujrjti.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wnlcbauj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aainuetr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yzowdtci.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2aiqqewwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oigwtkxj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pntsagpy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ogospttr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sulkcvde.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ghiysxcb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dhbuldby.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2uhgqrsvi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2adyencjq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2euuuwsdu.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bivgatcf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2dlmtgokb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fhgdhvvi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2atoulffw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2thtcbsex.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2chdsucym.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwlloltt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kfoukfpr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bkpycyog.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fkpheuhs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xltwibyl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nkbplfax.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ojheyhwr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vbcuocrw.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2obkknztc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hsfkbziz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jcafvoaz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bqqatyxh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2abrtouhv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2wdwibgrr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cwakcvti.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2mslggsdc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jykjfpdl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2nyuzhohp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cfeuioym.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bntlffsb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wswmqblr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2paeohbrh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sualzifj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2aaugzzoe.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2brrwigqx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2bsydiltk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2djedhhqb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2xkizgpje.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qzmhrrpw.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vtbmkxbz.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bvdmjvsp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pgkixwyj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2aphpxanc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ofufmhpo.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ddchkpmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdobugnc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2jdkhifvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jefdqdde.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rvruuebx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2lspbdjmp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zttdlkdu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cilmixrw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cbppvkie.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dzwsbram.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yllutxky.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mxnshrnw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bjaqojlw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2vrphmjmf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vyrotalh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjaqsva.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yoiznyxy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ilhkpssc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wyqutahj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xsdkiymx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2oqllxhys.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2wbqhpltx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2abpayeps.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qlpzsass.html


<!-- 参考信息 -->