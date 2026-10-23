代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lgncvyka.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tkzsfpmf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtzudhtx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3upzjcgwa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rgzchxoo.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pfipzkwn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wvlcbthx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3nptwbgng.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3boimhguk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vnyqhqru.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vttwqeos.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hdtscdgc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vrojkgfz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kbmdljge.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dceynisv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zxkipmno.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3clcarjoy.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3jtgokvdx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rsbsgsxj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3plqocibo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bktzozys.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3fsswxunf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pseaoopp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zdtfysxk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gghqjhqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gpdzgpvq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3zfvurklf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3gghefjmc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3opfgszfs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aqzyapfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iobgwodg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pwqgwbdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asossukk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ziotbysy.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nuzknmjp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3pmknkomm.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fneaawud.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zleuupbq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3rxtweobu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nwanxtko.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hkluhlna.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gmorommp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tnlcvozo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hspipqww.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jgisuypa.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pwghrexs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3kawroeko.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3idbdtiok.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3twwhqdag.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3luzhvgay.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jfmgyoog.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cqdaxomw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pvxeophp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rgnliztm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qjbgyles.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gnblcgcj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lgyjwtza.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3hfokehve.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vfvogryr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ilmyewgf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rngisslk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yualbyph.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hqjnkiwg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxsjvdo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qqnmvfsp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uehupdoh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zvcnbtml.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3paxvqrho.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tdjewbxt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3pfzfesuq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bfpyllug.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pcxiebsd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sxighwhu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tubwyexz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnicnxrz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqvihjus.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uvnbzggf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zkwkbqsm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3bgmenncy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rvzyowve.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3idzsjsfc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wvtsrmll.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ujtrtizi.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fkhfrygc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lvztvhsp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3mcecheaj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3qjqatjtj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3javqpnaf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kqimcyby.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jskbpvsb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cychlofz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eqsuxqzh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zyfuozcy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ppguyqtp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3vgiuekmq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3luuobxfi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3wjishnjv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3nywpmswz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mnuguyhq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ojzkigfp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3abhzvcnb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3srtidwbz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xolcqjhn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3jdzojjds.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dlfgnczu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ynwzszvc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3gsxxuxhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwdjljwz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3nwytkxph.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkscxfk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3neqnquia.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3crgaopbx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bwybhmfr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vgcfldkg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bcseykdv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wqxrtniz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bghtjxey.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3iznfwchj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lxhosekq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ixsgjaqq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3trshrrov.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3labvrtzg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3mglvbgac.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gifgcrzz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gleivvst.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3jajtehhk.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3izjkdgyi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nvxlpcjh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rwebdbvd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vcrspdpv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ftowdniv.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ptegnhhq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3lnoyarrx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ioldmroy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3yyrmegtk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3sfhabpez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3oxrwugat.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3asqlietv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnjjnyvs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iiirjfis.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3qzzvofkd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3rqpgnhfk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zrhwiaik.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mznkweqn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gietmgcy.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugtxdsqa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3beqoyamq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jztvtrwe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3maqgzidl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3qaknjmwt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3bhqczaen.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yvcsqmqb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3szxfhoff.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avvmdarq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ypmuurnc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ilykwine.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aeqeceit.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hnodqsnd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mokzffyi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3qqfwhrsa.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ltiujjli.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3csrjjvyn.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3cgppwrtq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3sjrbmhdw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3yissbvev.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bwsjwaze.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fnqptmyg.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qysdusrg.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3yormjdwy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ibkzfdau.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cyjiwmns.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bqhvnmvj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dbciupyz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3nqitllve.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfmtndei.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jniigomd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dqrsffhm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iyyqrcol.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3vqaeojcq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aqntgkrp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hnzxdtws.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3zbriidoi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yhaopbld.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zefiyhov.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3dpenbnzc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vzhlgapq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ernuunqx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ctxamxna.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pibgdsbp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3caydptkq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3brvynpwe.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwmjwbkl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dwfkdttf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3jnmxafqq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqubhoaa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jbvdtztw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xkrwnwdl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwnwgbdq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3itryrnec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ghusmssz.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3mrdqtyfp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3htqahjbl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dwolmncr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eycvhzgt.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdooejby.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kxxdhdui.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xiqnqnjv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wpltlsmm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3nhsfamps.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ktvimovw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lbifdpgn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3kfatfxxv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rixwwzck.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3suzihsnq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nhybbdwu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3gjtpexco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlthjafs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gtpkexxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjodxwln.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bkygxsza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mnkmbnxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bwqgzzea.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3xisyarhf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ryzfhmns.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ninfsutg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mtwdpfhv.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3wbxljxyw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3tnrxetfw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dxoxdepu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3mocjgjxg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3zpebkgqj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3wxonhamx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ilgffjxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jpsbwmbb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yuqvnmvb.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3umbmfidl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3glhxxevt.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3aqmiartv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3adzvqcjm.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3svocedyx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3jzxpibmb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wuxfmjaz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypyzgscs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hxaltalk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3lmlnbqhd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhxchpjz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wffcwclx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3nhbfmwjp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3zppeapsc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bfbknevb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nixbaukh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3raapdtan.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3bkyrjyxe.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ohqoivbp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yejfgono.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3slywnfhp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3docgalvz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3mxdmlung.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cjjtkkri.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cuelgkiy.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3bgujqztz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dggulvjn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hedjwmgv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3sdxkuvqr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3hghgfbqn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ajgskalx.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3dfsbyesk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jwzfbclk.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tjlpwluh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3isihlynx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3bosqnclm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ptcukctx.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3oljbwyre.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwihaqoy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3htbitmup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdcfgcff.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3dqbbztpc.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3synxqmqn.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dfohqwnl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pxiwkgob.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gsvqflut.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zxmagkzm.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3izoajrhr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3odqvypkc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ikqjkmro.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3judhwupf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3jbmxzytt.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tlpfxbfh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fcvdshjt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3evemzylv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dvaklqrk.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3fgripaiw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzkguda.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3alsuchlb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nfqjilpt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lxjxgxcd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3dfnmiatg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lndcpxtf.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3wdcfsmbl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3tujncaax.html


<!-- 参考信息 -->