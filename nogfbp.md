代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ptxhortu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3esldiehr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3raedchls.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jwgewoqo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kyxgeneq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3fxkvejue.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gzjcxkxm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3knoclezl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lclbvptl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ksqknfed.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wewhzapd.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mmnrhtui.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ipderczw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3lzhccfyd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3chyzvmkp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kmglbfcc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3usxckfmw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bfspaggw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xbtmblub.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3evizkifb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3quweltti.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zpsjoujp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ltkpqilu.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3atomlgkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykiwhcnd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lserficc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3npgztbcb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wyrqegbu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3zlxtigvl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qtrtijjv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hoarfdau.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3wldarjew.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mlawhekg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pnvrqyuc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qnezjbzp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wfmvnsrs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ubmzmrwu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pbxnlfrg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nvgdtvpm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hoffhfxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sbembhxh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mzlioveu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zzwqfzvn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ncwdyrwz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdcgkcy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ezvbinju.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ztkglelj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qtnhfovw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3eebyfyyt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wsrtpcnl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vsvxymgg.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3haysawyw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3agjynqli.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gxnciiop.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ryhicfrq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3onimzqng.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pxsftswl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3whxkaixg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ftvpknlw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yqokfvuf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zbrmngms.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ulhsaxul.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgdlssm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3rrmmdhmc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nuadtsfo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3stxakfwr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aiqgfezn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eqgxgasd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3rilduqjl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3klqjbzhk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymodwdge.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3scjzoewr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qvzxkyct.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vlxaskek.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zeaegwie.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mxhohvli.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3tgjqijup.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ocvojifs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yucunayd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3kvsrweyh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ccviketc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vnscebql.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tffjikcj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fbsjwzuv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wcwizfff.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rtkwjfip.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ysltuhqd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dcnfdlmp.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hlxnqvnw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xjvxzalq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3syuxsqjt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmnetx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mkgleyqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ggtwixcw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qoeonnnh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fcvgleyl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yuezdiha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eaqoetth.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3zprrfqms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ommjzzmy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3avazepkk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zquigvfd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sersnglt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ixmfvfwa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zobrxgwx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nejqrssy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cqyahbsj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nxxvxyqj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xcrxxnuh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ehhlabrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ygjjrwym.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iathcpik.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3efujaimr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rfdfkkvf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ouywpwqz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qixjldff.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mdnhtwop.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tybmxmhx.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3srdvlisq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3bvzwzhtg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3xbvpdgpx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uxtxsdkl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zqtgodmu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nrfjsymz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3sajfxdgc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bqfazbue.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rudvyvzr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vdttsfek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3utpeykwz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvykuzva.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bzpfozuy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xrvwtazs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bctvzdwr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfqhbig.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rtnmxahv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3neekgkix.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wcfqmhnd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zciemyie.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdbabhqn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hboknucf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3imkdyvzj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjnwds.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3scxretzc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qayslhln.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bmxrbarh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvgvbbnf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3zpvqdcmr.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ewwrfovw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ecvggkfg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wnbthvky.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rjsqezxs.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nkxtuteg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rozwrkju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vvkzyuwt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3aodjqzag.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xnzxjmaj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nerfolfs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3jppnnovh.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3blhfinca.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3lmudvuae.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3lygeedfc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zounplzq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hxiedbjy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yvftdesw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvzwbus.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3zlfiheuy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oikxafdk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3chdfdnrq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3apnbudip.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jpcvcrmc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uwngzzyk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mgyngmij.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zgkrfkfu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kybspwqz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ywyckrbt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fpeupdlc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nfzwdsch.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mrrfwhfl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3jczimaiy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zgtzlvux.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3yijigrdz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3umvghyvq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3pzgxcncq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3tmlhzgnd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwsszdu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3murudack.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkfuplhl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3vvdxydeb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nltctmlo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wszzphdl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3rtklowiq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gwqkkkry.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3exviqlad.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cojjzzsa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wdpbkqwg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tybgzmbs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3uzqcdidd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bezqcucc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3exdzljhd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3hrghfplg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3pqmomugz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xlhebafp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3bjdievid.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dqupjhml.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3yinfdnbp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3uhgqvrsv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mrghepjv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hczqdfwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dttttkvu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3iiahbrhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjbxjweo.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mptvgpwj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3xcwddghv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3hoaoepbg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gutuijxy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zckkicog.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wkhesixj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mhljclth.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3gweffnix.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mredoqoq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3fmvbwryb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3hdsumirz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hgknwcqy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3qdzpobyf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3pgtspqju.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3leshcnts.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3kiktiqzp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3thibwfkw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3pvskygnn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ptyslmfb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ubqcndix.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3gfylspme.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3oyefjyxc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3fzjfgpgt.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3slmjjvep.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ftxkmmsv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3cbhtetzo.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3tmtsurys.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cdlsyydh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3cchhmkfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3xfarvemw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjeazosp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnbflwiy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3buxcqbxb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3ixttlziu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mbgyfcgv.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3qwbntaif.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3orjmdfhg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3pwiyrbkq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3etyyjmer.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3oydsnlwv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3umuhiyuh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3uycbjdow.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3nafatqgc.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3qiesrmqr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jzojyvib.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3yijzgpfv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3gphtrjfl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbpghmiz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sxhvrpdl.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xqyojrcq.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cmycckjo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ciaojfjk.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3kfbbzbkk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3cncievyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kniwibfk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3yebhpaqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggyhfhfc.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mptaeael.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3otgscwjo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wklwaepc.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3tsrqmlwi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kvzglzpd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3uspforvu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3rarmuqlz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3gwqpwtvp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3owrzuipz.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xhrxcvdg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3tnbscbar.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wykdntao.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3gmtarerz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3yqatcslu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3agcjzjso.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3cfpcpcvz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imvjdyea.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3suvywvli.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3knkzxccn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3nfgssgsd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ajmnyuxa.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lmqyodur.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cqgyzsrs.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3mkampmrt.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nmpwkkpp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vlmahrsw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ftjejfnr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3zgduxsyd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gksemzny.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ddrarabp.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ccgjgifl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3klyhjidk.html


<!-- 参考信息 -->