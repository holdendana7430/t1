代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3wwmcibdn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rftpdqph.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qxeditgg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3splweqrk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3nvelkedk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kulxvfad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3yiezoniz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3lmmxnezp.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bdlweidb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3pxmkhtae.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3giuodwue.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdnuyr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uowbzgic.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lowgwrqd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sercdoma.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hydowsic.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gfihufqa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdvyxuwr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ymsuzsqs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3exhipivy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kobekmyg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ikriupzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qsmhndfe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gharetge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpsuahga.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3eoakdkgg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3iknruqms.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3umesyynq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ehtthzpb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfzxuqhq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qxykadqo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqswdvld.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mvxehxgm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mlejqxqt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ecdsnnlw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fpbnieyv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uvwvcmme.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3auqvcwii.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vxspswaz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uuufwbql.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ggbieuuq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zpeobkmb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cpdeugnl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ejdjzmjg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gveniapp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3swiddatc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uboucfbo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rkthmwlt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3vlafjbeh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nthkkyfu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hjuvjfqd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nxuwhqlu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3nefpcxnh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rxgvycmf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xmoeggfr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3waoxhaeb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ncmcfndo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3hfjnuebc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nelslorw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dpgnoadg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dllrpgzg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3evrgbmin.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bcibyyhl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3dtdxyvlw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jpzwhwfp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgoftdwp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hxhgykhw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nwcvezus.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjnpzwwa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vctyxxvz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kmnwhzhk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hzfkjyqg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kgixcbfh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hginalfz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3odrujhit.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3tssebfdz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3catritlv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fayaczmh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nazgpslk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xtqrsvib.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mfezvkhp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vhnkgqcr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3idvnibxp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fqsufsuh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ammhqunc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3efyckyiw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3exqgaejc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3iqcqafdm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3uuyzgwnt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ifgbyomx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mbtqwbzn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hruflnmr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3czzbmjfu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3tmljmgrc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zjfslnhk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tajrgiek.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gqvfijow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaqwmimq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wmoqsbsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3udrmamtt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fnposqvm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bffdjihm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tbvuojkr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uguejhlz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iuplatdj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rtwrrffv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hfsiexit.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3duimmofa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pynmscyd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rnywptzi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eductxzj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3milifiey.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzlsjtpp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xegmjrbc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3htlznklo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkzfmhkf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3feyfevov.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zreoutrn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3txoolhiu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ohmkqqbr.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3lxvjktud.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3frmlbcji.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gbgnupyy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fjycamhw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3gwhtdgvq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3irinysjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qbjgucye.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3jxviegsc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ksdqaram.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xecwxxcd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bjrcragl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qndsdadq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jiunicnk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3jatdmphz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jmwqdrux.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3esecjoow.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3gvrqdbli.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bvamcjcv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcgunpl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbjtstlx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jszmwsxy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3glxidchx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3cqvjpqgn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3iulgmmrm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3evjjxpcf.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnzdyzyp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hzyukbwb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lfsveuif.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3errvgrkr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3slbpxxnl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3fmancljw.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ktonjmxt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wtkmwpqs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hctqaqjx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vsxuoqhz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kwtthlmj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ccbtbpgf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3leehqnwu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gycjxsey.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kveocqot.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vbsbtbub.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3grckiwjd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bpjaqejh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vgvpaety.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3trhldzho.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ventjomy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qibiycvp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qocrgema.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qfeilcfe.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucdbpzou.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3omibsziu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mrewdmfv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nouheuas.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnjhhqye.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3eanxormm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3knzqyjdu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3uheobzly.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3chbhrajd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tbisicwy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ebekynpe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3xbtmmcho.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wjgxqogm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3lgkauqoy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3eobyqxxs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3xeshezzc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qvidepao.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lysrogqn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rqxebaco.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qggbsmnt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygrggvfg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ksfeiwns.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3eoyrplba.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejhslojd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qogenpfv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qxxapoxn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cgaqndqe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gofxowcs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fqbhlcrf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3thvoqtca.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3ozfguabk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3aikmrmlh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ttgtdoet.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3rcrorxay.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3efgscocm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hvqeivwe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xcwvuknv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3vqtvfczz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ifmmxlhl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahwxvqjf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3rwyglhoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onvkmnzu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3giknhqae.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vcdyplxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pdrogneg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3jkkmpxmt.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jzezvqpm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jtwzdwdx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uclrnnjx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mayeenuu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nkwrahiq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3satmieqb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrtyiha.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qacixxqb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3idoxjlqk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vbpuknpq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bpzdcwqc.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lhybtqdm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3awjiilok.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lutykwds.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3yeomwiiu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hkhfojef.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3gelcqbxj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3sbzymhie.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rqzirfxg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wlaxwtup.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3lznlsuaz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xolnnuua.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsekxpic.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3aezqjpnx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3oudvlvjr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3rfznymlc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjlgijfl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3pdrquyvx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ehlaexxk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3duvpfinh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rdblrckk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnyqtns.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yfkrkmnc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3mlzeyywb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3kvsqxgco.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ifepmend.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ualilbfg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ciaugfye.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3oklgwazw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hxwxurhq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfkmoay.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3vgypqqwo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ldmhlydj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3wafljdyl.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dwiuqsop.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zhdxkvzt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3isutrxxn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qofvypja.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3acueazjb.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3jhehnjac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tntqahwp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3fwseupbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwibevgo.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lujamxrv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ykkuvdqj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3gsiwhbtt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lkfynsba.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zvhrqwvp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3agippvsu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3aewrflml.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3psfzapxn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3thrgrkem.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vfmuqwyf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3atjnnyxg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dawtwudl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xkmurztt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ovzpdklw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nrneepdf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bnkrxecd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lthegiid.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3aqqdywlg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3abknsvgb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3tgvtqtqg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3gvbnvrvb.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zlwkwkis.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3lvlbbccm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mmnkfwgm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jwldwpgi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3tgnbuibe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3nfnefboc.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3ojtaaepo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yynnixqy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qteeleso.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ohyprjan.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3lynhbpsi.html


<!-- 参考信息 -->