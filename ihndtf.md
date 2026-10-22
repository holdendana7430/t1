代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sdlccwod.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bktcudip.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qmavayvo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2bdzeptus.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2efhhcteb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kydkwblu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2noksoiub.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gdflwbvp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2knxzjtas.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xweevraq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rgjjypfc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2gkozokyo.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pogkunnw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tofmoxqm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fogppzei.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2seuqylks.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hvvgjatv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2irivbysj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nqtyqsda.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cnfmbeix.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2svumopme.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gvjawgsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avdsebcr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cendyhgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukyuncpt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dpddrrny.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2urfmjpye.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xxyjrvds.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yvtgslaw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2erhlymeq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ntxaegok.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bsqcntyy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2divcvrlq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ewlfxjgk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pymrwmdg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2noxuhtgo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ygczrhof.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rlinmzoq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sndjhyre.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rewcbhaj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fojxdfer.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ohthkens.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2atebqvfx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2afjsbhti.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jknvhzrb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2mkhlnnze.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2efqttxtj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2afoygidi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2goxlmtjg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2izeritxv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rzteoopg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rnfbbrua.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dblgsxqi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gruvthqs.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2urhyfkon.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uezjrgfs.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kwqdkqnh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2saekslrh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vbkpxuhu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ioptpkdf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2zozklikw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xsygsiui.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzjhtgj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qokcceiv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hxrlaxnk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2verblhzr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hrxyhmxm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ofwhoivx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nggmguld.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cjhtbllt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2putizwfe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jncdxebh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2aqubdhzd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ghbfywxf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uesvptrq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ozjgtgcq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2icsagvpd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2mxdbedbu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2frnopjce.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dnckwtjq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rsmjfvgx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2qwfoqxiz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2daohehlg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2oseiimmr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nznvzrzs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2waqezlwo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kgvehspj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gdyhjsxm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2oghfytyl.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2soptbxpz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2hntsnnsm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yfnuecsg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uavigtrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gnlnbtij.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mjkywjxd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fklmofro.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2phvlwkii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxgonexx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ogwldhdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2duydvujb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2alijkyqj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpjlccxq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rbbudntq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rkrkzqca.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmxbjsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ygqyadkq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2icxswwaj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kpbmsvmi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijguqdfl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kwanucla.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lylmcplf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gsburyqa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2nlhfcnvn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yruqblaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ckyrcsyk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iheprkld.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mxpjkedr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wywexdcw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2dtqybccb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ravzfpnq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ujxddmgb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ohcwesqw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ezxcofea.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sezcjhet.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rtyyaorr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uftfxygb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2adbbvhcx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kldczxgw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fqennpfg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhguxiql.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puwsvywg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iozqskub.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kipwgtpd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hdycoqgh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ngvxukag.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fqiyhepa.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2cpybtyyg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qyvqsasr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqjggekz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ewijcoyt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nofyodbp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rzefdkpg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2svhadard.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2skvlokwi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nsdermdj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jlppuggn.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tcyaevvg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2glzqjful.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ideiyluv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hcusiqcg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fymlzxtl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rnyyojnb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iabeyqso.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jznkowmc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2euqwrqii.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2teoqsrsz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2kgdmnagj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2pceggled.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wygzrrhh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sfijpyce.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2efwwqsdg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2jkookzja.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xrbdsfvl.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cpfdukmv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2msnfovrt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ennixzij.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qfyolyix.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xeydjlbi.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwzwwjyk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vdkfvmuy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vyweqzwi.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kkibddrz.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kdkuaagl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajmndfrt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iascxuln.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zmbeoaci.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2dgrqedsx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2sijbrzly.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zdopsgjq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2osspgxoq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ttyrdhjw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2owbpenbj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zdndudcq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2lphlmjee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vagvjmeu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2kuawqkdp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2pyojgndh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2cnxwwwsu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2papceioz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgdrqlwa.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vmdrjots.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2uqnamtla.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkgajfbu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2haixmjem.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2riaqnfxm.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lacdjflb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rjhyixbz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wktssvqu.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2viexwxdq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ahjwcmoa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ckuosori.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2wfuobdzo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wjilgfoi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nomowapk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2imizpdks.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgprgowd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2vfdazvlu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2muyujvuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcqkzzhl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ajjkrzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rprgwztv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tnefpfld.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ygcapfvq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2hrsauglz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qyysxhrp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rhzpevha.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yyarrxgk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oaghesse.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rclehdsr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2epglcmts.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mlqkfjlr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cddsbwdk.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2haasvvqu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gxmqmpnx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zuighcuf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ueunqpbd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ldqlrqvu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2hqgueyex.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2wbgxmwan.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xvpiiigc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cskjzvam.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2xuunynds.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qennveym.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cupnlepw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2exizvljs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tfpikszj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xqajmvfw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fsocznbg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2efzecpnx.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ayauvspo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jidirtfw.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hdokdquz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upooaelg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2lyvmozvp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mmbcjqzk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2lmnqvzjk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2anotwblb.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2dmeizcxf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vptmffje.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2mesawgoq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2yyekydga.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bibqclpu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ycphtrwj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2ocepzfir.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cbasmffo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lejnewhm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zusnztjc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2bdixnzjn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgiwmaqd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2udezkeja.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pgduubyw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbgmpu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qdptjegz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2xyegtyss.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wihvwhhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbojiiws.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2oaqcypmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gucolyyr.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2izigdbjv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ulxklmex.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2rznidadv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ixudeued.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2stgtypht.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qrkpergw.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kjgzcceb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bphlporv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbctsqzi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2uesipkbo.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2clwitaps.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrhqnred.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2phvwagcy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2inbdiwoh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xjicexvg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2camrqfqt.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epgbqyze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2hlsytenu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xcsoemhg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vvnwzify.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yuyaodtv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qomsxqtm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2sfkawyfh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dwmmugac.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ctukswow.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ojcnufxq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2akdfnytf.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2usziebfr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2obuxqmso.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xcskqmee.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lxqzpwgh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bspaxqsq.html


<!-- 参考信息 -->