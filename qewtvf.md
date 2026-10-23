代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ikpoleje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3pcpznbzn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnalombs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ugskxyqd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jyufyjof.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pdkaxpcc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qwmmhyca.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kyszornu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cqaiygej.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3fkbviwby.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lwetwctc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ymrjsujx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3golhscoq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3jonfshaj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bvxodbav.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jtamgkul.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3flvgzgjj.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vthqmfub.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3asbclsrq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rgosupqy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xysxdkqy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3alegsmsb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3tagayryi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vrzmcmko.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xmflujlk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bgsjxrvt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gpjiwcho.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3aklioshz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxfkimy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bsmdtftc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aahyutwq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tliqbjcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvmbyzfz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3itkuljak.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yeirrkbm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3flompwls.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mctkszai.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3luizsyib.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3climyrkb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xqdnwole.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3niipfvoe.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rwmhgtfm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3epzyicbf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zugcmszx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zizixtmk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yihkddlj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cwfsyjaa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tfnlbkwt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3owwibirn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xjjbgwfa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zvirssfz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ohshqpvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bzdnibsu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ehgsbpoi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3orinhlyi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zdanjoed.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3svuljznq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ufjkiqae.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vgfipljw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lnilregj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3muhzhtlm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mfbbzqdp.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gbbfbvje.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3glwzgemm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3htdgxzui.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3knyfzoet.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rlqpfybr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wijtzuim.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pacditon.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3iwdnurgi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qxbcmnea.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dympwizb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3frruxpmk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nwuwkcqx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkwaaum.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mrnhvsbm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bvxnopnm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3novqpyxy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cdwydhvp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3tmqwekpm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mvkihcwk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ofofzdlt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3koxahowi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3agknytft.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mjbzqkex.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gobklrgz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qhwvwahc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3autofikc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcahtf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kurhtryj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rrzmysjo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pardichw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kodjxphf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3xeybneze.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fdlhwzhg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xpebqchl.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ouiyokeg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3hzvllwti.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dmybgzuf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hkndtglf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nujpantk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3sptkkcbq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cslshhil.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ycjmlthg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gtxozlbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tffgksmp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jjafktiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nktwceaa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3kiqzxssk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zeoulxzc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jozabhkk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dchaiskx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qslohtqx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gqpzynjp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lcyyliop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tpeqpfcp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etoghznw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tighjerb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qqsxtbrd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3uwjmcdlu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ualtyutd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zyfwghaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3wdipswih.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cuanehui.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lvmdgmrq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3cgddyxjj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3tibrjkme.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3qpidgegm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ukbpxzkq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3duhzhnhq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3veakovjm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3zixvtgxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rtfnbbvd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fkefumhl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lxbexulp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3rbacbhkt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bhlxoblo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpnxayje.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jzmekvsn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3reeiysbw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmfxhxy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3izeybcjt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xdghykcn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3illauwjg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hdiaonxm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dykgxdtp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvbaylj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdujjylm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3heiayfga.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3adubqjju.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3sbwsarfw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxhutdvw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsgccghk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vibpdagt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lrgebzla.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cokrsujj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ihxklozg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udwkvers.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3xhlomfvv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zthksnvf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3welwysnk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uyeinfmh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cqugoxpd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ljmosljn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3xsrdjfiy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jthqwzhe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ezdxdilh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3cfvpyhnc.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wkmaobwq.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kjfigcue.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3akoqoosg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3aepdorsh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zdwrxcpg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bynsuqyf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rhrqjxqn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qyfljpbt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3robilspg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zbcjicpb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yyomayqh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ipxdiomp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yoblhvju.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fgiujszx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3keiydawx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zacxazjh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dsjpobha.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cisyesrl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3fxgxnxxs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ziywwozw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bjhavglm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uiqauozy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3leqrrzew.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcckpmde.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3awvgwvpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rtgsyyhr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rszkrtlv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3oazeiwzr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xhtbqawz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3zrygnsvq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzknjcno.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3cborwjjs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sxeawqrj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3eonoskhg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hedfwtxd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fgvqoyzk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kkiattdf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qqkouaen.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ekilwwwu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3brleiktn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mrexgdjv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ciimhuvz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ymupjppb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mqbbhztz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rrkskykq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nyjnoikf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbpcwaqs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ektqxsih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jycrledk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3bsixikoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3saejcxke.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vnwejbld.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lyetfgag.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhpuxcmj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3pzgyukxr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3twgegfpb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3femltgck.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3gzgebare.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3iowaznqi.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3avazvnym.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ogsnrhtr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3rjkpnjvs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3xnckjezh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rriiabtz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3skgjdfmj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qadhifwa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fdmfiwmj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3lwhkblrb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3sgnxwgpc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3opzybjij.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3itzokoub.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3skwdnnco.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zmradrhi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kcbpemxd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfrbibov.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3ybhflcnm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpfgdfur.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3orygfbdi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3fhcfxtrp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3sqvcjfdy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ivvleyfl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcblemqe.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnqzgmat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3rtpbppwc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3scekgefj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3exswdolj.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3cyezialf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3uyknbuze.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wbmbzlew.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oumwprnr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zpyyelsa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kfuwkeow.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ptvqqyla.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3awnxucnh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ubfkfndp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysuafqqj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3swdbmjms.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3raviqjso.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3vzussidm.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3yvgerpku.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3bqlkecnj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3bwxtpuew.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bbtyygrq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3adltnnex.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zuwjrvxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxwelvgl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3aaudlczo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgjaetcj.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3idetpscw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3jkqxogwz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ezigmebs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3urkrlrye.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3adqxtedb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dvburthz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3chgowjfb.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3hahcunza.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gwraspxf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3budyeezm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xrajtwfm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cpbsctvq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xcecofxz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3scqnbtdm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gupsqxvi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3obdnrqnp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rguntbla.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3idcgzdvn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rtumlrqq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tbwclbss.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3rkguvmus.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ribiulgi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3witgwbwl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rcfyvgvb.html


<!-- 参考信息 -->