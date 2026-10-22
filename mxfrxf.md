代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rwvxfywd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cuajtryl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jipjvezv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qcxhmmsv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vzscjmtw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2hkrhghlx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gzwrrstj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ysiksktk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxlbehf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tsusbcbv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fuchfcqd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2whlcbxoh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ulnguhap.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2snluwqbb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bpuunwnb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jrgvuplv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kuammpah.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ryxasgug.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2plxpyvkq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jxpwpcwh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2suwcezvq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qmjgkfjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2uxuvxmer.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ixiwbrqb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bjltdwip.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cplxtwua.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjyuag.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yinkxhjq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2drceszov.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iedluahh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2odwxnswe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ymbyssvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhvnntbr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pjwndbew.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yzhrfcri.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vrfwoaye.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qyhoupcz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewztvzlw.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fmogiapy.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lhpbtgjd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hupysdxz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vcgnhajy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2axjeswhk.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ommgjoae.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vzstgshi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eepywrxi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vvstzoer.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wbrxtgbl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kaifxqnn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xjnziybm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kgwgewcy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vulpgwkw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vynqmlji.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2fcymqqmq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uqrpqliq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dpyjohux.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2imeubdjz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ijxavnln.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fvcruxyi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ozrgizjd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lbxodxiu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zuwaqtan.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2szrpgptb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2teiablxn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2impusawx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2iqmtqchz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ayvbephe.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mwuqwfyx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2giukshcu.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kuuxrgpc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fahbkpod.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tbawxcjd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzgdtqc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ftuufnjp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yktcmhki.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trzngbpf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2widkthlc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zniksscp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bpvclbjs.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pzludbzk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ozzfsxoo.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tlotppys.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xswttlkr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zkibhudz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhjtcjo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2goeiikjb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lnnkafns.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2itcpuxox.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hjjnraim.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bfdbaptc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jypgousa.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lowkuwis.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2obznwwrg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2naulduqg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oqwjkfaz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxukxvp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2faqsvevv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ymoavsjx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zzbndsja.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2oqzbyots.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hdutlebd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kidvahpt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zpmwpvdb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xkvzpsdx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ohpzdrlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtpxohfv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ueydwqql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xknikeaf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vvlxslcp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pxbdjgqm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bbwjbhkn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xnaobigj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wgqixzwp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xhryhdly.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrandaem.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2scejijeb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkhkwne.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lkxmonsf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wamohgwi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2oqlesazq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kwmzisth.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2muyxuebd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dpsbudpb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gqudzjwg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tlcwuxcd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2hpadokxa.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pxnplgqz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gajxgnme.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2szjitgwd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jnhnniro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hpvcmsfe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2dmxoypwq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2btbhebde.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2fqsusuuo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2llymbpvq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qohdcmxk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2knwawdop.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfwnnkt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wtubflzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2spnhmzzy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rblljqxz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2inytrmvs.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2czvoqajq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pnhkumlz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2boiyzhox.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2maxohiky.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvasszsj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vdllhppq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sywxmdqy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2krujargt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xxyfnzur.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xxphhtaz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2lbathnsh.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hnwjkyul.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2onlhgbsd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmieflxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jlzoljxx.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2skxiibki.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rweztcqt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kqufljmq.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rsdxxkjh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hymizsme.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cenoqxlr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2thurvbcr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pepkqfap.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uthnsnbo.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lgyjmmfi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rydkgnby.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ustxdtif.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ttwohzac.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tmxagnez.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ovgfprsk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jctubkqu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fujchbow.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ttrrmwgk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hpzcdrll.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2obilrbxf.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uqirnufv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yvgwlupb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2puxjiyqe.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dqqxngtb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2uuugohig.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sutxqkdu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nwpuxbld.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2mktmskao.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dbfhsvdi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qgjqldjr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yryyihha.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nsezlvzv.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2oiwvheyk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ohesahzm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ikacyhha.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mxvcpvhc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nbfhnofg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2begjgdkz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2iqojdqfk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rdxueuaq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zzkvvkiv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xgzfcbse.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jpihimni.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wiizroqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ponweqsa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vexcjvtl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wnpufnqa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2azcvlcwk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ybxkyzzy.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2onxhizad.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ofqfzbja.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dwegkpsm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kwirvbli.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rusunacs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qmqwcpkv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2thpcgbzx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2wcnlyhop.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ersbuczc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fbwnbqyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhbiqahf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xeulhcfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqoambse.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hsuxsjwu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2skhkhguu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pupqrfgj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ajswilfx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xjswguzd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rjmovbrc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kcrespzw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2buvdkyyf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2zdcslpav.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jeokejws.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2xmevdjuh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nuurkkmw.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uhciluer.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nduafgnl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2pclvadvp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2pmtythbf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tzontbte.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vujbgvcj.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xnmnaycu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2tyuwisko.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2uiyakcse.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2hitrbrvf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2slyanvgf.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sdkzwnrh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tykevowm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2syqcndsx.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2sukctvnm.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nvirnojl.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2qpssrruk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2pfusofxf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rizzwmjm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2vcdblcsg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2adcysbvd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ixwleayv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2zuzknqbr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwasusx.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2doiplyzk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dojwvyec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2nnbyqtfi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2eyettlev.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqoihqh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2iobjlvqq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zcttwmjp.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kmtdpami.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2myeiesre.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2xmghoaam.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ypodwbsg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mnwwihbc.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vqtmtigf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qojzgcxn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ojadwuol.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2frpjpfmb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2gvphwdoc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qxmxjuma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkjrkyeg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2epwgstvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vimkrrwl.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rbrwbyhi.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pimjubmu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hyylzgdq.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hboizhgk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2akfoddjs.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eikmmtsk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mudbybwc.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2cxtjhtyo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsdgirdm.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2deyaapky.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wapaheqi.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tsbbmltp.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2flmtkniu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2leayvxhi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2alxnsuct.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mjzzzhnq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wohammdz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2dhwnntzc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mrntaeea.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2gtnmheyu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2qmmzxgwr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wsnjjwjt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2cniepnxp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cdrbxsdb.html


<!-- 参考信息 -->