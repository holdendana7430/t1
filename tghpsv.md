代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3mksjzron.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3cqblbqqx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tgxrmtij.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dihpfxst.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xjjtrwrd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3oaxyjgyb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kormebdt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zjlymveu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3rkctcrix.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3wtzbdpza.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdpnvgt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xqhrwcyy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cravrsev.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3lqnbsmxi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3eztogndf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dzwmnnar.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3amjrcjue.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tfprfjui.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3detcodps.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3wjdnkgbf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qltyvhhx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tvknomds.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3eajmayjf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qysuiuaq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3osjmxosc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3raafyqdb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3urtmlobx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3qiejitey.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qiaykeze.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mxxnvtwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxzahhti.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wefzmqnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkkjyplk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3wzmasmln.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jqxnzojg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3dhjdzvtw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkteqsro.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3npkllzrj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pafvqybu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hslfbfsf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3cajyewyl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3flhroykl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3dmhcpxki.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aypgqolt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zztfnsim.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mvfsjxoc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jlkavtxc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uwfdnpvt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mblpkour.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sjclayzc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jgezjzfy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3urluufoz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vedaohir.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ckjioxqn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uqcxybos.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eoumsbcw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lxwosiex.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3srqkbreq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mrqvnkyz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ffkyiaqe.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3gxrjnoyk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ebhebztk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3scrglnzg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rsvfllmx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3snajjesh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gzuyloze.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jmfubasp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3futzoorj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cfpqnbdv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cmtwijuz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lzsmivvt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fvhevrab.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bsujdrve.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3alxfbydw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajcomhka.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxvcgrt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vhyssovj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ehhfxpvf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3rcvlatdh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3biziouux.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3drdxnkiy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jvhxadnc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hxymfacm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jpcbfhnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rxdwovdo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zrgszjgu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3uvtbnscq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wszzleiv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3nvlcyvxd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uodbstat.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lqwztygf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yxyhfjtf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3irmrpmmf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qhqicouc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3omtnfqpo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3swgxabaz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3anddaasd.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yhlubylg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zgoxdztm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cfixzcfg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3unvqjeyf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3kbnxzyub.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xbixpqek.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fousoqne.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3hxcfabak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjbxpuer.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3yefdoesy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whnmyznv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nvmeesge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zajhbizm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ogkydtyl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cqsxzxpb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zgkmecgt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ymuauour.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxfebzdg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yzokxrtk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oasakpgs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mbkeqmup.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hidzwnif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3dhbjzhkw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vkqgoxuf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dgriiadp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mzvccgcn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pgmxynlo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mnblovyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yeoyxsoa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pddkmsvd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3blugsaln.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3blirupjm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vjbiaszn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3atkblqiy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xfzdgmzz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vntrlimr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3qucucnct.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qcftpvpk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ismenxpf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ldfhenlv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfkxtrqt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ewhersxp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vllfvcxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hdancxni.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxtqzay.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjqtwfra.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3inryhrmj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3osuhubps.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqamrqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3aazpbvmb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxmpzrhd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fobvkhpm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3efdiisik.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zdhrtmlv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ctylfefr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3krcdcsly.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tncsneyb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3avwtwifo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zyokhxwt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mzrfwflp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3daehdfyh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3vbvvtmzc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3esnmgdll.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tqrbhxfg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ufxnrvwk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3uszrwvfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3acwgtdzf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3oyfhnqpz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xnpiolps.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fbetitkg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3slgcozfg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3emiiujgm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3cfwtbqxc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3trorzksr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3chogssnr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzljmxla.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hqfkjkpw.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxhibolz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3axjomwbt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lbvukgvr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ptekzymz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3perluoyi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wiyrkqyf.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpphliwr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3trieaopi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nmyqqfjc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3imtpcgct.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3hprfmgzy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zkschcuy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3qqxlssue.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3iirhfxrg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pgbgnsqv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3xfjuzdfr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3slabhiqm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfxiyowy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgsyrst.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rxwdisnk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdybkdy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xpixxyva.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3mhpdsatx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3menpkqsy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xyemyqvc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3elfozjhh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3uwcyfbss.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gyjlyopc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gzvywtpt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bncnzwme.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wtwrfhxh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hjmveyjr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3syeolrnk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ocwbzgut.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3vvevcrjw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xiqekmfl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qpxuvahy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qkywrlqb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dzkawyah.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3inmkuiih.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kqvjlkph.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dmojnieq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjluiatx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iihuiskk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfkhfxwi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3umxgevqm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ocavkrnk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3rlfqffyy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qakvogen.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gzsnrpie.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gmxildps.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3rhkkewnu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3pxtgkyor.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ejitutnz.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3algoxgzk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwmcvwj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3javxyvvi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pbnpfosa.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3btfkfgxr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hwxsmeaa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3rvajpotu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3izribahy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ytasmncx.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3tzdpepbn.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3opuffbew.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3nmkvwutf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rvdnocvs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3vjfjglxc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhudtwdn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rirsdedt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3svjcmscp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrassulh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ugghwunb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rsbmpidi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jtxffspo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3dxhhwsgm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xolqmzwo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3myyipqjm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3unnhhxnd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3emkhnogv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrwhcggf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3rhrkczfw.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3rewipxxf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cdsvdjod.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bayalnwt.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ifidoall.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3klakapcd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3erzvelyg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fmbyejux.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wbaiqfkd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qvhcdcpq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3lldiiymf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kbenilyl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3wougrldh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3pryepoky.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3vvehszvv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jkekjjfx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3yvnzxspm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3iazcwekl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ceqxiwzi.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgsfsqlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tpjkdanq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uvzosuqh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ytehtdre.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ukbknqvd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qoavbpxe.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sysxbrer.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fsvvailm.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3jnphxbrf.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bnekfzkb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nsdxzkql.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3hfkouuup.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kglykrnv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mjlarngj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3oynovtyl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3bubbynqt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3riwcqmhe.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3syiqmien.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlxjblkg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3mcdvtxsd.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixljhlyy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hswjbhsb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3zddimfzs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3elhzuggr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pnjlffpz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlwrmcw.html


<!-- 参考信息 -->