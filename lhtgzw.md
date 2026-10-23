代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3agqikqxm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3umkiomqp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vmberoqy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zduqbspb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rxvzgeve.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oulxoxrj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mrapqbhx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wfpimbjt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pvmrsirl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3brmduojo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jgddyzwv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cpsbhzjf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vavgcxqo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uwbscdgn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pealnclq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3uuxlelkf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aijlyowe.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ubbyxkcl.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ovntadis.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3zhbawlum.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yvspwsup.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gshjlirx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xvuyqayf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3twxjhrhq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xahzdatb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nsmdcnjk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3akkbewwm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ydewbghd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bbywwpou.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xwvgwnmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eirwgkaq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fvudjodd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnbjieqe.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bkyxhpcf.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3aredrdfz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jqbkxtyn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcizrzdz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iwyyunuj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3thlkkoey.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ncdwtcol.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lmzpmdmn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ywxisjtd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nnsgpyxl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tgrhvdel.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3esgvyrve.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3qrmpknsc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nsnfshfu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nuyxjxgt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3enxabwow.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3hhbujpfn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ikyghxhk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ddwlurbs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3iueyopyf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nxjgiktn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ravhbkuq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3chibomun.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3visatdoa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zqqosbbw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fsvhelix.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3vqkbhajp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3qhlqjpyr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3grxwfaer.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bcqjzdfr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fvwczxjg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fsuwewqs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3kkcrxufm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3elrmtgad.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3jlzahetp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ifgllmru.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3elstjewl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3errmetfd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gwpqpdak.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nddtemel.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chqymtzx.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lktchmsf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rswriboy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ayzymgay.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3roapeenv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mfujnnnk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3espvshso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3efajdlwj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3eznocnhs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jlhotwzo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vvadqfbh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qqulyfwv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3klmxibay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oeuegreo.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uvspjowp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xumweosv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vesmfdex.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dfxeujjg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fgjarndd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3fdqznvkw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3dspvuvvc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3peudbzzq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uxjdmwwm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bkudouop.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dysesutc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tkfzkfeo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oaaisncg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pvmcosdw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jlmqosxc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3baapjqyp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xkbzdcrg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3zvskwhat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bowzofgv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bobcxufj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qckspifa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3prbjqfoz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3shrmnuhr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3codnltzg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3abmgxqcy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3hhpxkkbx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yueivrvm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ofsldbcc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3jjquiyex.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yiolwxfr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xtkzctdh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3twayynba.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3magtmgqm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3gbubjxiu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ctqygent.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3jcowmifu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tndspoub.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tculwegw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zcmycbqa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yjizhiff.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3dkitsxld.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3cytjvcif.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3znbatvyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oawgvcbk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jrwgvrke.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3zvteuwcm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bcctazlx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wulxszsr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3hfixmlqb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rhsqzvng.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuohahhb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gsknmmsw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dqzbwtxp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mfzdgmsd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gnwzwlzn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jokshvzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gqhpvesy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3caylgapl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wuvnqpaa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3gylxbhiq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnyguwsk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3svzsidun.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3glwhzfaw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3shartqch.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3phrheafu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgejsxta.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ctlhlocu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3eapkwiqg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3buxxzbjv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ynhlzdjk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3alvnznnj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qyilxvve.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3gqlpbogg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tlxvpeqe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vvbhyqbh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3srsenrzj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qyjalrvl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3twwjmggk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3dyiyudfl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dxbsbyzc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ahqrlkpm.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ocdosfme.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zotyutab.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3lxwbiyvp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3gorultwa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3fxjswytm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vxsxnvfk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yvffdfhh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tltdffdm.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qolvwktz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3upfaczoh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gghncusa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iotqypfq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yylpbqwt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3aujmikfd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3coajlklu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3etthsgng.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3tabcbwrx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3aytmiumm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3sudsptzh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3yghksyql.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gwafbqom.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ycznchms.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sjyqgpku.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cqoodfpw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dlncuthb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ljkkbklf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcdylibv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ungcdbyp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qrybenhh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mwosnhzs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ewezkyqf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nvratnzg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3apevwpib.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fhzcwgzk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nevyovgc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mszrkazs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdkrjx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3cwwneypv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fndjspsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3yhcjmvwx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3sphazsmo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3uumolkbt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wanrnmwo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3fljrqixa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zsjskabr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hxzhphcl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3oeeipsxk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fibvupll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feckzfht.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3imhphkrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pglamjbh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ydrbfdtq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3kpxafnma.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3iyudqqrq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3wulddkwt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xlrumztx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3cyyofkli.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jdbknmjn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jmsyjssq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bfkcvbbk.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3aoifdwcu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3wbamlrlw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3enklwguz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fgqsyiff.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zcwgbcrj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3uisnejpd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3puhekdmg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3robnqxvg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3rkqcydmz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3papumxoq.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3tssgrofr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ptgvmjjn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3alfeepgd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tagfaypg.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkspfrkw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oxebeedw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3lapsxfis.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qfxwzdgq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3endsngdg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3yxkfhjwd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zvozzfby.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3rvzapquw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fuinmsfz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ozicmkqp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mxshjrhv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vfmoksli.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mjnrmyuz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3jxxwdrbk.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uiogppdf.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3cxwmktyr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3enfvhyfc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3wuqrfdls.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3hmolmwyt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3qlophtbw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ljqkurmt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wyttbhpl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3ymhsjkwi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3sqgvngdk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3icjlgman.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rrdhyfob.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dyjwhump.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3reeclwbt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qkcbbqin.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ambukqdh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3armqsiav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zcotlnmg.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrolgwgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joviinob.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pggsirmw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3meragjyd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dnmismmh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3opxmidvl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mxkibtln.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pcawzgnv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3anecccbv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nakcgjah.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ddnowvzl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3pkwdqsvy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3izihzoyj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ilzzfmrc.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3symchmfp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3lljqemci.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lysrpobh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mipjuskq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqvnudt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vdpnxsnu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gclktsdr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3qreyupqo.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yyiffmae.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cepfyigb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xhemqikb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ynchdtrp.html


<!-- 参考信息 -->