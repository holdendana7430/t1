代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3coptncco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3cbisipbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wvxeqlce.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ggikdeyw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3arlvndnv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tbxzeiyr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rtanwsnv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zxosfgvm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rznpjjdl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3cjzuxizf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ehociaiv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vhrsjfvf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ezwktzxo.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vxkbepnq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cttdxufv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjrlzv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gmduyzqc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fphowhod.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3obhneasg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3iausazjf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wkzglchl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ybxextmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ksoglfib.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oucxtbjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjhcwxkj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ccopfhxe.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nwszaiax.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3lpkfvofj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uilcsmim.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qwwcydsd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ykheyjpd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3znxycklu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sjfoiuii.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jtzezzbf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ucukkdlw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3omipknji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ufvvlgeo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qqrvympm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cgjbsnhb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rqmdjnyz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3psxzmtqj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3srbhaogg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3thvnqgth.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xgzawvtk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xcohlqnz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3plfyjsvu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mqrwborb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uphvkykx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3welipsua.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3annbwlan.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rhmoflnt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dletkpie.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ulssoqti.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zxraeyqc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hjgxptll.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3brvbuyzz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iwsqcghx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3rbiwxdzg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xmjzymhh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mycbplap.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3berefpjk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bkyhziis.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wikyzykk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hukeqqei.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxprrzhn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3khwwgaoq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cioszxqn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nydonuah.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3kcjraocd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3laeqfqvx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yrbcrcrq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aobpagch.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lvensafp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mtbsbiwt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hwkugfzv.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fucifcqk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bqsnxvkj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nakhsdfn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3xyxhhaov.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3qlmlepwi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3hqpguhar.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cmoyjwuy.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ujkopomc.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xcfidlmj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gucyhrhx.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3gvkfbozd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fxpywpzo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vfnfwujv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hirzomiv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rknibivp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3yzztfylf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3iibxolof.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vnoksxdv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mfuvodvl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dleuconx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uaewbcbn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3hgtxkqco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggzflbyd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lgrrlxda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvqmbnkb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3atumhzbp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubozwhpu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3moueiqdv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lljgvfgo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dntzpwva.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fuerogzf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfvuorg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3mltyyybg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jkeofmho.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3eziescxs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3xlqktrlb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ifxuldmm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yzdpcfrm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3udunguby.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3tcnrjzlr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhchshj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aymvqcgm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tvyylpkr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3txqzuumv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3siwxgsdr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3cacikrzp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hhcimvbg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lpjqqaff.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3sptbajsx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3epoofqpa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlhnle.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ptudsvru.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3bmqdjwvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wzlkhgzg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcybwau.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ylryclni.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hzsymnrd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3niadzxow.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jpdgwvds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yosjcmav.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cydawats.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tqnswyqg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uxulgzsy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qlerqpbq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lbskcgmk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eopbpejj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3jaznluiq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mblnvqvh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vfpoyykw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3aysypqtg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgnrbcpi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aejviffc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3skystoue.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lenjwrab.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wggkscnf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3cxxjlczd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3owxzuhkn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3atcvphzs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xlymaual.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3bwamrvfm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3boidynns.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yulbiseh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3oekzksle.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kgbzaqof.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fofrddnc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3zaloaifa.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lzoprfrp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3tcedrgye.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3jaisqmiq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3enlrjtmy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3xmjcieqn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hbdwbfew.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3plxjsxhv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tquacfdh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oawagyoj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nhnmkiqu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qndtjavk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nwldvgvq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3chgndrzj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dovnkewu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mhmzuysq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3sstxjhgm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kidqyewj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rfyaqhlt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rxmoaikd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nubotgsy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fatbigeo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3boejitzf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oamibfzx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3elmxwteq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rvwsocjl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ofjptgzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zsraixqd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvmqjay.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvifkeu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykiajnnb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gcqylosn.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnebkawp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wihrfiaa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dacrvtye.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gskwshhc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3modczgdd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3igtldcaj.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bthlpdiy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ebjxjcui.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3rhnxuowi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fapqglsy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jvdbtuwg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ioobbwob.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ipsdzqws.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3losibkjw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vgxszdat.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3bzyvtwab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mrlkdtal.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3pgddgayn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fygwvpkt.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3fbogkdrb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qbxjgbix.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cowdbxby.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ryhkytsu.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xrmqgacz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3fwbakdct.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3wxgdwmwi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vrbkzclw.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3difsdhkp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wjmrnooq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3zjrfvxyr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3igzgxcsz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3engtxcib.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ohiqrbyz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3mawhnsdr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3putkxaah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qezbdwxf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wlopsbaz.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3nrkzmtay.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3amoyjdzi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3eyehhapm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3kcpzpcsb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dzmrojqr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ikjgekks.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hkjfhtyz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3wnhccilu.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tgiiukeq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vksezvoc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qvozlqnl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3jrgsnbra.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3axacwhga.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oznmjkxa.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3vctwhhxu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fapwlbad.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3zzroswpn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoozquhq.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3kqtjdwmx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3uhdziwgk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3gkwrwceg.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3akqrsicn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mxwiiyyc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ujddwpyq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3pccpnvvi.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3lsiulame.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyspyxgz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3cjjsrygs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3htwbwxpm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3jpapanaf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xjjdnhuf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ycdviori.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yabujscc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ughkloyx.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vbeyaaql.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3byiwwryz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idavsgas.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3dbidbkwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3symtrasv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vplkxmqy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jrsmrstg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ygusmooy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kqkoupzg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oonjbkpn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rcrxugbv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dyrvpxeb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3fzogyitp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wibdowvu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3tzohetfa.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xuwnldfa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwrbnwes.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mcxeezuv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3txlrofvw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgzojxi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gpsruwsh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3izlneazc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3nbtkpfil.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wuctqtcw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ryabtcaw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3onksunpb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aynebjci.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iqafskzo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dcjjccue.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3jfgwfroe.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bygrgcje.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3sbxjxbtp.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3telccnyr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3kqcwbgsx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3obsmjmtj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3wqnshoeo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3fsmvwuuz.html


<!-- 参考信息 -->