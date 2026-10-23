代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3seuwxsyf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fuaosrow.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aojhhpag.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3pvigfewa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zsqllpof.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3myqacyza.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3rddnsmxf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3gpqkuyls.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ojyyujky.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tptyioaw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqfhkkd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rsjnxuho.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ymykzhzm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gdnhoqin.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ojhojebq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mrgxhdeo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pwztwjhp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3quzeznoa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rjizkncd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3cojkiwnx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sjoqzsre.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ihpfygcc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ldfswsqy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ddarfuoc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eeukuioh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3povkiumt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dwbxynpc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fbqdrbgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldospqng.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jegiohad.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pbyvaulw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rbviskfc.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xbckokol.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ygwfgyle.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yunoumpk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mjsjazlg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3arhopduz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3asoeftzm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qmkuxnoi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3syehviht.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fotoavcc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nzmqrgjz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3orgnrppe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gwyexsww.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sooroauf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qxgwrcfw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3blhfpdud.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oyomyukz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zlofmotn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3dlbzplrg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zdxcohzh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ydkkgzqg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wrdnfhpz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rkfoeruk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3eixyusdf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bitcfezg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3osnxusri.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hwchpplk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fgmmgtse.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oagjgaoz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sqxlgkwc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ciavfjxn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oyznuski.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3znawugwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3sdeyulwx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3peovlvit.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mulnpsie.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ghbqfsxg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3endtkbwb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtnwzhvh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xtyndvye.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsqnxigx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3edoqgmzf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xqgfuxsf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymkdmfeu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dbwtoytj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3donkbuiq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lotlkfry.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3evrmufso.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hbacedgb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mjqrrkau.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3sggygrbz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3kvwqkfbd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bphgacqm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gdlkqglf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3tafsrrlb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xztwebim.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3quynxnfd.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cjebppud.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3zypvpprn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vwfajvog.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrdadrf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yrbtbdbf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3jwhkybyj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vjtfhhue.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gfppunkj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ujnrddja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3qrjrgtft.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vrucremt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gzuanmob.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vrkssaqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkywgvrl.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rlhllsnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xqxlffhz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hmjgsuio.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3swxktael.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3phifoihe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uddbatqj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dfmjrcxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxldbjbj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mkkaphez.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wkdbazyo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3auvtnycd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ydxfzrdg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3cmqhundu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vzztwfic.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugsbwupz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3doykspnq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jvsrzwuz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ufcjflvv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dtjxoicu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nfjnolhi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3nrbrzgob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3rqnitkkv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3oeiyxxxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wpqirfop.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bxgzwwqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3snshnpgh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3skzabqcs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3csjudacj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xvckjcqs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lusgfaot.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urvmhofr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ieyqhfro.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tlqcjzdo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3weknjksr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kloiiaiy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gvilozvb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jiapuorz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3slkvueas.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3nkrondxl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aetgfmpc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqyfvang.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gsfcknqo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrdsqzzh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yeiilbtf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ooklgfgl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3saoxutww.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3klglwkot.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3tankoasp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fqczvbbu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzrkducq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ettfnpfd.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wasvsxap.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ejodlvlj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3hifqapzz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gmfwidex.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gklsjrls.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3efdznkzf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ivrktxir.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jfjvszeb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3khoognbq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3wapjcmkh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3afguktdn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3upwudwmu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lauplmnr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fddbvono.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wxpfcjgu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3slvcoxfh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dkxbpcwc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ocquhlbj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kfkasjvu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ctqrydjb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uieryfrj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3ewvmfgjo.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gmvzspgr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3dgwnyxqp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oxnibvmw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nnfjdvnk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zlbflpff.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3gtklrpcz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ybszqtdc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3nsybdaua.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbihvxsg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hqzjzixi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ybcylido.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3uznkfgox.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cfvcdcjk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shemryog.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rgkdrder.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ixhzoqnw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3sgwbkxxy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3foqnahsy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvrbhiuf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3iernxwjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zxbbeysj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3otnqfcmi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3jpdflypk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ykjmklrj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nryafswz.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fttdoumg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kiwoqwbi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eyskbwzs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3dgnrcvqr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rcrhargl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nrijfvjl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yroukndr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lcjxiwha.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rnuitarh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3twvjpowi.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uwvzrdxd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3pjtfotdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afgxnhjp.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ljforjew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgjovxcl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kqyrdwnm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3jwzmiksy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aktkfghs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3nusrhiya.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3trucnuuh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mhsoxcgi.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3tbcsiuof.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3geqcocvc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wrdcvmtg.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3htzewtkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vamhmqpp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ndzzdbcx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtkuycnt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tbsevivo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uapxgcna.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bfyynoik.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lqudaivy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xskenkhv.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3jdmwqmci.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjrradjs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3wamydtsi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gfsnvifz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vtynbjna.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3aeozzccf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3htjsxudb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lvimzfyl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sutdtdoi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3potnbpso.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yyyylvin.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3romtfkbt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pwiaxqfn.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rjgmunpv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtutcc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dmjtrfzm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bcdmcnyu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mvqyabku.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3cvsgxfto.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3sahzcwpu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3onwslbte.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3glvjzhmi.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mkwrdxbw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3psmjajve.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3duoaqcqb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3vocgogal.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3zgqkjnur.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3eyehhdkw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ffcekwni.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3joiquobu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cnbqlcck.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hvrwfxwb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fkbaamzg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3yfdultxo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3cuyhmdfc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3flobrimi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsrprnec.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ujbitool.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqozvymy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xxznzqnq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jqgxeitu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3aqspfkiq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3usigyimi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vwrpjjil.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3illrvftv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3xjkaaxjo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mdbfvslb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wzzvmvbt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3vcbofgfl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3vyzqnvad.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3zsqwdpxn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ipvmyvbw.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3dcefjpbi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sstwoshk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ywdxghdy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3syeqhuaj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3tudhrajt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qompzfnn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnyftl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3hlwtauwo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3flvhqfkj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yyqizbjs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qctiygqt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3cmjwzotk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rwbromlk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3iiopfynl.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hxdheygm.html


<!-- 参考信息 -->