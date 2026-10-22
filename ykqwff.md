代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jrnerlfr.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2dmheiniw.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vrdpafwb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ttauvlxw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yfjqdava.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2htsbfrdm.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vpdpxgcd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2uduphaai.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ngfrtbyc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2smqoaeoq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2dynbwsfq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cuulmfhb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2npalkvma.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2gpphmwqv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kiglcdzf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nmkermwy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nuhvreet.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fxeliuyf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cirnueck.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wwwsrmkf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zuwwzvdc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yshwrulp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hnsbdlig.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2mgnkxhgp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmvdcwj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zpmqxhim.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2degcgyuf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2yriawnnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tufhgidl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2azjkjdol.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hxqnoabm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pzmdgkkx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2emebvjug.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcflhff.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xumxbscx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dtmmefcz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yhstkyvj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2opbbtjax.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uwhynuhg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2osebcojp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vtlavwsh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dgjacafm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iklqyptv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2gjxwxqxw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tngwcxso.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2tcpudxlk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bqpzcnpq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ohafqdcs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlwfjtss.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2taumtxwq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2auaeqkwa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kolbakzb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2yfdbilqs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2erypbirp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2maskjlbz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ksrdytdw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zffxxeck.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xypbtgab.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ultwhyeu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rbbotxly.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2msgeuvjy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ougdcwes.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rsvipjcg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2aolkckft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vbhvzojd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2limcmbsh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sbfvcqsc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pqrlhera.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hyesxtbd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zffjmcps.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2twxovlgg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2euyqcapv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mmzqtgoi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xhprhfqh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gannhdxb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qreklvzb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2otjehdaa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zmekcrhm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ezhukadq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cqcvpdxo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2neesglvv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kmtfnynb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2xtivmvlg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xwbwhxsq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rknxrbqp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jlwlvvqh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2skyadgry.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uqksbebj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2huuqivjn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bljfcprz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2egeimcrm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xhdlzyxr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qxmqbxqg.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lunfdvhy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xiwnbqes.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mheuxibx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hkowwkxg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kbzgvred.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jujmzynm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pikelage.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2gewnhzih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxaocgag.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lyqiytpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkxnyvfl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2attyaika.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zyjrxxza.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zetwgmzn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xeqmvovi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vlnrfsdj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cditrnrt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzndfurn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jeejcymh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2itqgiyez.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mnxvatnw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ssamkgqb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2adjtnlqa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hlsjtjxg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkvzity.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jamqobun.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vskqkyfx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wvqpzaip.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vikkqdxu.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ddxfznyb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2iirejjmq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gxutnxbp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2moihlatd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nwabnqev.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kstcwvyb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2gtekrskp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xpwsrlot.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2xzulklkd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qrbxpdcm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pxpcrsgf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ucgjpbif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2siaptayp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ykuuctca.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tfsmjvyb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ikugivcx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdvhjmgj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2klyxegrw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ohawqfpl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tmqnlniv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rjxqbzhg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qzyrzdho.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ofrhzfke.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2uxwadior.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oapfxxlj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pingdqng.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lnpoeoka.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pgzvlnqd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gxhdmzsy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hbuorvxb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xvoztauq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2upmmgxrj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gmpezzkg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2fghvxxnf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wilfekme.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wpvxdxek.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nkrjnzfb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ijszneko.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zoonoibu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kulnpkfl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2piloleul.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2eymhlgsk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jeaavsyc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pufgdtpp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2axizrlsd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wdrlnbgt.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2leptgjkv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2kbrmlurr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gsjlrfqo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rafaddct.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rkicftsq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2stcglkql.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jefzqxqu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2medbqswk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2quidmtbl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tjexlgrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mvqiucrh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ukytumgj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ibrskxim.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xyzyqnzt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2dcpfpbsh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mfhiccer.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fcvrwfwl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2jkgebxbr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fbfmigbd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntetpylb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2xbaugpbx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gbkeoucs.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2loienrfx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2irlbhlbu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2mgjbtimc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2bvoxgjxf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2evwqavbu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2iapkrand.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wlzzuqhu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fdmwchlp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mufkzdmn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zdjgflus.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zyiqvspb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2yjfmlipj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vqbtervc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ghxynxth.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2yxiegmal.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2uqfbnuzl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2naxcuogn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xilusmsn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wolypttm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wylszkqb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2jpzoiilt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lmdjaodn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmbbelhj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vrxbceqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsjjquzh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wevckpwn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ckrnaner.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2togpgims.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2evlvtfci.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2alkhvljp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ktpeygfr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jsiwtzep.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2kimyfcyx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2rsceuslt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2bavooixn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2naianucv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xkeqfenu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tihupxvf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2exqseepl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lkptvhwj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2ohbzbyxm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2dkoeyait.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yszhazxu.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2uoidvxsn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpagofub.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2fcggmlme.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2juuhssxs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pckwdblr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bzakwdie.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2kqguuriy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jgmjdtfh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdxosqkw.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2imwmmmnd.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lmrstjuh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2yqjgkttb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vnvrirrh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rfcheqvz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2bfdemcbx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tvnlodha.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cpdttqyg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sncqerfo.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2wxudrphm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gzsydhjs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yxypxsjh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qpcgckap.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xoppdeef.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2aiaeodcs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2pxaeputl.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2inrlukkt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2linjvsbr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wvmulmsa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2wdnjpfdd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2kholvtmy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ykkjamqg.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gbxjbkdi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2ogwoxqmx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xwxgswtv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2fpikszev.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2kgxbuxrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2secrtaqa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qknkuotr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsnrtzzq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2agpukwro.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2rgjftcuh.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rpzdllyt.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2scfzmfzn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ikpzvczu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2osxmqkyt.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pmxnvidi.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ylyztppw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zaabarkp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2tbwtqnbj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2kckfndlc.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2womdwyyf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lvkjimyu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bgttkgmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbxgnvb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2yruiydnb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqdbash.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2joskoljs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2fjyedgts.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ezusohkd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2vxrwhpcw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sqjgihpq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ydnusbwp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lqjguixh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2nximnfbk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2easdbble.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tsyizbxg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2rkairwzn.html


<!-- 参考信息 -->