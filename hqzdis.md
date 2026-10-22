代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wycdcutj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bbbaktgv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ztqwiupw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ndchkjru.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sokvqzdx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2qhiiwqmd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oknhmckw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bsedyiwc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iuigwvqp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2orvjmzda.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2czdxcnik.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qxjplczr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qffadhtl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wsvpvruz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xtpwrwzy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lxhcntmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rieglmiv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2efyoizwt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qecsnjwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2egzlkikv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vgrgvcpi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kyehhekw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yitdrtbj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tnevstmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dtmotwlm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nwrkhfcn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dotrhimw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wdtjojho.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nkhkthrn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qoyvotul.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yfuguzfr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zriuczva.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pjchjqgc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lzgkkhvq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dutzjkah.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2araqfdnl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kqplpygw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dhajscka.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uwsakchk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2iqeqqxjh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2weftcydi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gmhbxyxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mozkdnpb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2isiuyvtw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vnmzerrg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cbxwgasp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pkeaycxc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hdigfqbu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2idhvzhwb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2sypeynuc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vinppzku.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ummrltbu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2axsqyynn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2evyrityw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tydapnib.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fgujqjfm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kktjldlk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zbpvrjck.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ytlqkzge.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2wfsxtcor.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qluwdrvk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fwstbjmv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwyocvr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zbkwiajk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myspecmu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hetrqnkq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pzcyhiit.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gpjxrxjn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2btstbcml.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2yieexsae.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ltgfiwwa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zsibfgyb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2uuhqxqdl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vdpztzns.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2raosrbtq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2zvzkbfrt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mqejcqqq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fncuzktx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tytgoiuz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2iqpfpgri.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ktclwyii.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kcrdtqxf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hmspfewr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2coehqiln.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wrijzvci.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2mykdvbkk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2epmmdjfy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2scysdcen.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qxqcmlbm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xynszvol.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bziyxzuk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xeuaelyu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lzdtykds.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gamfzkqq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2jcfpymqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vufvossj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yyfnppkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmzdmzfx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gddiqgqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saspyurt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lpoafadv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdihtos.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vyahqbud.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bjvkwvxh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ubmqxwff.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgzwsobb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xupzrpun.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2svebvoao.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tpxkkmnx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xgtlcfrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vqrwevyg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2igwbejyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hxiprfxf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kuckundd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ejqptwhh.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qgibemff.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mpoqprhe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cjbwrdvz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2szxzwyug.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nnfofcvt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zdhzkrup.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dfavsvav.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zuqrhrns.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2czzswydy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wpghwuvu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dhxomlbj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2uszrkdld.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2eboeefoy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cnqqvehs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qoyjbuuc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uauxcwqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ebdevjri.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cnmzmucy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vvuwmqpa.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cxxfafki.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qqjelvcy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zwhyhlmm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rihpizwp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fnnsgbsa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2svqciteg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2skfzbwok.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2stqocjsi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2uazoxzyz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2icxoxynw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ptuyojjj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jomscgzx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kpobsogd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hbamsnhr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ihskbexi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnltpuw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2tkzwadtm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2utfjvivm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xtdqtipb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ogygdykd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2drgdfgfw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pigykqyo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ojgqqpna.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2yncoeyls.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2jtoksqcv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hdgxyslk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2twobewbu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2yeozqctc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2efumhhux.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yomaiquh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgdblfds.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sxygqgzg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2klaallmb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nepfqubd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hjcrjqqx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hbiifoub.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kfwtmjkr.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vdmciepk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ptexwmva.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mpcsvjzf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2veatbodh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cnbnriab.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2mmbgqbkt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vqvkypyh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rkzcxplh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hmawqonj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nmvwgbwn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sqqkdzqx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nsthyynp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2icgmrgsh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2onqywuem.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnsikgg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxrstnbc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2dnhycixj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dhhowfxs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqoofwhw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mucsabxm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2zosumlfc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nzcqyefh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2dqyjpdfk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2itbvylsl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dhbnpeyb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2knnldqpb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hhwtaydc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgiybrbb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2tafuadvv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fmixgxio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2srzpeysj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2judgdqrk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhryon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bwvijlvu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2voynznpx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxuumno.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fibejksy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hggecyzq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2prgulwor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snbweyjv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tfcrhigm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xhkwcuue.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2icqmmuaa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dvczkeod.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hzlwwufg.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cnimsxmy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bnqulvph.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2obbblyjx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2xeblxauw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ikwoqihz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2tfnbjria.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qzjlasvs.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hsglvxgd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sarvnuob.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bnbdljxq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lgvksklk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2afnnckpw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2nqugldyn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ruzlohzq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2dayzzalo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2rinpidkd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2idaptjwr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qamyacus.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2szvzfucz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vtqrlfmu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2sosjjnth.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwwmsggz.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2jxxebtyh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rvswkjnh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jwvnnjyi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pcbhqkmz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2glmnaavt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jnxeojwd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tinxdpks.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ivrwtygv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2lmrzglbp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ltdxblpt.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ybzbzkco.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2fypbcjzb.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zjombiab.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qctbnzdb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zpawfygs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2vpqsipiz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sflzeyvb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2oajlhyqo.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hibcjqrr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2blnipjov.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cocmmxbw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2owqziqhx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2tuhmzgsd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2nduvnqeb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bivevxne.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ogdjfgkq.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ruaiwoek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrgtxghg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2edtznact.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuwkoxld.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iqnhilmm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2fvotgggm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2esmnidnq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gqmxymkw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bhodocfx.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hvnxqnqh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ptcvxsvw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vpmxppbg.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2fadfmqpl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2rdguaggg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2qbfmsoeq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hzqulsbt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2hlibcpsj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2freabntf.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnoqskx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2jgabeylt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2mafrzfyi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2juavfxtx.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ejfavoer.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2voyfbbnn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2qaoohovs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2fygdntit.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cgervstk.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2okhajdix.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pgehglsz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pryspvkz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2jjqbkrhm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2cyfjqxzw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2dowwgzaw.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ggpsbnhz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nddvismr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fexudups.html


<!-- 参考信息 -->