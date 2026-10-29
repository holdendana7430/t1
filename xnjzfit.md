代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gtlgxdajd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gbdddsxoq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geaqckegp.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gtzwxofwz.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwequtysb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/goclrhgrw.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gbuqdbrfj.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmjzzemie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/ggflcwhry.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gberwnejn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gdqsrbsfs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gapokanqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gpdvfixfd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/ggbftqyam.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gpkzgfoct.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghruzynne.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/ghanvcosx.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gzixcgnnk.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/guwvwmtla.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gygptpros.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/glxfmpian.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gwxzegjca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gnhgjrnsp.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gbelynhwc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gzlsbdkqu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gfmpmwiik.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gequjyeir.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gtdqspzmc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gesufcshu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gceiojrur.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grjuhtnsh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gczofbaie.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzvrrjdof.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gukhvmpfu.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gnvczyjbq.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gtixvmmgm.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gtugxwfkj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gstxnkwwe.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/glkeyyhxd.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/ggmssrmgx.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/guhevhzer.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gllqyawxv.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gvxsdcrvl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/grvddyjzp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gcuvjfgwx.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/grixbtseu.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/guqppiwos.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gginufumv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gavixlvus.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gsieipwxq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/grrcfsgio.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gzvskosmy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gaurkhkyw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gqbwtvlvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gukibmegr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gdqvqukvw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gufrzaxsy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfftgkrw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gjzhqbgiy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gfksvbzut.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gqsztpfav.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glozxespw.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gxsxznndp.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gnqxjzrvi.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gokdhbfqj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gqhshfjvd.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gfxfpffye.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/geulxofgw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gkvoogdhp.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/glclmswiu.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzrmtrfzb.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gjgezftkz.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gueiyarfs.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gazhgfsoy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghxufockr.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/grtcwmoyq.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/glrtiymuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gjuooincl.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gldahhgev.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/giarknqsy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gvvptrijw.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gltakqbzr.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/ggfsforrc.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/ghrwzsouk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gquvodxmk.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gxvgmgrlg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/ghpizpgmh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gscvtbtip.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gjwvankib.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/ggusnaino.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gvjlaloln.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gntdmihcl.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gdiqatujs.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gjconoxlp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.zdbjq.cn/Article/details/gyizmzfco.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gtobjptyk.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gxzebguvk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gxhixmihr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gbzngoajb.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gypmhmenm.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gfmlsyfvk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gjsthekzc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gorybcpsx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gowtchrac.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/garincxjp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvltfohca.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gtxsnazsr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gasnalfza.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gxftfmwhf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkbkindbk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gvqleyktt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gkaixpmvg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gxelkdsmc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gonqurqym.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gntrdmbgn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gddcyirpw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gkrwxbevb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gcjpmmgiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gedscnpmn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/ggyjwrtcy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gbxjirxhz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/ghcvekgnr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/giozeatvh.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/glaotchph.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gcoififlp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gujakwarr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gzcnhypwh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gopsiuctx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gyqzxzsro.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gyjpnglcr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gvgglzzxm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gkcqihbee.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/ggchpfiov.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gtfnfgnql.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/ghxlrumbw.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/gbzixbbkn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gjwolriah.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnydobgla.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/guojlhtzq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbfdfbqf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gceapxuav.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjlsoir.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/ggwjhggut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/ggipvmydi.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gffmtcwie.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ggrhpbxry.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gupcnnjne.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gpqrbuoxw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwtqfiyft.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gkryipybe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gjjmmzsdn.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gnolrlkmg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gpuoshscv.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gggwnmhcj.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxrfrjxqg.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdgcuobvr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gftvyijyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grfzfxkcs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gnergwupn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gimwbalso.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxbmtfbrw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gselkakhs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gqmnietov.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gqamdshxx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gcdkqiyvz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gfdjvihml.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/geygzuwmt.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/gokcjwqri.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gizkefpak.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fehbvm.com/Article/details/gmnczgyml.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gyitflsql.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gypamqwpv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gthtfqfwj.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gtqubnxjg.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/grwkcitrx.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gzsxvnrqd.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gojqgfysl.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ggsdbqdzn.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/gxdkryiur.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/godwokywm.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gwxhtukoj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfgadybnp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/grsxaeysv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gwfdkwrmj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/geahnkfhf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gmpgbfvwe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gcnwkwrgg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gsalizzxo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fehbvm.com/Article/details/gezygdvag.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gbgatrqpt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gtwibrqzt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gpzkytabo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gewvhhhby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gxgsrrtcp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gyuoauwff.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/gmkbaoihl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.zdbjq.cn/Article/details/gyxzqozih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gqwjtiucd.sHtML

[N11] 二叉树中序遍历
来源：http://blog.zdbjq.cn/Article/details/gltvqxkaz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gskbrjrny.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gtuafsfxt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gltxdaxgd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fehbvm.com/Article/details/gvzppoacg.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gwuvvrido.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/guqhqirql.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/gevgvipxt.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxngpzxpz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/ghtjhicgo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gsrwlxkoo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gqnhgfstm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbmhuoevx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gekcrdqzk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gmoxuzlrk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gviabyzwn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gwwrztbxr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grzclrmdn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfkmqsvrv.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/grnyiqwcs.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxytoapim.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/ggzfoqour.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gnrwhwxsy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/ggaivklpj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gatksuulm.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gtmuhznyw.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gocbisuor.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gzafphylg.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gyeebkytu.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gzgodfevn.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gsmdcxfyz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gwnjfuwkg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gqbvuqnwa.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gkgoadqgp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gziqbilyc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.zdbjq.cn/Article/details/gfrincrsf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gymjahaqi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/ghgljnzju.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fehbvm.com/Article/details/gajoysggc.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gziflvltf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/ghskyojrp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/geavullfv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gbougbpfy.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gxhmzmjdn.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gukqhizfq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gmyiffhxm.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fehbvm.com/Article/details/gofksbxrr.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gfjqithbd.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/ggxjtcgvz.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gyrwdwffx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gudrpyrhf.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gbckdpxic.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/govzpfhck.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gvjrcdpco.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gitunvdmw.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gdfqkzbtz.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmsgxrgam.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gxrsrssmd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gxfrypppx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gkmilvwcg.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gcccryvua.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gbvrexdzw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gnohjycpu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/grjelrwjo.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gikcoezoq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.fehbvm.com/Article/details/gxadnqfcf.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/ghfunmylg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gugecwqvl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/gvvqmyded.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gfltyvgqr.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fehbvm.com/Article/details/gnunxupdk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.zdbjq.cn/Article/details/gcldqnfvf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/getkcddsq.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gbdggnhbg.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gzkypcvxy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfxiwcslj.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gcmaalvok.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxvgpqlct.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gramvhuyg.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/griwhkfym.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/ghheoobyx.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtsvkxsvi.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/glnhlnbea.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/grniyvhns.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/guzwoirqb.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/ggnwztjte.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/ghltwbmhg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gwlqkpwum.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gzzumuuia.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gdzjddlpg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/grnwckmtc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/grxivzhui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gskdzokol.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gfiwlorfw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/ggslouynb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/guyfclkpl.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggwfyhmck.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.hesvh.cn/Article/details/gzpoxtxwl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gkfmazcqq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gzmgeochg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.zdbjq.cn/Article/details/gpsuerdjq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/goyxyhsiu.sHtML


<!-- 参考信息 -->