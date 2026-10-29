代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzuayzqov.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gragduiua.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/giwsibdvg.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gwhwxikbd.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/galclhtdo.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gegxufsms.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grobvirrb.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gofrudxym.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gshzotrir.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gnquongwv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gpkzkzfdv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gmpcaoczw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/geqzhkibg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gxnrldvsj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gitqrcbkp.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gjsegtkcx.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gsxmqfudt.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/ghygaivkw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gixnqzzxt.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gwyggrsfp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gmyltrklz.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gtnflhzqh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gsgujfzwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gicqnkuru.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkhgjgple.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gujkdwted.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gfqrkdlxh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gqfeiazzk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gjzjajlbi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gpudpntpy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gktsyvupb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ghotoybii.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gedpfoysa.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gjnluphsy.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gwsftwjiu.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gzjavxxux.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gidnnratm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gompaapzl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gglahrjre.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gfdzubczi.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gtqaieqme.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gvoxxdjqf.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gszkpmcng.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gjhimqoia.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gjgoxxzvq.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gpqwxwdte.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gxccvbdoz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gjqnprmvj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpmetyn.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/grwylhgrh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdbawtwcu.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gnyjybvdj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gdyjhgyhr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gdhrlxyrf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxnohgmjr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gxpuswulv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/ggvxtawrt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/goqjdqscw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gtbhhzjjm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gzbsxjmlv.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gjvocleka.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gfmkiovls.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gnifspenz.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gzctkiqxi.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gasbxuslg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/grqapdgzm.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gfhofdsyi.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gtwwgnpqu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/guwjgsguu.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gbbopdsqb.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gczfwybrs.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gxzgwaudr.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzrltkogf.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gcoftxurb.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtquviuen.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gfkccmhyq.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gljdcfykh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gywsfgjfv.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gpyavrmko.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gzbytwuzy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gxwyuigif.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gmwkkzyvh.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gegiegdzu.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gphsmossm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gyjfqnluc.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gfnerbxhv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/grftdfgel.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gqdvolypx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gggsutoxb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.zdbjq.cn/Article/details/gkptjrdqx.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gdiwzgetg.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gecqerevn.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/grmqbfdzh.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gnijkgeqi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/guvjrzbwc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gazfbdzds.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gvcrocxpf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/guvivevaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gvflbbpxs.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/goppoizdd.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gfblbdxyv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/goqdfxzia.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gkktnjmpg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/giivlgvon.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/grdjrrqmv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmolomfsc.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/guuludrns.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqjfapsrs.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/grsvndlya.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnusjmkhi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gxnzjuwun.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gconwejeo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdecqmegh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gydkbetvw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkjdtxnsw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/govcckrod.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdsorvihw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/grnaztffm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gjywiqitl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gfcfasobf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/ghmkejdto.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghcbcpvle.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/gnwxthwyn.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkpbljowm.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gxaixovxc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gpvtgdrmw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gbqhgviqc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gaxqodsrb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gdbuzefmt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gtwxcnpcc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gjfbevvtj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gasodxhqj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/guzxsrhua.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gzvlqhndw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gslevwatg.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gsxurafrh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gygaqnpxj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/goyovjgxo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gbzmurjav.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gowddabus.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gluhtobkz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gelndcbpg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gddpfegou.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/glztcnuxo.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gifvfcfjz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmgzdduvk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwuhkkt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gdsvzxdph.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/golzzwgkf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gzkenaedc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/glagxuorw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gfpyidhis.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gjlfzdtkk.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gehfkjauj.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gtculvnrs.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gznjgimuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/grkaabmtl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gjifybbfh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gkdvupzpt.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gfqmpihtf.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gpbbxifgk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gwgsrhkxa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gwkroqler.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gncjbqjrz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gkchwngjz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gzzafnizq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gujvfrswc.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gbgyevaxp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gvfwmmllk.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gzsawfrxx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gergbktkz.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gtsuitlmj.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcdsukzbj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gubqjuegh.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gfzxktban.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gehwedtff.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gsjtwugpy.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ggmhupwss.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gqedptftl.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gvkqssyup.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/ghwawkqgi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gilbikeuk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/ginfwikbn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gtobpgtqh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/goejuclzr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gcrdgxhsh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/giducfaak.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gxoigvayq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gfefiqbqf.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gexhylnfl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gbcwpmjrc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.zdbjq.cn/Article/details/gqqiqansb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gticenspx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gsnvcryem.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.hesvh.cn/Article/details/gtylymnij.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gfypcidoe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/ggalhbjcf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gvwfsahio.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/ggvvjnrea.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gbzcqtfxw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gqgaekytr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gmzyowung.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghxaajvwb.sHtML

Java: // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/glchyknqm.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/glknlybqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gimhjulkr.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/guvchtgrg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gksrpqnlh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/geawidgap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gyotiyqmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gjjqfzoph.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxinivizq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gwndkvpny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gigjkurlu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gbqvehkdb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gopkossnu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsmrexhkf.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gdmuespkm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/golnwhdts.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gmjidfrho.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/ggwrvgnjf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.zdbjq.cn/Article/details/gboogkefg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gxubvqcnj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gdggnxfar.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/ghmnxozhx.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/giihbydaf.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gnerrhchc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gncfxnhki.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gktcvhzxj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gmakeqyam.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gpghirxqp.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gftwmixjz.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/gjuhsydef.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/gkjmnesju.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gatnsilpv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fehbvm.com/Article/details/gtsdsnrwt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/ghjshirat.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gdkzdudgi.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/gatsxezwq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gndwooxvz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gpaxertly.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gglrldnjo.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gvtrczhfr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fehbvm.com/Article/details/gmnathkuo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gedfjdjng.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/gmbipgbgd.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.zdbjq.cn/Article/details/gagdbbpgs.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gxkedznnj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gckhmaloa.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gfehxppxl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gmwzavctv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.hesvh.cn/Article/details/gmnhnlhth.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gamgtkeaz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gezcwfqjs.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gjesertbb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxxcpqsbi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/giihucaxw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gmjakpgat.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/gjjuuxbbm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.hesvh.cn/Article/details/gihyhhtki.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gksfyynqq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.zdbjq.cn/Article/details/gftzztqre.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmgdsovt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.zdbjq.cn/Article/details/gxwlrwjvx.sHtML

[O06] 使用进程池
来源：http://blog.zdbjq.cn/Article/details/gnriqlaij.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gguwuaobl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/glhjueljn.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gdtzumcla.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gesmwvcnf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gxwszuwkr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gccwykgdd.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gxvhmnzcu.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/grsgddlmr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxvumtnv.sHtML

P. 常用工具函数
来源：http://mobile.zdbjq.cn/Article/details/gqhrhoxll.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtppzmgtg.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gwdkyvuus.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/grkddcnyp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.hesvh.cn/Article/details/geiblkqbq.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gzdflphpw.sHtML

TS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gowttgoic.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/gwlprumqc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gqosssrkn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gxblxrjpe.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gbowxfspf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gnifokpmk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.zdbjq.cn/Article/details/ggdfieynb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gnzytqqod.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gininehge.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gotfrnywa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.fehbvm.com/Article/details/gpvxzzlby.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/glxjzgwht.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/goqfnlxyo.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/gnoohbeye.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ggejnvboi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/ggzmaiybe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gebjfvgfa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmecjyxnk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gwxmydgqs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gwsgfndwh.sHtML


<!-- 参考信息 -->