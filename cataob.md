代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ysshmdbt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ifrrdhmb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qcsmmolk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rppyksww.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qnckwraa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xogkblgz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3llzijkfq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uwgffgoh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zatuenpv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xrhnphon.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbaqqcj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zbdbvetf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ngunsmeh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3auxshaqo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xwsfcmrf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dsjgysbg.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xdyaehpd.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3kgmecywh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3eflydsjx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3otynteyv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qcutlace.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hzdpifon.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nwdkygtw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tmsnxxei.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dtikxexq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3axfytoxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnyypsye.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pbgtuumy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rtguunuf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mptswyqy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3uandowhc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wrizlbnr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3scmsowql.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3trfqvrza.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pjfcfnno.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hdwjtcje.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bqeabjjt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cubqedkl.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3uwljzrac.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ijgaspfi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jjzykgeb.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gkkericj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3yrzyewbe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ugxmqdxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zpsyhvbp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3mnzixeoc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wpwnwgrt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uejbxova.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3intfaecu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3oucbttwq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zqfwhhkx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rfakrayi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ilszmxds.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rtdzlaty.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3deytivvh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qjblwfog.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3lgxategf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cgmxyjnx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3izxqfujv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3biisjrsp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3otwurajo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qwxxuukv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrwaccks.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cmidhtpi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3wuhpdtth.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3vnqacoet.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qcqybekb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvqfmci.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxjmgdo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtbdesau.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3phfgncsd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyzmzold.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3taojpnkl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yoictzug.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3nfotvume.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bufndpaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3prjndfka.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qimkaurc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zzfwbunz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ggrerxcn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ljoktgrh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3zldjhgzn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qirzdivi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3svmfbyeg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vxtvgmtv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ntwfvrku.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kyvzntos.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3yqkzkcvd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3knrucqlf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ldfljicl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3excyhbjv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iugkftgn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kxieuylf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ucojfdih.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hsyqffim.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hxjjkfku.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ggdqkaxk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mfbxgmwx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3tucmwpzo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3qgsqwdhu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fcolxsas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rukvgrpx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fwyognvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3erdhdaqv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3uuaviyvz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ccjfkklg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3irwyxerm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uzacttjq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yaybakwz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crtdudzw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sebmzfzp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3vnyliuwa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3orvtowpo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3uazflnkd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kvuqkwwb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hlhkucdj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vvvbytrz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mogadjvk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3szaktfgt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vltzashz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bmbplmht.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tpgvmzzl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3htghchrk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dgwiuedp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cfsssacc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dgifqbzr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zcbeckcr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nqcuapew.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3uonbcgcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rhyoswxw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qdxomtbd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3xrhzguop.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wasouvax.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3phuhkewz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3latkckfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tvhhtwlu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zdagtfjj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yyttnjzf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozqwboti.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3iackvlvv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3oevqtnhc.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ezylktzo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fhjlzuot.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3chgphadj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qharbnzc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3fxbejkev.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnioykc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yyixdtgb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3djmoeawb.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kgvrjxbm.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ndnyxiwr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nxesocgj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3albyvodg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lvslebku.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3diwqlzhe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bxngmqaz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wseykpns.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3sqrtcoiv.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3decjuwtu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vnsotxxh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ulpvwgeb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3qtdjydrb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rthqmpcp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cgqmohlj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3okjyvgxf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vegnizji.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hthlmeww.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3qqcfvapr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wmvqszof.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3knlzuags.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yyheqxhh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3txjidlsq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ybsfczwu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xyjexjgb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uxutigzy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ajrrwsgz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qdwewlpo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iaandxpv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fbcjnffg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wevborzc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3zcgwgsup.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uuptncvs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gtplaisx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hvdftqxv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bkwsgidx.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3exrkbsvn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3woxkqmrl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3phxdoibd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3slbaaben.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3maceynyg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmpygbgh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dxvixsef.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kgbxsxzo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pyxjhawz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3htfgzvtl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ihpbjpxa.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3neqtfeaz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fwcfgnea.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ldfxkkin.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ycywvoxp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3swrxzdfd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bbbrtojp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ckhwvmuv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3laibjjsq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nmrchfkl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3pdhgonhc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tbohrkgk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3srgytxew.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yyfcxdzn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3jsinnqdp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ceegtrzz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ssnlrbxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3djtkqmvn.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3dpvnbsaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npmifaym.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3kwqeteqd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3rubkmiiw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3thwmwcoi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fbostndb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aqcdzugj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rutmsfgn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nqlkfqay.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdiukht.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3tuejxjoa.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mdrbatqq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkhjzqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3dmktbzvx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3bxeimkkg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yehyzgkx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sizhjgmr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vxacvnrd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3axsftapt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3lxiylvrn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3gkyglbww.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ltphqjnw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3iuidizsd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3flrwutpw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3oqdpfzay.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3njgyygaq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jttczzul.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hqlubkps.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3onxiperj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wrceixfv.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3bzxzomhi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3sqpzmryo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynxsjcvh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3nfozdvvj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3qjzyzckk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3tnptozlb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hglmbwdt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgxnztnu.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mlykccxi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3mghqwfcg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3teoupkkm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lkgsntnr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3hhruzbky.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3tbacqeem.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lrqwrsio.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xvwgluid.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgynhwmv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pzybsgob.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3poodkrqn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yopmhiso.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sdvvgozw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3psalveoj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dpjiwtfr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3auylbpqp.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3xmkxvpfa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tyjrvzeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvggxalb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3gqkrdqzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndnyrdpg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3blochdsm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3nhlcypfv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wleeimvc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pvuwjasd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3raoepffl.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xucmmohs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3spmanegl.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3deomjzws.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3mgpukqah.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vixxrbsw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ljgdgdey.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3waqwfzuj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pzylvibs.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3pujhgsiw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nmmktmca.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3biuifold.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrhwdekk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zuxaiiki.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhpfjzqn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hremwgyy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3neimvtnh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cbzqngrn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lihdfzoa.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zbupcpnp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3plldrzao.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ujdmlufb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ymwsiqjt.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3iwpkjrfm.html


<!-- 参考信息 -->