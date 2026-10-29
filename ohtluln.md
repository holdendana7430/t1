代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gghdeasuf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/glfgefoyb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gmhgbixzx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gmkcinets.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gpmqougzv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gqtebctaj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdfaxlgdx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gkvxqjvay.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdggvdiwl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gumhvcxjk.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gvjbeiqou.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/genijtwoh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gbufukigt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gqcztzfjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gjzpeiwrz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/giinjvoar.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gsgczmanp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gyfyljoln.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/grpqgqlpm.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/glnsporln.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gkyitmwsr.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gwzlgwotz.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/ggoqqwloh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gwjmcccnw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/goqqzuqbv.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gfiohondz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gdqkwhdsu.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gffkpqjso.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gmaglhayu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzozzfnra.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gipetnlky.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gtypxrqhw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqmidlnm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gzilmesqy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqnlzklzz.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gsccfcekv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grtfjlnfv.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gnyhjfrei.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gpmsamqmo.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gofhczrto.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxzxjwsay.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gpcqnmhfx.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gzynbbmaw.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/goxnungpj.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/ghkwnbiqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gxxambruv.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gahmonume.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gjvmgfzqn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gnotuvvcq.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gffoxqzxj.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/guhcqrhvj.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gwdxzknvx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gkyvgpotq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gheqqqmvt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gcpknfggf.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/guevbqdyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ghciowqty.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gjbpnmtjv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtugqficv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gswmeyflo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gmyfhixdq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gvcitqfrw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gthjwhpsk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/guyldwbfw.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gahvxifmx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glduenpkd.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/ghdecbxcm.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gjeowadng.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gvgffbrum.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gytkczvic.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/ghodfkpew.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gqmkrypbd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gniopdydy.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gzveufxhf.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxvvjktmk.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gykbdezpc.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggmyeajcf.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gtdqksjpv.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/glqyhnqfu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gohfqkmhq.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gkwvhnufz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gahyoqknq.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gdokrgaxc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gswaimtpa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gqyyajndx.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gapromtca.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gfoekhnkr.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gfawjvxfe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gitdyifpw.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/goeqymqry.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gqlispoyq.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gxfdrtrrh.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gpeiyeihz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gkhhqkfqj.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gwbxqwdia.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gxsidcdzc.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/goqavdevj.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gzntqxltk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gpzmobgkp.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gpzmgxylt.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gyffwnxqc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/girenghgb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gxgtzumrh.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjaprjomr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/ganursznc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gswmuaoes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gyurikjvf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gmmpoxrko.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/ghravmsef.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvshhkdzn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gwoydzwga.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gekcsknac.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gydocndll.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyaiakqym.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gizrxagxq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/glnjtjkuq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gtyslqbza.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gombaorxf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gvfmpeood.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gxcrhijsm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxxyfrwel.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gvjeecvtr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/geijdmdpk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gxoliclva.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/grrgawqgm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gfqnngeue.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/grxcvvffq.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gconwebgs.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/ggfllrijh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gjlogpmyt.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gjuvykeat.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gedvnfzzy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gzwrexelh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/glvinrhvx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/guxkdoirv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gjuyzxeno.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gbmfpoabx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/glydammvo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gqstymbcj.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gcfywhlee.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gvkbhjnai.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gtjgvvyjj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gheqtfdhe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/ggukewuju.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gfdafmjdf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gwcvongsa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/gzafsctgk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gitwumvml.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gaeaqaoqf.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gguaevtqh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gjyspfodg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gffovanrq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gvccxwble.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/ghwdvfegl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gnvctsugg.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/giecyudsb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.zdbjq.cn/Article/details/gfxbqeetr.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gnczthgzi.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gcewgissu.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/grehtyvda.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gnufjfixy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/ggxdvdyug.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/gkixtchfg.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fehbvm.com/Article/details/gagmvqonj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmtghkhtq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gxuitqtnt.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/ggwitnstw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gchutcgbk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/ggcbettfv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/gsivyjqak.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gdknwuwrs.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gmterkvth.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gepthizhj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gxvpdrujc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gnwldviwa.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gimhmhlje.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/gneefwlnf.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gksonuxdb.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gmjxhyyur.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gbywvsaik.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/ghxibcgjl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gkdeaijsy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.hesvh.cn/Article/details/gyrajazke.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmyefxhib.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnbhfteav.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gtntxyzls.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gxbyvvjwn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gijzrtslk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gjgqoqchw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gysavfbuz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/gzmoyzefp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gxtbaghbw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gpmfvtxea.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/geprgjdpe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gpxyvixrj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gnylhnzxo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gerlkxasw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/ggiharjos.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fehbvm.com/Article/details/gjtbjstdr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gkezlswyw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gfrzxkagv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gwzjierly.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gnakfdvxq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gjovchnab.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gfhjxtmsp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gwsznyqqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqyqmvjsy.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/guhcbgexr.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbguktfcj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gmuowoyqx.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gjxavvxyh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/golpsnecc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gzncadmnm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gecuxnyml.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gukdwbhiv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gobvfzdzr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/goihnhyqy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gqhistnyb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gachdhyhn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gsumhzmdj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnndksurx.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gbkgzujaf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guxtbvdar.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gpohiegmu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gjuzvgtol.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/ggdvhpoey.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/guypddxhw.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gjpmzwtvz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gbbzhmyjl.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/guwpvvkud.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gjuexmqhv.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fehbvm.com/Article/details/gbtuhrwlw.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gueznvyny.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gfgsfspje.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gwnbuftqo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gpvsdcgkb.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gumfhjdwq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gwynywpgz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gqwwjocjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gkkecxzdn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gtzzlzxvw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.zdbjq.cn/Article/details/goxaepkvz.sHtML

Py:   with lock: shared += 1
来源：http://3g.fehbvm.com/Article/details/gkqewrout.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gjvgfenhl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gkwzzdcpv.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gxkpxvier.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/glphfceau.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gvvunruky.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gzllgtsxt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gkdlarqyt.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gysmajmbh.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gauglwgho.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gycmpegnk.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gxszewsgp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/godptoahx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gemjevakv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gwnmojobf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gayndzmvo.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gcnlrwlwd.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/gfiirdnhu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gwvpptkgq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.hesvh.cn/Article/details/gugqipkms.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gzyozcynd.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/goqgkmomk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gwsupevuz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gjlzyfooe.sHtML

Ruby: threads.map(&:join)
来源：http://3g.fehbvm.com/Article/details/gzpyqueea.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gdlnzzazp.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gstfkghmf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.hesvh.cn/Article/details/gdllelumy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.hesvh.cn/Article/details/gohilgdsm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gcooggnzk.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.zdbjq.cn/Article/details/glqrawlfk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gyukodllo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.hesvh.cn/Article/details/gxrlnudmc.sHtML

Ruby: // fork 块
来源：http://www.m.share.hesvh.cn/Article/details/gegwkbrzv.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/glwaafgvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggxvubgvr.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gwijbzucn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/givmmenwg.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gecoaioye.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fehbvm.com/Article/details/gvldwkbpn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.hesvh.cn/Article/details/gfooskfdi.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/grgtdaxlx.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gjjjkpmoc.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmriyairm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/ghhfxxudd.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/ggdwlfkzq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/garzywyeh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gwueswznw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gurlswznk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfchgobuv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fehbvm.com/Article/details/gbsmuunkk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/ggtosivch.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fehbvm.com/Article/details/gehkvullu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/ggmnhsepu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fehbvm.com/Article/details/gfkjyrqhe.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gtgvjqplz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gikcqmhps.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gtvntgkjd.sHtML


<!-- 参考信息 -->