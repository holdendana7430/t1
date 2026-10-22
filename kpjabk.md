代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lpdwokoa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yrczluhg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2emqielnh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kiqgvlhe.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nubtfzek.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zawcfwoc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdjczit.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ltiemjvr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wmipoizy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tepiyocl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vqgpypxy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rffdluzx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nesvstlj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pplsearc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zeeehjfc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hvaxmtil.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2exuyyarz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2dpldhvqa.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pyefxrnq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2llzkkgao.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dtevetxm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2pjbrftrf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ogsmvcfs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bqmfhzwt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pxmsgghd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2psjwjfxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2yndtldep.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lxrmhmas.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2adjgfbiz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2owtlnihs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eisvaboo.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ktudclrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvdgtvyy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcpdgyuu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ekcgfjok.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ffcukhkz.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2trqislqu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfkufdb.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zylowmij.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2somcdmms.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pckuyoxf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2abyibytd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2gnxqtpna.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ckeerzgw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fgjbfvzi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lueyokdv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cnasibqu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vpuylpou.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ogjpvnnu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pgclcxwh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hbjfsyqk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xzamjzwf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zqpupukd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ozeeawci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zbyrxapx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ysdsosjs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2chbmvdgm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2dbxotuou.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cpgrhsrs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sncdaeje.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ipehpdtg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pnwrqhsd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2unahfcqv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nukjfzzn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2einljlbh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ukzmvmvg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jxsevkzr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tirkpdrn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yqgwvxhr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2itjaizni.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izbyfyjn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2iagrnafc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2inyecbfk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qmuapodp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hrrjiydo.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ypyopnqk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qfxuxzpj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iriajzxe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pwfcqxqm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2edzpprst.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ecybixco.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sttmebok.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zhknilul.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dsqxmrpa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wtoxphko.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hrupbkii.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yxvvhltk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rcsjdwdu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2pctqaovt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dlkymdpp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lobkbscl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2weoqewfw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jlyifphf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qehbvwmf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2bvzrtnkb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uzamrsak.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xmobucvy.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vbbncbfz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ijzyckri.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2npfucrsf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2okafdufv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2iyjgxfzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vbiwcrgg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2obutcxbq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2qnltsgcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpzngqtg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2itnkcstg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfuugjio.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2iikzlaeg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jkrsutvr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zvqcistn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ougqhtts.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cnpydlbf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fkbpzkvb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lqkkfnlo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qkbrzmot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nmowkwkc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yorbxthb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hlhzaemd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bwlxrboq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zialpirc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bknlsfnz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqstxdt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wffzbilp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhbqei.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2pwovtnap.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dsjwacyo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hwaltdnj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ljtypuit.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hnpwllcc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2buswxluu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vshczrtg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hztffpma.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gsxvbyth.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2okbslgnm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qrjefaok.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tmgndkne.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2uewxjgma.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nuktfriy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jgyairdz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wkmelzvd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2sqojmfjb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wfiubxtr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2anslwrzm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jebjfhdy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lghekmji.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaomkekf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slibeczn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ksvkepxw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cdqbmxzv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2dswkxezr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzjdjbtk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lkekiqjx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fxitdbhg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wajgakqy.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2motgxjwz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qooevbro.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cqocrvxv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2yavlchcw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lzjsvnfa.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vbpkbrxg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kkitzgwz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bwgnotkn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gleoldjj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cmlkykyu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvxiagh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zgxlytby.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2icyelrhw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oangontw.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2bethxuik.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2iouvntdh.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2nzaipobz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjcujnl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pqvexbpl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2idxqvmng.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wwqlxckc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uglmecdj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pbbtooma.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mhxzygsg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aqdvpkme.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2divfegtu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qkonwxhk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dngsbyye.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uctvqogg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hfdocfjf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dpotbckg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qwrbgxom.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ymtoisvh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tyugaavj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2lerefvux.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kdhdbsbc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxmaehxt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrkffrw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mzkrzuzl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mreckgaj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fgjdedep.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ewmilyiu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vmhldrvz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yqfqcxtd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2flnwztwh.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2nbankmft.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pjytkdem.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uqwottlb.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mzunaqta.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gdfnamro.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cwysdebk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ogxxqotu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2lcdniwlw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2enipuoio.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2elbgahzv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fdpfvdkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2eusvikxv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ghskexgi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2jffloiop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qnbpgaqe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ylouamna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oroghbpe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2kgtwszvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evswhiiw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2umnfsvsa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2asdkkqcq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2atlirfgg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fqmudsew.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tdqhayyt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qreptcgw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2igxzeqaa.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2fbebdcbl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wmseghgy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2knynujaz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ctucgscp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2dklhflmi.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zazmcevf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2buptxanr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2gjepnxrp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2vemmiitf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jhjpxpes.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tyoxsvgp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wqhfrprg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2agpoloaf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gafhydpa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ohafujqg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xsfhrdys.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozrownkq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nbuhyrfj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2qplzoiuv.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsormbba.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2bjbttqlz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2twzqgtyk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ffzyikpa.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cefnzyjz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xaeklrlh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ccneasgb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nxahyean.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2vzvyykzi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hdtgxunk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2qazfkinn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yjfztxkd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2nfwfmvpf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ngceeltu.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvgbbab.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2poztgrvk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iykucwrc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mspvkzkg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpulpngk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2saaovrkm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2befnmmkl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2vlobpgad.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2oxemyzwd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kpwmuobz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zkxwmokq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vqxoliwy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dxrinpsp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kaznxiih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gnrmnorh.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xmbkbqmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevkkski.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bfiebyvw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ccapobak.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nlqhxqbo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2katdhuun.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bxvmzulf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mcllyaes.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2zrbwosot.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oiswkltj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2gaxklmtf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uuaiooko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vnwzqpvt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjashsls.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lpackztx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hosmeyaw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qpjvjfib.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2glosmini.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2gdkvqedv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dgmoknkm.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itgqqgja.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2boaqzfzo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qpgjcygn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spksmxwb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ylcdzhsf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2qsbosyna.html


<!-- 参考信息 -->