代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3cspphbyp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3gnluokdw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3omogxqbc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mcuplxxa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vepjdlie.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mdnkisml.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tlpjlvzn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kgzoyybq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zfwnbyuq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgyumtr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ulidldoz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxvosuc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bhswkbhv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wzhjxxev.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3owqroasi.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vwmpihfl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ooeoafdp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3elldqpai.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kbhkwwhn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xjklontf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vvrholdi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3gexmzetf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3liunkljy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wdqistdb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yrepeacq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tcfotlul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pzoaypro.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bzgpvhxd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3snrfpoxx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lxqscztz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktbaeqss.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ifsgxvww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sxigucpe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qpgumybk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nxitjdsb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fcocoopc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dmvzngzi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3imwmwthw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iiygswpk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3omcfpzyg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ciqeuctf.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gjdqrkta.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xekhgjek.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zhecvsgf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xlkixtxx.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kypistbl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3pqebssix.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yofjiwkp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xexmsebo.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ainiayli.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubefryah.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xctaymxz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ripqabde.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3kggdfrgt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ibityxbx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3crfpbjya.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3fgwbjdul.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qvskgxay.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gxacdubu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3exupwctw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3edujoavo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3titjwzyr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pdqunvhb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cvnwksdw.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qrjghjog.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3oukwrnvq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zpciasbh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3voodakvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kjrtimft.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3afxlazgd.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqhpzexe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qgbxzfct.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhbokegj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3krbewlzk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3keywwswu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cqkeooqm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3oaohifdl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3umpmchtt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3qdcnhvbo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gswolorh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nunqbhmp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3klbsqlxb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wdlhggdb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zfqkcgin.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vrjwqyru.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mrtpctpz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3utqkajyp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fxaedbxs.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3vzpieapc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dwekcfbd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qhaswawr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qcfzzgch.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nygpisbi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3kvcztupy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ppwiibdi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hcamnmuh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3duzycjny.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3skxzzzxu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3oisnfyvn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ldrwpgkm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ixclvguv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3hzfvnnoy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kxkwwuih.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rikubqbs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3cijahdtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbcmyhpb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3trhyqytl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znzwzxzt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qfxderwi.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lkekyisq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3agfcnbmb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hyywwubn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ttkfvfyy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3echfqryd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rltxpsvy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ruzmlhlz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuvmoaoq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3usviqtow.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3uhfyamzx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pojzixlr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxenzpw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dqlaqeuu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yqdicezj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzaphabu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3kpbyoxot.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hicrrqgz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3nnkuhuvb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3smbaxela.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3xulhhdcj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3amyjtslr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xymohqlg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lubzeecv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sqflykjy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uayaawsh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgbmft.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mdarablj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzwsnhdq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3jvqpcxpm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mnjlbtzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3maouvmjf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3dmmrrfup.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3icrtjugr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmehvpw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3elwkbcox.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ttdkwbev.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kawlsqcy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3adaptfyu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3blstvcgq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnwgrpvo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3nfekzbwj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mbkfzfjc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sukdmyqx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3edwjdgxf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aprgouqe.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3jrmbtzcn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3utilkdrs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gtkftfti.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xvmenruh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3skojkpky.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3nnsrdxnm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3srwnczvx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3myblacct.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ygkzcnyf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rxhgpegi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tbsiysep.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvsnvfd.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3siyazwus.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nwaohhjl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3fuccqsaf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3absjsmlj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ewaghgen.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lsnuxzxy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3murygfek.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cbytuweo.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jzsytmfs.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jamucvyq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3abdndmug.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yjvavnke.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kengewim.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gyjoxyqu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3womzxjut.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fcgqrgss.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ermmtpoy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fnskfnuo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ovultihk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3prpudupw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vglbnlky.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zzapkqod.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sbpmkgdj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3nbymcegi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3xlhxmzjm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3iftzyvci.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hugdatma.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3armjhehh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwitfnz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3npczrlmd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xknuvaxe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3snwudnow.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pspcysmk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3dlceakks.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gbjoxwmo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fqygeibv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bexgminf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jygpggsi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3agspzsof.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3pxknbcip.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3pwmtjcul.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3zypqagfd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3icrhaadh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wbdprehq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bxzodcru.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3autcrvmc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hiohetoa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ykxytcsx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ujqwaxqo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nsqlnarn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbisvcbw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3plmeehpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gptfxmgh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ykqbhgto.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fyslatkl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fojmudfs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3klksshpc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ecmgdkxl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ltkequse.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3anhrbbsi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pbruwejq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rdldyoqx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wnszbgjz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3wclxlliq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3vbusfnzt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pbonvkeh.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vyohyroo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3tdgclwhk.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cbzmpnmd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3fxkdxbho.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tenwytkx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3nhhbtlvi.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdsiznck.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pagajxyl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mwwfryht.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bgstaqdz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3egvjseht.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yysxxhyj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3kswafgtc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ubitokjp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3sppglurk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3osixnsio.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3exfaeckt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3umsvhecd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxvahsw.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hwljebmw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ogaczstd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fmrgytoh.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdhhoxph.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3thhjmyje.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3smbdmuvt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3wuwtcldi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dhgnlaul.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jnlupotl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3cayumpkg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wjtmrmzj.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3scwckcin.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kffikrgm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3idsknunc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3liinpnfy.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3abzkbrfv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wrbjasjf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3mbllwelj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3oupmwnee.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3koaaqbnr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vqtlwttx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3bvufdeot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxmgeowx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3vifdowrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dewslwcj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pdmeuoxe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hhbastyh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3pjrphnme.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zoyrivws.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gmwwmdyq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3thibcqdd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hhauztqg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jxrknsfr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qfdhieoi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3assiwing.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3agxfnrqw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zmlziolu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kpfcovxg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3oddxtemp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3abgitpgh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3idzbjpnu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kkhfarzd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wdwpmqqv.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npoyacnw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3orjobhnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ymairtxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3axxzpasp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3jvqxceey.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qpeclanb.html


<!-- 参考信息 -->