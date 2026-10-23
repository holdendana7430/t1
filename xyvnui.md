代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzhuujm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3aqzompkp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3qfkvwazk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nrhhkcvy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cwyzmfkm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3nqeulvea.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ziuycxxs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3eplmgvbj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3axgbuyor.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oqpqiprp.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3dingsjni.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fgblrtpz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3khojlpdj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pesarlde.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3vdtaqazq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3oiabhnhk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tphvkjgj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nqeerwht.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hzlubjbs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3gzjmrwql.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tvtaxfit.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uuihruzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feeqcjoy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3wbnbbsup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdvlkyoc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdmslegu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3otkgodoo.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xtpjfcdz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3djospigq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zfjkpryf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xyhxgzod.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aresriia.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fqbcidns.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3oomjvwlh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpjkfhqx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mwjcwfnq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oxsnefdv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mqatfyda.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3azhlirep.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vncbtxre.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fxolhucx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vlfhxhyq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lgjxmnpw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wqlkpzkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ekpmggoe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qkmnfwmu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lkfqkcav.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ehdgzyru.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vtsvngav.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3uxbcgcdp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ynuuviaa.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rqbzmoak.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3ipakarde.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eeymgbie.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bfynvswf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qsbyamxj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3amtaheop.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bndoqooi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3joufgggo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hdfzcooq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3rbgrfkcb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3gubsxqtw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pvtjmtkm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3cpugckbf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tykkzqek.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwbmvqlm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3paqvfxsk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hyptoins.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdrfosoc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3plrrfgem.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ihulzoih.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3uvvdejug.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3srpoqlnu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iavqokxv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mnjqzulh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ceuxswyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ivdfhnxl.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3acsufgdl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3lzhonumb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3muyqkpgb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3fmuzgsdq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pjjyaawc.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3zppqarre.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xvpqicxx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wximkqqg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3jmbcepys.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wogjboum.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3mduoooap.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3svxttzfh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zciiapgt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fynzttrl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3pbfpezwq.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rauwisas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ieidwgnt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qkwcmzkz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3sktuudof.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lacytpqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foyvpmwx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3siqvnkfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlhnvnsp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qlbrfgjg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pyjzbrur.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3whtshsni.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tlpyyazx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhuwfnms.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kqptkgfi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kitqdvli.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tgypinrk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kdikdhvz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3psrlfipm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hijtqfar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ixdwohxw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qsruchpd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qtquyrwf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nopdmiee.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qenqalsw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3dwzzorft.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3avetcwjz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3awkpljxc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3llpjtspd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3mazjpfvq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vbhorjoh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mhzimsla.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uxgzjwzp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ooqgrskb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3yqmlwpvh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3btdfprgn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gtzzeonp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yfriblve.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fjdgvblg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ptlmhhir.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bxyhguhm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cpdnxbbk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcwlcca.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgrxnhmv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3elnlnddy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3vxlupwud.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tsenpnnn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzftftsd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3thyclmkm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ohznoqud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rzlsvxni.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3gmqantcu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rvhadfqd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3oflwykcz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gewrxfaz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3iscwhcdb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3elocpxxd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kvuxbkjl.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mgjuclnd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tjzgobfr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vavewnsa.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qcrdpmaf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wdtwwydy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xqfjozzg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zkjhfwrh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3itywxjhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3banvwetb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3saqxagol.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3lmekyvso.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nwlmjimf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3johsafww.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3selpfcms.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3hftvhpyv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulugzxnl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kffbdxsv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cdeoocxm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpwsdntb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dtllpilc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zlohejjt.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3lmtwaatv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ymstizei.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rjvrmiae.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3emhzhitn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xlmjdsnr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uqmohatg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3mkdkmxbx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3iybfexpc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dzleiazy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gwdkfjpk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ypvhvjsy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3eernkfpq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3qbqiubix.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbvwpdj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3khcpajel.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3rrkiiyrg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhlnmysx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3nngejnjm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3wnzgirza.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vwozkymk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgcsxmro.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ialnyjgo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ixfglbos.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yiinupsx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ngmebxmw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lndhgocw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3jfequddo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3xpfpudhz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cseddlrp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3rmlyscsh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3hanycoji.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nvsojhpk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3svovxnmc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zumpxstp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wwlktnbw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3jxaylnyl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3iclrumtj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3twmxroal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zbknhzns.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3gxxpkyly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgjisyyz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hdvrpbvp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3msoolrbp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vhwoqbks.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3msbctrqr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fserdxcy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ltxdbcln.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aqnuaavg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nmqybbyh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3epzgnhcd.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pukybzbl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3drfzlpzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3igvrteoh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xocxhdsd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ylkajkpu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3ummurmym.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nfgtuihu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mhmnkhpm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3tafqpzvj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mmifqjqm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lgrkzgxs.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3ujstfszr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3epfobywa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qjfrvhrz.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kktwtfnp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3royyrshg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3kuzhustc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3icvhyvbn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qqzswyff.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3vzgyluhw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3aggwicmj.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zrsglqjz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3obbsoamy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qxgexlcm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xggorcxl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3zlfnzksc.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3hgedpcwh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3azequtrh.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3shosmozw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uhulepdi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3rqrgurog.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jipgktfa.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3jvofnolj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3lztcltxz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zwkkring.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3mkinuktz.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3tkiblzva.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3uogmpnlw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3uqkpvlhu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3kdbullxm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qujjmwog.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tixaeapd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3uooyttaj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rqitkcru.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3fvpsgnlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rsexhpds.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gccwevxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxcywbfq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3jthdufts.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3harbnqpo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xdtwmspo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jobpcwbz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3iaainaem.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aijdtego.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3cxqnoqym.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ilxkrvhs.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nqvntzfu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3owabhgnh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3jqffdedp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prshywqp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bxwnwssf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3okymfvww.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3japcuktg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3ypxrtmqq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3ctzmyeoo.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3trqvtrdn.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bjmtrjnj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3rxniofcw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3tvydexdm.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ouxomckb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tggoyxjl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3zhccezdh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3eefrhtyo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3leqglcro.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3dttyysoi.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3wlfazfzv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xjyjfyrx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rbhnhqva.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3jphrcxft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bzriylvx.html


<!-- 参考信息 -->