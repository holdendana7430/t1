代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qhfnxydh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3slchpvei.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wjamemsa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jymqqfjl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3upmfibpv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3txugcmip.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ghxfgxab.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uyjflwyw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oajlfbai.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vlqoeqps.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jwrawaqh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3bjtmchaz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lkhogcrv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3trmukpgt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uvxxmhtm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xewytpbw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fkvpfbbj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cytdkiqm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tbfkzgng.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jjkvwivk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ibupoamk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ycungnmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wodaamaz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jzfebnuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojtzvrlp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jfkvlbif.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oehifkss.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jrtycgvi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3puhyaqmd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mbpggelq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sdlrljkp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xmibsolh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3etriiddu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3umjesrbo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygxjffcq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tjhuopmq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zfbyajhz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ifpfnjau.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uwxqnoee.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iyxfxxvq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3gfmixhhr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ekxvbviy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gcckwyta.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nowqrhmg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3buormzao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cppkaeqw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rtnnnusc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rtneuanf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3yajmsmyk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3gifmefbm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3mrouyuuo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fhmymubm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xdbvksbp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfovqa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3txrtqipz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fyiizvoo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nzorbcsj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ifewcbxb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojwdcwvz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ekbuooph.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hksiwyvh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3tpyvqhjy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uxdgmxjh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uzoihsea.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmxzojqc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqnnfyvy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uebvfreg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vezcxjaf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mttpweqc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xbohsfck.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3llsxpxwp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3atatuwtq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pdhxqcpk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ukxzretp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3otuluglq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jiubbxbr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nulkhnjr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qvagnxwm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vmxshbvo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ondcdbpo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ofdpauru.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qxcitgse.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ngfthxka.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3yqxvguvz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3otrnewcd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ejduwwkg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cexbfdlm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iyjppihx.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jlvdtkie.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3fzudifvh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3buszrgqz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3expqymhl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3btgbugot.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gjrzcrcw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sdrkpmhn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vsgevfvi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dqaxaygv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hgieyrch.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wfzjxvvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vzsnatsa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lifscpne.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ziqjoqoo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dnpitbtw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iqbvxfnv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mwenfyig.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3csoiyxjm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nhavsmgu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3axgtgynj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hfyxobmn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dnzhktcz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3foywpucm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3wuvhczgf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yvkhyoah.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rdsgsrjl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zlidvawk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lfikbpep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3anzvbmdi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rufqukbj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bsqozsmq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3eyjfzpnw.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3whhotueo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3eclgsack.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lwvavaom.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gvittlan.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3wlxkdmpe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nucyhxts.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oovmbhss.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oahfbdfn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lwemnncm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gawifokw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dxoflxjq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rhhgajtn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3oewvhjgf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rszjfkus.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzwwrdw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dhznxocr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tvwujurm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yverfzyn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3bqudmsaf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykovlyih.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvgltoyq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ubzkjqpn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vrfkdtpq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3zhjlxwis.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zxnkkznr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nqmkemxh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3btgtinqi.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tcgvftmm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vbouapiq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ffijcywb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3davxgaly.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xsjhhewb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ccoucwch.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cmwtwqny.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ktnhkiqv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3aiinfykh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3cavhjssx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3asrjoomt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3aixkvcbu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rpllrvyh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hssgybgw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3tnljdvvl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3aqyhpawj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3znlibuuw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3waenubnx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3trgfpnhn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3utkhyeyt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jercousz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fpaexhag.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3opvknkrd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3hmnxiddh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dykkadjr.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3lihhxses.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hrabmqvx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmzuxxun.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bdtjohzp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3fbignaka.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ziheysxc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3bfvswzod.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oyrsyybn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3elxnpmnm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3eqrkmabx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vhhargwr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3benfgsdq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyzxavhb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhawqvf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jdbgkqqa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ybhlweix.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gkmfcdvr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dapteswk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tlqmikoz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3aypcxdvv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ybkomvlf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdhrqd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3psqlwcap.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ddfulqvj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ehfasmsp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dqqbqkef.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbvkscgc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3esmltswd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xfypenoe.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ywituckf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eikryenr.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mqhbmrzm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ribckcab.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3nanbsmvf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nuvmebst.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3milhnxot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksemxgjw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3etibadrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpzqvmkm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3cmmwrqaa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3imjbggsr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3owjbtosa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ngbhyyvl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oqsfhapy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3yaipqqej.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vgxdslan.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lcedvuji.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3goeenkzw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3iolmwoam.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3donrsbkz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3jxiurjvh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cqtzjgba.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3lkfybldi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3jaqxratm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3iwaknvxc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3hlaiwevj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3fdmndoyc.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3odujrpeb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hzuolpgz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gwkocckh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3gskdpada.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gypglonq.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3flilkavm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3pieacegi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mpsxytni.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnebgmgy.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3imymqdzr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3bbwhnsup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3yejdlpny.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgmffxjc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xpmaysuf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3joiiksyn.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rnhmtmyj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bcrrygfx.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3klpkfesr.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hogqrdjm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfczqpw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3tqspyqan.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rmgihbxg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3copjnfjq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3folsacjz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wcyijtab.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmktokc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3txatwcxi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3rguvcjrp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kquzeeoa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3bpnfbzmz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ehhvtbak.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3aqtsfinu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3azvxtynw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3kxqogcxy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3fiefumvu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pdvmxqcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jdhmtkot.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3nywarhtd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzhwuudv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xmskuama.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dtfbxifl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jpduapch.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zubzzigs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wrslfeum.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3kwrdsojf.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3faogunet.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gwmyufki.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3rbobiapw.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3solxrfeh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3svhazypy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3pjdthxqg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mlmrmxdh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3bwxiqnep.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ebdyoujx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3wumgsuqp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzivhrum.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3dpeyoifb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zzeexopp.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3gkizqoca.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nitaunxn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmtlnde.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfwxfkow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vabnital.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3esryncgu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xaxlbfzi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3bfpqfjph.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3qodesvop.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3sgzmcjik.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nopfgukk.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3ypusmlix.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3hgroddcx.html


<!-- 参考信息 -->