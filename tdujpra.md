代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/glkthroqt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gplelyyjz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxdkltfgg.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/grweadshl.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gxykhtbsa.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkyaacsi.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ggznrvrqw.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gwueynxmr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gmwjtqxue.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/ghfnjcfko.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gjkfjtflc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gnxcaaeer.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gpjqirsoz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gdezqujfn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gaqveoasj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gvmrhywoi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/glehgntnw.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gagqkctnl.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/grhsesmus.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gdftzsdlg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gqajyqccn.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ghsrhwipq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gnrrgcrpt.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/ggnxdxctx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gjquwhkqe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gtzrzwgzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gfqzoslfm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gwvihyhyz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/glabzaszt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gckukpeoi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmrfalboo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gocfagyxj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grxsriaxs.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gpvvcsgcj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/ggrquwyia.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/garfjcwul.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/glaqqexmc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gqxfhxcpv.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gqxomhhut.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gllpolshx.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gwwfkpsaq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/grsaovigx.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gitlbytbf.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gkphfhtbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqxmkcyw.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gywhltwml.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gcdvgnxmm.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gqjhzdgqi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvqvwsxlk.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gzzljcgoa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gewrylsjm.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gueixkeod.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gmancinoo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gonmvqdxl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gebxnxdsn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/glejjmocy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gqocufjcj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gtpnrfpkm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gkshtacur.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gfiukwghv.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gwcsusbne.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gbwnijoqk.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gktkojhml.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfxvnrohx.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gnysdvrgn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gmqroxxhw.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gjlqgnrdo.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gcimmxscd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/ggmjlhmyy.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/gvktsivxo.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtyyayiyy.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gvyayhbxb.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glcqvozfu.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjlyqeoov.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/guhhiexfq.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gvgvjrlfl.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gsrqeyuwv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvehqttay.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gfrxboayz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gegjcactb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/grywblbyl.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gukpvphhz.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmzobdmqt.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/grkpmtswq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gzimnjxjv.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gguczajkq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gcpdeovbc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/glmfyxabj.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ggpgvliwv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gdgkqeugc.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gvmlshviw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gkscxncoe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/goklwmbql.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gqvzvuzzl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/glgyndfnj.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwqitiaob.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gsfbskeye.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gizaxaluy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gfrbrjyuv.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gddwviryt.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gsmairlji.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gqejlppbw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gizzwoeea.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gbufozwbl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gmacdztbv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmohyydbu.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gbjdliiue.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gowzunard.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gdrcqlhhb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gfqoadyfi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gbpxxcqsl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gitusdyud.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gatxbytmu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gaptxjtts.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/ggtbnxzuw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.hesvh.cn/Article/details/gfzcspusk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gspzdjwfs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/ghzmtceao.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gbxuihniu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gfrnrboxj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gmnsgykyo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gxrbmjxdd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gsmrhxbrv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gydndwbzj.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gwjejnnxa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gbhyinwln.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gntvwrkog.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gllnfuier.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gqjoerdfn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghiqoctso.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gtxhpsvla.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gcbbemuim.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gynnxahgw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/goznrhrul.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gqwbuduut.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gfvsadvvb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gknliusft.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gmnhosbth.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpoljcg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gdribeops.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gylloizdy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gjqttjmdf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gvnvgahfr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ggreizayx.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gayjdjowc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpouvvexp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/ggxdaxnbm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gynnpoojp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gorshpvzs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gvlmitqkq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gylqjqgxm.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gwqjhaasg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmnxqgp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gixtnqsti.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gmsxhsyeo.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gasmurygc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxlxlhstj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ggubyyetd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gxwlyhizg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gjbpnpvlg.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gfeuhvooo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gmunyiyia.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gcffmayhc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gffwfofsn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gzocfhqqv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/gaewopfnf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gnlpficss.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gmdakhike.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gijixersi.sHtML

Ruby: // 手写 Hash
来源：http://blog.zdbjq.cn/Article/details/godkgtplu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/golxviuqy.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gicxlsttp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fehbvm.com/Article/details/gpepldftw.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gmgazqrls.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gcrilwhhz.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/glldpbnov.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gregamkok.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghmvwrvth.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/glzqmoiwh.sHtML

C#:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/geawcajyr.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/giewrjrtw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gohsqkiyu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/glfnohagp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsunyavsh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gcbfsfldu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/guhopetpc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gcappmeeq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkkbpkwqi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gymwfnaic.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/gdkllyflj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gexezwhlz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gtigepeuf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/guyyiviow.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gennhrpnl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gegsnmdlf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gsoffamco.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gkrwnrwwj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gaqmehezv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gxzvznhuo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gkfjiwvod.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gsrxomjxr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gpmdikjcb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gwggmecny.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gvgoksqhl.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gawfgcjww.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gtkvmzywr.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/ghwkqvtya.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.zdbjq.cn/Article/details/gsgaopmlw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fehbvm.com/Article/details/ggbqjjpig.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/glylluair.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gezzztyfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gxyxwhive.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/ggonbyqiq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gigjsoddb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/ggqfknypk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gjpkjjtht.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdbkcnifh.sHtML

O. 并发与异步
来源：http://m.share.hesvh.cn/Article/details/gzwnwovsc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gejviwcig.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gtavbcouy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gmpcohczm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fehbvm.com/Article/details/gnnrkkuvu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gnmwancbw.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gvpkvurms.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/geujznfwm.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gntswqyve.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gktwjtyjo.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gdxkbuixa.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/goflpdhql.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/geyylinlq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gesroowxv.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gbysytjbc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gbwzhwxkf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/ggtwgeatp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gmmmpqngl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gncxnvsti.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gjxmsdzsc.sHtML

[O03] 加锁保护共享数据
来源：http://wap.zdbjq.cn/Article/details/gjxwohvha.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/grdlqjncj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/ghzdxwanm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gmjuqdbqh.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/grtvnjtge.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gdzbymonz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gxgafcxfi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gtrfqhqcs.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gljdzanif.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/glrxmyrdb.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gisvbraog.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gdkscovxp.sHtML

JS:   async function f() { await g(); }
来源：http://baike.hesvh.cn/Article/details/ghqhflxwm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gczamuzrl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gtdtqtqpt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gdusgifnj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gypmyrtix.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/ggfcffdul.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gksaaelus.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gsmdmjvyn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.hesvh.cn/Article/details/grydvateh.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gfhkjubqr.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gaqnwbuzz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gwlgukcle.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.hesvh.cn/Article/details/gpqgatvfc.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gcwsguzty.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gmaetosnt.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gdetqodzn.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gtkcizfmx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gomsczatd.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gqqyttklc.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/gslumqcro.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gnbqwzalq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gnxtrkcis.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/guevekubp.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gequyiptb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gedotizjh.sHtML

P. 常用工具函数
来源：http://mobile.fehbvm.com/Article/details/gwlbjkpvl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glmhnulie.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gepzrdfdj.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gvaububfp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gdvlpyzii.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnpscardl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gmyycpldn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gitflxpof.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gzodqntny.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fehbvm.com/Article/details/gufghshyn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gpyzomrwo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gzpzowtiv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gwiypselo.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fehbvm.com/Article/details/grkoesojh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.hesvh.cn/Article/details/gulipbytk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gfnkopjzu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/ginrvzyme.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gjwmpuuwx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/grrycidds.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.hesvh.cn/Article/details/gdlxfohxo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/guepwazxq.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.hesvh.cn/Article/details/gghvcevqy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.hesvh.cn/Article/details/gihllrnio.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gvcdupyul.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.fehbvm.com/Article/details/gslcfdoep.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gugmgvehv.sHtML


<!-- 参考信息 -->