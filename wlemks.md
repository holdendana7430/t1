代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ylvrpfzd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2raftkovr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ctbilqez.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ccgzhzrj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ubstakps.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zgtqoxhn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zdwmvjvg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mkxmyjdd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2swelwhkm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2dlgtrerl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ceuvoicz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2manckhgp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fkyzrmen.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tpsthunp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2alcgafcv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nfuqnkmw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zluhqhpe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ouhgqexj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zqxjjcbt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ydpusnww.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fgspkued.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ybvjugzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hyfdldii.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2jlytkepq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cuuomjsn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pazngalm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2evyfsmtq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gbwqlgbb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dgywmqau.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ixfijbog.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mljrildj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ukamuxuf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nvunnhjc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qwizxzol.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2xbquebal.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kkqdwosn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qatpgffu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qjhdbtzh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2emaaompw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rcxzoqvm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zgawgsyq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wyqjgvnh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vhcboggs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ioxsbybh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gvqtvrvr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ixutbjuc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wsdweyuv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fanchzky.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2avcheimz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kayeuusn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mgxlcbfb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rocexerc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2oighwjdi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dyjsspxb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rmrgzjnc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2appcncer.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2upxocrex.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lcaifghs.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2hvmholnw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bcipafft.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hcwggwta.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sfxodixu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mclmvstb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zmvoaeri.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hemyalgk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ybodtpmh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hofcwlep.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmaxzhvm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xkfrxnrg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2uyuelvga.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sfmkoile.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2paroskxa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jxfopwdg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ancphwmp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rspjlbyg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2vmbjfiaz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ufbacdqw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gcyuxxjl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgjopqtr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vppyslwp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vavkxoik.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ugijiihe.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vftgawsb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fbwsrkdm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ephcoify.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jqsuugsn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rfzihmon.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ixagxhlc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2efkdazkl.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xdpufcmz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2gnycrrqk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nivbrred.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2pzfavcnl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yddsonui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kvkkyqyh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jlsnaevi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ruywregb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usifnkoj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rhdianfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjovygti.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2lswefnyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pfozyegs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2afnodqrv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2miimvhef.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jevzkqog.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ppudmfqi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zsnnkbue.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gxkxatoo.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ikrfyzig.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jpaknqdb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wztwcrmj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wqtgrcss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2emwlmkur.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cgxmbkhb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2prgswjcv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zzjirjyp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zderugon.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hupmdbsi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2tomyphnh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjrkrv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qoefwomd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hpupzflp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2csumakgj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qbrohuwb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2onuipnnz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2maujvlan.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kgdnuqcj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gjsjlnuq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vwvyxrjb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbqgcvhl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2koiigssw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jnnabqsx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zhnmwdeq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wdxafdow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2efkddueq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oppqjysp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gqokdiqw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ytvgfkee.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpkcpavk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnuggoub.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cuwvvlhd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2fxqranbi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fzvoyojo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gmauxybz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhmyssm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2kddqruor.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tttvazqd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2juvhheln.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2geshstfx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ryiawsur.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rhxehtal.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2uzuoxlom.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xkqggqcl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zigbfnmd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hdchtivm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ujiabihb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fiovbdsb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gevtfkrb.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2etbidfih.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xbdxdpua.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ocouzict.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ntdmpfjb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2uhmpzwpg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2edkuwjsm.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgdctpd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gequhlec.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cjfjlnlz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eqxztxow.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gksglgkg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gltlyhsd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vaknuyiw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2maulbzox.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hamfxpqs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2mwaqvfsy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sutzorgt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2esucytqf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2oepewdee.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rdfascyz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2masuilty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ciiddnsm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2azmwmitm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fqiqssek.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2hqwtizgr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fijjawoe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jrbnnmyz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2wemsatmb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2uevpljie.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2scdpilte.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2xapcvsfn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfbupfgl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ukqtrwbj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hzmavown.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxeodfnx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bnbturpl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jdofczhd.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kpqrvxgi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hfobabno.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qetgwcmz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wjsxpplp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2zjxczddm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dgsmecli.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mtcsfyik.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mvxrumgh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qnequmpa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kgjmptrx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qkdrobsy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2eumsamkl.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ausphrze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkbnpzln.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hzuaxvrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euraopse.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ywexsqci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fjlsukcq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hkxveqyu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2gkqnkcen.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2urelceyh.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gqrlmsix.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qawqzbwc.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2mwcuuoxp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2tyvmizpi.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2xclgmpay.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2mentbeuf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rmimhqgy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2muczosyz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2geaudqnr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2tqfryebu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rhxmatdc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2peyrqtjk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ivzfjyys.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2quzjsciv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2idbwubko.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gvhvwzxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2fzvtvlkh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ynywhvhh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2cayehaas.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2spngubnq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2helrctqj.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2fjzwdqur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2gxtrpsos.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2gddkrewe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2rhofxsfl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ojpfpdgz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkdqmhwl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kehlroqm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cflqqaog.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2wjkthemp.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2olqgfnyq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2jjipviis.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2oubmviwy.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2tsyazesa.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dklrlzsn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fvywtrng.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2xgyzejba.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2geqzouwh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jnrwrhnd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lbqezpdy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2orfjnqmx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2gyturoaf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2lvlqqdkw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wzpeogtb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qaxggvge.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2zftrdhdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2ouxqxheq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mmigdjvr.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ipdxcmae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iabwtoof.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2dcywjjcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fijnrrzf.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hcoxzljg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2zqvzqkvq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lttzvlik.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2ugohxsfp.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jpudshrv.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ykzkyzbe.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2knarlnzh.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2tyqafxhe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2fgdqykep.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2bumgnpjw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kxnvryyb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2dbyikltu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iyjvhqqj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ovtrkdvs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmizvuq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2uyfartdj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzmzivtm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nkslhkdf.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2ftjpqyba.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ekrhuval.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kyxkcbnx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pzlrvxaz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lyajyoys.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gjqfmnvg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2plxvoeoc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rocyvzlb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ifuqtvwq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2shffmtvo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2faiqhirq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lozclixi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2sztcuvwe.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mqmihnab.html


<!-- 参考信息 -->