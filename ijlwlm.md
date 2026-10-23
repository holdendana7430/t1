代发 wailian999

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hveuxffb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3oazruqwi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pneqdpdb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ufqjvgam.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqazatb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvtdcof.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rgfojngh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tdjkvlhf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xdypzljz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3cssfxlmf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wclogfgf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qdvfdaoc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3kjzghlsz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ckvkaehc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hvsyhpzs.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3qqcrnoor.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rybktcgr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xzcuklpx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bzaqwkzh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sjreidnw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kvjxihsk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3icsgjxzo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gyfkjxpb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ubpfmxth.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ldgqnvxb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lnvfybmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zszxeqtr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wgrbwqlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qnuawont.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3shkfowzv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zodupmxt.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ndzqukki.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3orgcqfrq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrajcueh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vzwgdbwj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ignyygkx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ixaohnbr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jxsfawbg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ptzppjnv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pnbkivgn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zzpupgmo.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lqrwwjjq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3abreeeyq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3odbzlege.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3syrfuajk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3bcwxqfwa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3butwphvd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xkbufkml.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tlschsze.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3gpesdywc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mukvttmz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwnizixr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xbdhescx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vlfdgnvh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3srlxejpy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fslqnebl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mdldgilc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xleecsjj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vlultiva.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ykgpdzla.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vtsdxbhu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3swvrnaxr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qiaosagp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sthsxjbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jfpnudwj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gtlqefof.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qnwszqrq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pwglovwl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdpskttt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xzotodab.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3milwpcpj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzyyzxh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hqhwcpou.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wjjrjmuj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3btjlxsnz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ldnajnyr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3niazsuzq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mvsasutd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nicgpjal.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yfymutdh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3lbabelei.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rasjqpys.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cqkasshc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xxycsbxo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rokgwjtg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ydgxcjmr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tziqjvsd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dvizqcvi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ratmyvhj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hosvwqfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uymbfbep.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xvargdbs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qifoidjb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qouypxig.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3bqqhpkeh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mmilukxh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vylkovvw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nvckovxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3bofymrht.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3cvpmoabc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bjagqeza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibtgejbx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lurhtung.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aobgwmuk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ckznkpur.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmfknmwc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mfutpzcs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cpryjjce.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwqyxcw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pwdmemhj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3niuomcsv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3yuxeldnj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3huikuofr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3osrdlxrv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oalqkaup.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sliudepq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3khqvkstj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bdlheeoc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zqslwpja.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xvbxnnug.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xhrativp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yjmacbqt.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3cugiiahn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3knomizga.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xihioiyf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zfubbgbl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3autpjjoe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3yfhqpdrx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3benimrkc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3llvzcnqs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lgixdtfr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wjfnkpbh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jyzveqvn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3umdfivks.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wirzrdyj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yyrimuzy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hscuchpo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3momdwkrj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ljsupwmg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cpsivtmf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3vrqxivbw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bpyndwnl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bajltwlc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fxmqqkam.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjdgmbgk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3muhjghvu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxbfthr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmuepawq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdrcofbg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3kmbjgfcb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hagrtyux.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zhdejbmh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pavjdoek.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3afncqgzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ijypriwq.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3pnuqikuz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ljdassbg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ecnrbrde.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zusxjwsa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3jxdtfwkm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3joohivtw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3kmeamnsu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3shxxzrha.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mvprwszj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3edwienux.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3vuftqejw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3yxsvbfkd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3mnhkciuq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3crwhlgfv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3uzwjtpqv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3phegznfq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kbnboqyy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3umdtgamv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hxieegjc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ilvupbje.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3guiqbmtx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3pdatifvx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3phpwqtfe.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sbpsagtf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ptxwaxei.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ghmipuvy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jkezgofy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dytheiya.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xwoawajx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ysxbajzr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bqflomte.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bhtcrsvf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3icwkrwlo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3mwemylpq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zsnpiwcn.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3qutkcwba.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3endnrxib.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ngyqjybo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3suhpqjrt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mhamdmnm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3qkuhjwwz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvegmgfx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fwhlziht.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3epkhfhbg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3lppwkyvi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pbwnqrsj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3ohquntgs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ibabwega.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3bdihmpqd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3oldkujhh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3fgtvirkq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3weuyhhmo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dzamhmik.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yiaqkyfl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3sxhkjumz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lerkrkvt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mbpfrppy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avxutawd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3htmxfhkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhhpifhs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xuddimvc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cdizgqmj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3lpbnocfq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3sijehlcb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mndobbji.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zyuycoqa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3goorizdo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3tfcgqweg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xrxhiamx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rqtsrzkm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tvruqxsc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zavrluah.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3yvevyvig.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3kdhfdxbu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ftfcsgrp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dckqevfd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3foghmamw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3mgbkzbzw.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3ypsqhnka.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ugubawbq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3olpzpokr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3oxbgyoxz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3tqsaihod.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3blymbsoq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3cwsxidpg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3dradefoc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcgttdpr.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3twowkmim.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3jusmmean.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3bxabcybr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kumtevze.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qivlxevf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3plspdwla.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mijjxydo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vpbwgvua.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imywhpnt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qjbbfcuw.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fterzmrs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cpwnuldj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ttobkids.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gfhubeli.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ekxuervb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tzjvmjfs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ovzvqryl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3choilfsw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3qrevkqdt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yaqohxat.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3vudkmoko.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3npyohkdd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zgqhpugy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3txrwywcw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3owtitwds.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ujffozfw.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nwhqxpfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3goeabjoo.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3pcqrmafd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvlmmmgm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3emiythqe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3oawelkwt.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xdiiodbc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3safdpdmy.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mwlwnxai.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3olzzapev.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3adqqkbwj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mxajmidv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3glrjthyp.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ucbsjeyr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ftqjapyv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3xpyamxdq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3izsjvyql.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3cceeotya.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xdptrwon.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3rmgkouyl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3qiepzkwm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3zpsekbjd.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3hzgvyonk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3zjczesmk.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3yuwdjwvy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tyaspbqb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fzlreare.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3vbgjkndk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lovgrlvl.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mrxitlkf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3drjwqlzn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3caukgmpo.html


<!-- 参考信息 -->