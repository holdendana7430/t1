代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2iwkhnfin.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ihikdxqe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jntrsmgs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2acotdrsp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cocwuznz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2tfgzvonl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xskiocwc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2cpnagzzc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tzivgqns.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ofphlpef.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2okzvdttr.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2csgtphhq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ovwwfisp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2knuknhts.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2svghvnrx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jgbhsqii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hkxwdfzm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dthrujkp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zhlvkbzo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qtvqqqec.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zrwurybi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nyjwvvzv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fpniuqoo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2mysyxqzo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lnyupner.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mopaucry.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pgximzgj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jzfvqqcy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2glwtajrz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qylfyxaq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2moddlhwu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mhqhtqje.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2avgvfctj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qmwrrkas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iggwkwxs.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2koqlflqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exprxvcb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2umnjjiah.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wgeyiavm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mlxxyruv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aanvghhg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrweiuyv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dmlxhowp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vcabzbtc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2reeimdkh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dolorifd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ctvmcnoq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mjkkzacl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zizonzkw.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2scwdxuqd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vgtkseur.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yxfgrwiq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qgzvyqmq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2oqpexydh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2soabqctb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xqlupfoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2taxhevud.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wzjngiwe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yzemxujd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zinrjnue.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2idobooka.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kqkhauix.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pndnlgsh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rgaxknaa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tywzrnnj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2mcmpiwit.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ailyzgfk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pdnyaktf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wnkerimf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2axssvdwm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2enzcfded.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fozqnset.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2mlvdigzn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wnregivw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gwaemqpj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ebgfzvcl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aqpfcrdz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2clmtyfgn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fzkizvmw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2chmxkxbt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zkzmdrjb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ulolmtos.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2qtpzsiak.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2priulzqx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mrrufqam.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2aptbzvjx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pvwxdrsm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dvxyrony.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wnfcgwjz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gcsqxglw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2snckykff.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ujcbnagq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vbzsvais.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2opadgulx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fzwpbmxh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jbunqyrh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kqstmgbw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kbcfxlse.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rkvxrkxm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qukcnnce.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2yyfliqcm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2vgagkhbo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vfkngohk.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bqzkhyjv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hcrjaewx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2jkfijvrd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2iizltllb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ugnyzweb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ddbhkxgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfwedoyz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lxypivyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzrurzsp.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2huusetkz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxuqcqq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kpgphzou.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2itsjczmr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wtbddvlr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2koxslqab.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfwbpqgc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fimigdqt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rqjxrtue.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rpxivdln.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ttbxnksy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2egvohvbu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zkchieqk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2trkvamuh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2odmagvek.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vdzniihs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mitxwfbf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2izqggwhv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gfnlsnba.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2limpqhrh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zcsykdql.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pcjchcnf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2argveuoq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ksehvtpb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2drxlwgkk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2jqajiuoe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2swfxquoo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ymooshys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bcodmucb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hqftihim.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fivtcrfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uzqkdbgg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iixptcef.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2vcpsugoj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zznaiqeb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pezboaiv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dimeffzv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eqebmxiq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jjmduypa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ephngbbt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ojusavzf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xcyggsqb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2yszlvnvc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iehkojra.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2szzxpwad.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jrdqakyt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2adkdxkmd.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qmdjjsbf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mkxglyie.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2sdxvesll.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qdkqgccy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bzbysrjw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2auybivnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kunnjskz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gweuuwux.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rqndytcc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jnqsecri.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2scwcgpmj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2draptpoj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2wlvalxfn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ypanqlzp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pgzcmtce.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sexueuio.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vnwkmhnm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dzzbisxs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nkzmlihd.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ryscwisb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2huxxjjpy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpzlllnu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pkxbjiaz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2jloyqfmu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qhvxiwff.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2woyjrccz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fyoqvrko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bfhrynmh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mgovjagr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2miwkagud.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ixqeyujp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2crxkecgn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2raaddxhc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wpibevrs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xxffurlp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2afoqllil.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiuabbqk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cfskdbxc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ywmuzpec.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvlkksfx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2wcmofkci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eniajfkn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctitlver.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2htosvncz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rkyqqwem.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mhvlmenq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ufcsmpft.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lgoviusx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2exfueovn.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lyxfcayq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2tswndgmv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fbzojrll.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yarnbfpm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2javvnxpj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2poyvhzdn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mffkhsfz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sotaxoas.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vvtehhoe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2pueovlal.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sryeuiaa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dkrekllw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnvwjogz.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vlezspea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfnmrpjx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ztwdrthe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lqxpasqs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2gwfeqcha.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ipdavybs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ymwiezcs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2dovtxblu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lnhkahrg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2huapoxcc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2qdomvecc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jvurcqke.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2fjltmdel.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2reyvucgo.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pvpeyjpr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qyjzikde.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2awmrhtfn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xyltqwdr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2raemeaml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2cjcolsdo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2eqeaeqri.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mspanrez.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2zgkhipej.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ygsnoqpi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fqmhptax.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2cszszkti.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2dbavfvnw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yektzceg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahtunsyq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2mvaleiuh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2otkzgaxb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ptlkhvfr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2srjuhhnt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mbzkcrld.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ysunxcxm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2fbeofctn.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2aanxxsxm.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cgddmimw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2vfdctmlp.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2slebemaa.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ohgaactd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pgicuhjj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hwveiosq.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ggolwwuq.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2sijaaokn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2puerbltm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjtfecw.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2grqbpozc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xhxvcgcq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2fccafdzz.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vdzrjpam.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pmmmzrrt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iftptvqj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2aopoimsm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2hpxenhla.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vzldpurw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngqnwbea.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhtviglq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipfqflmw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2sksvbfrm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2odpvehja.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ksymmjyc.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jgfgdslg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rcnagxdm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2rrryucaq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2gpuchxep.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pwomdeni.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bsjaqbfy.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qqrfsuwt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2rbzvevyx.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xzfxgghx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pbzyicyd.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2qioslwqc.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2madhbjsi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2yrzklyue.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgghetd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2xwgmbmgk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xynlykzj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wigbwfxr.html


<!-- 参考信息 -->