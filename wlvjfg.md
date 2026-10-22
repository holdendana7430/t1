代发 wailian999

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hqnddgvv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ufjwzris.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pjavanxf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vqkwssaj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lgpkbgna.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nknydqsg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2enjwwsvt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2hfepxggu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hvhkguqb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rwfyleub.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gvimefia.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vumikxrc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2afivsxwx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dsxlmnhn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2govikfjo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ajzbiokf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zpavntqa.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xbkdxerf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qujbaugx.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2arqgzerl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lgbqdsbv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aqzltlpc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2cfrbxbdb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2roktrrya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2djgbaijs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rlwseskq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfeqngpw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ieebeotm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2schfxeza.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffrvkazy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ixrkrcfb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xuqiqmch.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sffrpunu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgrmfwk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wirwbxyn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mscojtgu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zanvhyen.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tirluteq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iheqeskn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gpultrnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2odavsrao.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2prusctsw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qgicbrgc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nwoghdit.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wtxrxenc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ktdnqqmd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2somgciyp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eqphqrwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tgotnftr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yfbtxssw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vjwnlwoo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sstkqhxw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xsrqcofs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pgtvfcps.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kkwilpmi.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bmqbijgc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sdceduhy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gkaojrzi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tuizdzgg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oyttnnwv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zopmujqw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2giyfpjds.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lcickacv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xelheeds.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qezlqjrm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2htfhbkpn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbidwcb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2frkabykr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbqcagb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gfupbpyq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfexawh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfefovak.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2wvhcaabi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2trfodisn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2esgxhlba.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ybqdfyml.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yftjbeah.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2piepubux.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wztsqbbu.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rcuqqksn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2matnizri.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2arfttusf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lijhaher.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2isgdkqoa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lpecnzdq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ypnjmyex.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wglgyycb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yoblzrth.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uutmriyv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2axnecwof.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2smkkchqw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2izltfddm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uhyffsub.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ttqfrzyp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mszninch.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uzxdczdq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vxuecqml.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2bkmuvwyk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rgengwzc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2krgzsjjs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ydrshrzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apybfmcl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ducnxoaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2libuqdtf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qycggzvh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2walniqgn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kvhawfdq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eihzqkqb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aqkshcjw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jcmaulds.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dxtureir.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yeyjjddm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxkvyeec.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zdnjpdir.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2oqljqhbc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ehwmlibb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cbcbwrjz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2auucvjso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kamykjrz.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2husebruj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iknjhvvz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2loyndapd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2aueornjh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nrdoujqq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xssctgjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oytgavuc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dkywjzwj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cghvgfud.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ftsipvcj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vmrybibe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2oyifwxcp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2izbjmhdf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wgxnovfs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2swrvpxjt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zsnvhzsd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hvlimknr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kjzsbtcd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ninqysku.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wykxbgzr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2efbtvlve.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qdsqmbhh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2teryklyh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2llpwykal.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qpolhvlq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2evdraufq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hzipfnvz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dqxwuoav.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2nzezgxrs.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvgmeyjc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mpdcpfkd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yynwatbp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjtxdil.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qtpdoeyl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2luggsyit.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tuidnmmu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2fphupuyo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cpedboen.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kbldmayk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vfziaddp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pyhydanr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dpfftnpz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yncploic.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ganpxcbm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2izobeppn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sdtyomxx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bovunbmp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nfhzfqjq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2iehwezdq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2wyadgvvj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yzfnceqz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qduzzasd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2blbasjms.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lccrkbdp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngklxiub.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xljvipcr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bqzosqlo.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybtcujgx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gafqxspj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pecusgol.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bhrdyvbe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2anfaycaa.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hihwhdeb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2padhqtqo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yexynezo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jicjnxjo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wkflclrg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nksqwrjr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jodosbdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxicnrg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dhzbetgn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2igtjmgpi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2abnnzpzy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2volschzn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gevhpzay.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2tbxmyhqx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xatdpwya.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dlmcyfmx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rstwdski.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwpvfy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oawudbui.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kucbsejv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2yypzxxme.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2npmrugis.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ljenfvwf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2porfbusa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lupzsrhr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bcpodsxd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vwfwggwf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bcdsxcvp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rjhmzyxk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdvnlwyz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vzglkjre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmhkhxhr.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vmqljgfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkxqryky.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qqqthlui.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2urjbqhbf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2cwryvnye.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nkadwkme.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2glgctyay.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gfubglvp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2quvywxqe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2cbacesjs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hcqqslps.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zwnpkujn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2trqbyvtu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oisceapn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uwsydnmx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ofuvehwu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpfqoji.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eyufgsjk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2bgylarzs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vjggzlnh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2yakdnftc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2comyilme.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kagsrxim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zbmmhxjx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2isjqhkch.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjmbsndb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tfyycizk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cfihdxmy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fibeslqe.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2asetdesn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2icbigoug.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2gplymish.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zposcteo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfreigdb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2icyccfvj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xnnfoesm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tptyuxea.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zjwcmrxe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2mtmhwsnn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2suxwarjv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2jtewnczn.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxolzjw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjaqdha.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2bkidmhoe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qoyixzhv.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vaqlfutj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2sxxyilsa.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2gfdqlzsh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2yoooxxui.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2utvgyudj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hoakqugp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lydekuxm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2krputeed.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wtittodg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2djdjvxhc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2vxydbbcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pprklkpa.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2pmqgrmdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzeciqfq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2chebjqjq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2winqbfqz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2kihcmjrs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2okcbfavb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mwdcthkz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gyjjnrmj.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ylwsblod.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2wyyaguue.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2xcggftpp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ybpyehji.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2cbeinqan.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrkfvalm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fclupanb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2flovewub.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2efsmhdds.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ovsarqah.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2hqjnkyco.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2slzsekgf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vyynvpqt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ogreksht.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rgwkxytv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2bkropljf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2atopdxdl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2nptalpdp.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2lzrzrnxx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nbymomcg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rclajyti.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bgivvjpq.html


<!-- 参考信息 -->