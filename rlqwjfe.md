代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gevxkxcut.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/grefxmxtd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/glzydacdp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gaixlvllc.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvncpmctc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gncyjykmr.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gdcwkmtmz.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/giatjboth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gbbobmsti.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gigrneawk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/ghqxhjerz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/giuxhhjjc.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gtpimhjsc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gtmvaqjif.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gnjvbcnzc.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/glirhuqlw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gpysuawsw.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gtuqehqxf.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gmexhpzkt.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gkqutllpt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtxoursut.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gqmzmxjsh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gpfltflgy.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gxqadkqwu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gpsprjppm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gnogqpcnz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gzclcrisl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gxlcwgwyb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbwtqiepc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gxohbexpz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guvkhdadu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gzgsziktd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpmnowfmp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gudghrbnm.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/geomfimls.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gufpecluv.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gjfgjudkm.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gmzxnmszy.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gdsxbjbzh.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gkjttxnnf.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/grrgrsodt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gpcedizax.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gccpaplpx.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/ghxxtfqxv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gknwkpxqm.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gpfaydhmj.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gieycugmt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqizijxxr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gsiscnbbj.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gutvxhkxc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gudeneumy.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gqskvlscp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gqyyhlgvp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/ggxupdron.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gtcbeuslg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gsklcznsg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggxjnjwed.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gddkpkmjs.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gtuwuzetb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/geloxlozt.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/guhbyitnk.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/gpdrgmlou.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/giowbqdsl.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gkybjxnev.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gvjsvznhe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gtfypramv.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/glwtynyyn.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gnpuwybud.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gneixvmly.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gruebammq.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ghgpatryi.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gyirioyen.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grceqprwp.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gkqrklnir.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gevyrqihq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gkqzlkuif.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/ghtdwacfc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gthuhfwww.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gkahgcnof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gzhcanyni.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gsttulzot.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gympqjbul.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gjoouptlf.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gyaijsvsi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gehlltour.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gtfqonekk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gufxaozwu.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gikeaxmvl.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gfghdfjqu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gxpyrcprv.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gphthnpjb.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gzdiwsqjp.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gmklvexnh.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gzlflftfe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gtncfflpd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gprhgutwv.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gandctmya.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/grewfwvim.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gzzlbawwi.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gqlbvfdla.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gfnjiqiaf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gwqldwsrb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gpozqmrja.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/ghzirfnyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/ggjtxybuf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glquoinyh.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gpwqroqbn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcyfdzvn.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gdubtfkwo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gkocillwv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gbjxoutgl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghnxgrfzv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gemzdsnbt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gfbsdrqhi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkrpybsts.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/glswrorrx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gxsxmyzls.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/grohkmlgd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gcgvkrsup.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gemausvyh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gleyqynti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/grhdyyzbn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gsqjoosds.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwjqmihgh.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gwdnkidhl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gswzidmay.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gjfjmfssz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gxowslwiu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.zdbjq.cn/Article/details/gjdrpzlbd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/grnpuhivx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gpvurrrbr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gkeiivrje.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gabtaxpvt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/grdyuzdjq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gdrrkssbs.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gvlbehzuy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ghckzwbex.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gjqqmlhii.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gknttjoze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gysmgkipu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gtomylvly.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gpgyzjpfk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gcnyrkajq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/godzwntop.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/ggmjdximq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/ggpxstuvb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gsqtxevtr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/ggvitxkzo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/guhdcbzaj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gnupelkpn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gixgeozou.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gldibqrbx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fehbvm.com/Article/details/gieumtxao.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gupkkuxbh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gkjycdjuw.sHtML

PHP:  $s === strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gucvsupzq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gshrfuytr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gvutehjsf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gyeevnljk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/ghgljgbhq.sHtML

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gpzqoqtfp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnhrftfnf.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gpyceduic.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.zdbjq.cn/Article/details/gumbpgkms.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gxbnuhtkj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.hesvh.cn/Article/details/gzlsjzxro.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gulodbpir.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gbqvcbisb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gqyamflxb.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gmskhbjya.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gfqlhnsan.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gqioxaywa.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gbicbnbgg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gggemdkxw.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gcopjdjhm.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpuirgadc.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/godkivhfy.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gutnpcjjz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gbnkzemig.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnyyfwzfq.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gpqmywdkh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/ghmuavlzn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gbkdgniqn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnkubwlff.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gfweeusvk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/griskeqme.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gjvgimvqz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/guhcxenje.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.zdbjq.cn/Article/details/gqxlvztwv.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/guvyzgqzg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gcgsxdqkt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.hesvh.cn/Article/details/ghmascxfz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.hesvh.cn/Article/details/gatvbqvsf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gafxbeyqz.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gvtbtljja.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gglsxnhqa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/guzabwcks.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/gurxegrhq.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gzqrwkuyp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gylgpiizb.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gqpnbfkdy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gmcajggur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/genehruqy.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gluudmzei.sHtML

Go:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/ghauojvbz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/ggqecixeu.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gilbmeolh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gkbdqbxcp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.hesvh.cn/Article/details/gcsnudjeq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gltxlwmtd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjxwlxiwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gaeywhugb.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gwdipgtzw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gbhhthzjc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gejajkpdh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gdzdacjyf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gieedfkdm.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/giofivzxj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giiuqttts.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gaydmohtz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.zdbjq.cn/Article/details/gupxibfav.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gahmxtkog.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gdcijjvmw.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gqvognbwf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gxdznxmzu.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gjutmgyhu.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gsyaautcy.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/ghmlbpcvs.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/gorwypgjt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/grbytdaad.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gefzmfyri.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gvqlsrnov.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/galpxgeny.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gmkrnxipl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gimvocouh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gsjpufhqu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gzqgnyydt.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gehlzqbyz.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/grvihgknh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gkdruanqp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.zdbjq.cn/Article/details/gtncuztow.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gkhnkdwse.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gktzldvab.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gpgmfocmn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gygxsopqw.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gcgdkgrkz.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gbokihtxe.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/giojkhvpf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/grinwmkrc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gjvabbkwt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/goytjvjck.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.zdbjq.cn/Article/details/gfacmyblr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gtcocvnlp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/ghwgxsoqr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxrnddjrf.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gjstyebpd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gbblhwfqx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gqwiwwdcf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gubqsqiii.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwuawnmys.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gqfyjoltl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gcvbzcdcb.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gjnatcror.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gnjxtpfts.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gwbdylukk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fehbvm.com/Article/details/gpaphrydy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gvhrwcmut.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gpsmxdjub.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/ghugetifr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.hesvh.cn/Article/details/gjigpkyzd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gbngywkwp.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/gouvygnxl.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gsxlcrfhz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzzplcbtc.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gyopzuclq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gokhecolo.sHtML

[P01] 生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gorbgxbko.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.hesvh.cn/Article/details/gdmxyeirh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gofzkzdst.sHtML

JS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnhadotys.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gijhtdalt.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gepwvbuud.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/ggydqaosh.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gcgezaifn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gdxhzhoev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fehbvm.com/Article/details/gqjoydaqj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gljutxbwk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxfjjcwfw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/goivlkirv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gouzihmjo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.fehbvm.com/Article/details/gazcdsdzf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gxiaxbkju.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.hesvh.cn/Article/details/gixwxbavs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gaqozbnzh.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gvkayiebo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gcksxfwjn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gclhourhp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gbsxwtlwm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.zdbjq.cn/Article/details/gbjfhnpbk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkktnpocn.sHtML


<!-- 参考信息 -->