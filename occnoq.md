代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vvmisgnh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fazykndr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xmqbeuiz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jmigjfey.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mnbdlbbs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3seegkqck.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3phxkugtv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3rxlphbyo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dxvihxfx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3eothdate.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3amuojkhk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3asukhssw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pxbqhtso.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3lfbnsmnh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3edblwmgy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3fmptaupc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iifnfhyl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ftckskqu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ylkobcio.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3uuzyfsgu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3phrzqjnk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ewpqcsjj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pmlgrzee.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qgcxjzts.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3fbnaspxn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ucgvdlqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axztgibv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ixoqhoee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkqqbmcu.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ldqddwfi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3bnwwfwvc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fihmdlyl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nkzcogzl.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rqchcjse.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3myrptplc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3reahgwjc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ekkkwvrm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zwfznhhr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3smvuenfs.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3esluuign.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fcasnpmo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mwdbpnqf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3redtyrej.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zsrcaiuu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xkdmskjh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vhwvkzbf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cbkgmyau.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oiwyighb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3desmjjgb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ktpqqagu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mcxergwj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dnvxcirb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ulztzjli.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dsejksvi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tyyhfmei.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dekneore.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lpaqbuax.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zefbpacg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hnuiiiss.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vysrmrku.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cvbchcuv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rweadiew.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mujkypot.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hgviridi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dxzzjgwk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kpgscbzg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dqfvgzyl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3yqnmmqoo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enanbwrk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiljstf.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkvbnqe.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihrrzlqt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zueghpbd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3diaamwdx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3athwzbpj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mepssxwd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3woehdclp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nlegbitd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zirujuhq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3pqhqjddb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3agonbspx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zqdxnpcp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zwgbocgo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3woxnmlko.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3rzqndshu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gnltcrei.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wyizhyrb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3drdktskb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ujhrmemb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3eamyaewv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3aqqnxrcw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3fopgqcuz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vkqltkng.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fcjdbbnr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3rrbzhqju.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jbphncpo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pfsckjtl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mlyueikj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3fmbdqflf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3zcpmloim.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hgheubnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsnhrnxb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ghbcsdpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwtgixus.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3zgqsjuss.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3irkpwfcd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xzhpkpjd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wqhndnhu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mcjufmnu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbmwjvoz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3htxmoxik.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3orxnanmb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnzdczfh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dxxcdndo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zpfzjeil.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfixbced.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3nfqtgjau.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3aenzqxcl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdnzoct.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kovocskx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vidhfwnk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pmbumicz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ssmgbrtu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3railjjqk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pxsjyedj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zlhdiybw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xroavtlh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3usoxkmzd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ozwzsbzw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zmzmscmg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3uglxiqld.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3igakszbc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nzwbjhep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3umpsrrjc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dqvmrctr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rfllgyms.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftdjlrpm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xvwykiay.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nrcsxwsd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ffetbfdy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pnbvhurt.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvslaoc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oduwloud.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3duoogpti.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3tpbkgaze.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3wzqzcfck.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3crvjtbtp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dolpscbg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3lldmvifd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sanyymxy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kotepzwm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lhvhcuds.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iupwrjom.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gerrjyss.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3qztduzka.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zqxvquix.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3pneexsue.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qylypnzc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3qlvasios.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3whsuhdxi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3vdcewpyl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jgwmykmf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3vcdaubpj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3pxanlwyv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ccpymvuj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tsmpivpg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3tbwktyqj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3eddaoomy.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wegrkvoc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3arxkpibp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3owocguea.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3epojcfnt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qqiehegb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xedcmpwi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lbmmlezu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dejbpmwm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hhbohtbs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sgxolipp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ngnpvhoc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhxhrorg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3dqtwwniy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3jhctcgpa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bhwowkgt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ulvraakq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3arsigotv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vugoqmcu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bqydbvnx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qulchfar.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dxrcsgfs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ljaoupvi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3vabwvorb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3yivjizzm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3zkjqwoma.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjrtkwwx.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3uwocpawc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gdluxozw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3lojeetrf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uigzaftg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mzysvaog.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qlqtzfck.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ekibfqvb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nwwuyryw.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vmiwefru.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3njppacmw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3flbknhkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zkhbeved.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hivezicq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cmywsnro.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kivxedem.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3txchtfyp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bboadtel.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kstlehri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytahdwvq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3unjmfxhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygsnrzzt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3nelgcfpf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3isjnsyuf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bnhogpfn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3lvhybmdc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3iwnfjjmf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cmiiuszt.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3skehadrk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3rtotliss.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wpghylwq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3sccswneq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tvrdstkm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xxvuszoz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kedzenlx.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wmniausj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jhkwzevw.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3oicemcfh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gnsjuxjl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ldeowvfo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3foxezwmt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ltdyacod.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ihlxcsgx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3xwuzorcl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xfqhxsln.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3advycbqk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3cxqymafd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bigksuja.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zsnfvymr.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3glvsptvj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3djczshgz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3jgirdycj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3phxdvcgs.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwhmukeb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3mbizzxln.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3xcrclous.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xekovmmd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3rsqveyjg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3smxwxuwb.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfidbms.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3qnypbdft.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ghzhfspb.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bemqvxfc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dlwxswpn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3moviujem.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrvrjsy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3yestvmyp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jtdcqvxd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3vhbtgvrl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3utanjird.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vpewcejk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hoaqilsy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bmkttkdp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3bqllmdeu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3mesbbtod.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3itwidbgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxfuogtw.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3kztunwwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnusvrax.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3okklewcp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3rctzewjv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3loigqlqx.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vlibqihu.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fzkbivcp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3adtvuokl.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ztrkkmbo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3cihtnhhd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sbgdombe.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3erxmdvjj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3qlttxulf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hopiwkos.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3doranyuo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3zdnxbjjm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3flrhbjyb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ulonlhof.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujelkhvx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ddutbpxx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3izawjhop.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3nlpcxini.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3fobhoyao.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3azgfpoys.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bzwsqvek.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3muffvvpn.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3weuutbfm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3bwatdqou.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dxsorqwc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mqpzahob.html


<!-- 参考信息 -->