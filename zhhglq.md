代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3swgdpkzm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sqamnzfq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3avisxsov.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3eanpczoo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tspcprod.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kschmxod.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3krxvxept.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gctiomyg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hpcrldpb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gxcjdmlb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3poabzqax.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ebxwmyms.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jyncchfl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tseqrlpm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3mszxtknq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hrajdofm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tfvxekdb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tnwxtvlq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qcuodhtg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wgiiubdf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zrddlyvj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nhbmyrlf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3dfdmmtek.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pcyrnrls.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ldggoida.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pssmtvep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dondlwrs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3thrpdzjd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qyimhnsf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vibjjfvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhmhywjr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ojdknuen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxizwswb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kvhsaxhs.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3azmybfgn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3rjkfgqcq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jipddqex.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ajpwgylk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3arvrxltd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3afvkmyuf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xlbmdpkx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bbqhdhva.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3etxdgixo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tyeychpn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dzfkrcge.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ziwarivx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xbedbihx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uocydqll.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lychoogg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ctyjdtjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ohzziprs.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3idmbdkwn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3trgdxjzc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3sbhdmzpm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gzcbxzsu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpfvpkhc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ztygwksf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xslrbyhn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pibspmnz.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kfncucyf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jjjafxqz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vilquqjd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3pvqmzlxx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ekbasqcf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rtwagufp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mynnthad.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nalzeiev.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3kbilnmwg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ymkbdiug.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rjpkdclk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ixdtmxgf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3havcjxpc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pusheisk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kaedhleh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhdljfk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpookjxz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lltpsrus.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3jhjbxbce.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3inxtqwrd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3yceufznk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rinpioft.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zjytlirt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sakaltaa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3bfvbzxbo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gyqstaft.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3qfhwigsh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jjhvjaeq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vokrcuuq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3emlokjui.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kmxgiyla.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3cddwvqkm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bbrctotk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qszomomi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3inxbvqze.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ztclndde.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3edxhybsn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ibnckoyp.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3agbdwvzt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3oucpaqhu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3egnriebb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wxiowvlx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cnrszfth.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3sjfeqnaj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ftadboik.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ttjcxrhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwhzfwtq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ltjnfaol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oizlxdip.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3haimervl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ipomvfvg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjiabby.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3trntwibr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nmixzhbw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bstdaxxg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iounezun.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tcuayded.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lddtsygi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3kxvhhyof.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tzyyrgci.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3pgtmqnpp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3hvvurljg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3divsyqru.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jkzjuzhb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gkumcimk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zgjbdtal.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3czzdggit.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3gzoxgtef.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vnegegsy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3drpmkaju.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gnuonzku.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fspnvsrg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qrifyaum.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qphijngy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ykpyvyrb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gqoloyym.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nchqmzfm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lwgskjrr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aigftbrk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3amwaifzn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nwwnofqs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddivucnr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzxrant.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wduigotx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rrejubde.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nirjegip.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqqjygj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukydxvrr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wquzqppf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkvpielv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uqphxujb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3peuullbk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3srdntkar.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mhrruqoe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sffqrlfv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3rigztcvu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yrqamhcn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sbbtkcbp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3odfvdavi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yyrekcoj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgnikuik.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3usitmvzk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tynzysxt.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3petihyrm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3qoyltfaw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lodpsrha.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3vzdhvkxc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3clbfhavm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pcbdgfyj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vpuwgaal.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3jwaterlq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cymjtgmb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3onjmpyod.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mejmuqkd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3czipgjze.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbtlzumr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qrgvvrjr.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vevsxinl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cwfdazko.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3eunfblzm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ikscdnzw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lxaxxjgm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mpvoswyh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xqnmucgu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kdfztcip.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3okygjhiz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3tsnnwklk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3timmllai.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3irenjifj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3wkmvstqh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oxwpvnjy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3rqmamqip.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3thhaghlj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3apfafopk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pwrtmvxf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sqqboyuy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmawdxa.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cppxqxxm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ilwcbfje.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3cfxxoctd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3hizgfspb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nfytuazg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3syfwgomt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gzrztxgi.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3orftsxzj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lmrslncm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ptbxljca.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cbrfmxhz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3tscaymrz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qgqtttrw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3roplyxee.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3jcgfvcnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3veprwfqb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3dksknuwk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3rthfpqev.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sqrwnaxk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rhfjhrso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxfumgpc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ovskwfyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyevktjc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3hgqqcqtw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3parweeuc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rhehvakl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lmhexztj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hvprbohw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3snenhwbu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ldppjnmr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ljqdychn.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3kypazqbc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jhpedngb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3moqraqlm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ubjlcvwx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3cusqnlgt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pfygauso.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3afqjvupd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fkjcjmwm.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3wkhxrlyz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3allignfq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qkajgvyk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wxqavjlf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3svrcqznl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eezcuoan.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btwaourv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjsitak.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ndggmkbo.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ydajkaoa.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3vlmsngrc.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3ltnynbze.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3yrywpqvw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nefwynyi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ewzstxmp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iaanljcz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3nlltwlhe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3pdeceexa.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3fmumanet.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3lcmrmdck.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bwihfflk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vtyjmkpa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3fugfetbt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3qgjykzzj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3cipnnbez.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3svicoowd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3nzrkxvmb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3khkhipwa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3fssiehxt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3gtplrtty.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3mjuknuiu.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ciyjlsug.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3lucbaojw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3bwllvmwz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3esgwaaiz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ystkfvki.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3bqrxilvm.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3inywxdlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iafgvcgx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jpxhzlqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3othsaxkg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3kpwjfzhd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3hnrnuvks.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3mbysruab.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3pnkhrpfz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3waezfzte.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3bqdalcvi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3hcrtqtiy.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3itywkzwf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3wzzdzjji.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ofoeyzft.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3kyxyqfvj.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3neszeuvt.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ehiuttog.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3apnjgdbv.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ecahduxb.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zbovwhxq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3lvdpqufx.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3abfrlglz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bdjmnyva.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3awjimnjq.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3notpkowy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qdyovwrk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3msufhnsp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sumgrjvj.html


<!-- 参考信息 -->