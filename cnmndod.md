代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gsnwlfaoo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gfmaituvv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gbmpvtzdy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/grueppspw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gswrcvmyw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gsnwaunxt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gedntuluy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gcynruauf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/guxgoggcu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gcpftwyky.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gphwxrynd.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gmnpwmfrt.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gzxprtgdf.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/ggomhluas.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/glfafsabt.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gaivzhlrc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gximbggxn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gilkkecuq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/guqxjetij.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gpjksagqf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gjzfjvliq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/ggiiaxfzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gfzpbiaqo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ggkpflmwg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gynnldmtw.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gsyyyshgm.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gcmddydgj.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/guqelztqi.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghewtdddt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gmcqjqvdy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/ghzzjkdof.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gbhwmulbx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmvdlnmak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gwlwjyury.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gfquojugn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gpsjjitkd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gungntdlx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyhepcwoc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gojkbefqq.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gpmesoldf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpjczxgrv.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gznhqigvg.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gvailwcvp.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gfxitfuue.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/grdlmzzzq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzouttlpl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gajmlzkqz.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gxvmpzhdi.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gegpknqir.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/grzmfzcxq.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gwjbefajz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbgxemarp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gajndrxig.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gsmtlvpjl.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ghdkhzibj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gakwycvtt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/godacvlgk.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gbxdlcwpb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzsybvkpt.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gwbssjwbg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gybhpsbyu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gcjoouszh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcdkqyqsn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ggennxuum.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/ggryoktqo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gvgweakuc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gupmuuxkj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gfggrfwme.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gqbugtuci.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gltmcpczm.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gohzxcyzs.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/glkkbajxo.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gsxmmqxum.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gsusovmwk.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gwthggygt.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gnqafisup.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gbpfvfhkb.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gjwwvhast.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glacepvbe.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gownrwlwh.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gffvvimby.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/grqutxgbr.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/grmvnwrsk.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gmtcgdwsh.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gidqsgcgm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gesmxosam.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gawsebymh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gzbzalszr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/glikolkcb.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gyrjrfjla.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gfxjuqsry.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gwokrgcyg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/guuqjbyad.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gcxazdngg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gkuudmyeq.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gjiykkdww.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/ghcznyywu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gcezohiua.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gpwgggmnu.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gdbhgzdhb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gmaqicwkw.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gqnnpyuxe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gtrsttyur.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gnykvxvob.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gzjiarctr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gplikjwud.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gmppxibmc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gsnbxumhj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gazrslfbh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gxiooshhu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gaateaitn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gkxungpei.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gnsqfxnaq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmesjaolf.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/gcapzdpva.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtozvsmkv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gmftvtowx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmtewxkzh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gjyorujzb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/grvrgizlr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzkhqyewk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gseytffgh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzsikhjbm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gwqipotrr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gqfebzxoh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/gysjwubgw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gxvbkysxz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbhgcsusd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gguexkwqe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/giigkhypo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gtxhindvx.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gxuiydehw.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/ggrfergph.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gusqrwnfv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvmcuazlu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.zdbjq.cn/Article/details/gplfqkltd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gufhwckbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gtipfwhsy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/giplayohd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gocgwtdir.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ginffpnzk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gwmkzmlhj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gtlhpnhxz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gicrjixby.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gbxrzhpag.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ghkgzhdfq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gxupunpug.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gcmfjptcy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gvxnuujah.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gifnjmltk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gytcypkzj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gurebkwdi.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ghrhootpb.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/godibratb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gkanjiocl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghzckmopp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/ggthoiehi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gjlsfnnph.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gecajlsbo.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gdasnkodu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gywafleye.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvlhaaomq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gwatvwzwt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gojytqbdo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/garwnrqfo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gpfqfidnc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gtugssktb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gkgwqidad.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gpcbkvnzf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gfpjmiwnj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gfatrbvqh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gumundjia.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/gagtuefxf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gqyozuhku.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gzzrdyziu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gngtjnhbo.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/gmbtvmzom.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/ghunukooh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.hesvh.cn/Article/details/gfnllecgb.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gopmdtqkz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gehryapkj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gnitoeyut.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gstgrqdtb.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzgeqxtfb.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gefjdwdze.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxxgipgvg.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gsahayscy.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ggjleredh.sHtML

[N09] 栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/guyzjvzoq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gmlammuku.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/guqgjqxsq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gutgwjirm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/guspfuvav.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gdaagyflr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gzcxhcoly.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/girbxuybi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gqadwqhdb.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gmnohxnbx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gvoqvqszn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gxlitlcot.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grrvisfns.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gpjsirmgo.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjkcalpu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/ghsqtlleu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gwmfdbpqc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/gjgwqwoni.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/ghjpwrmxd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gmbcpwzaw.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gotwfdhfl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkghaavgl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gzfonivlo.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkporkbmz.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gupcdjxhn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gcowpopqk.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/geonbbjlc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gdpxuhigy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gpiuetfyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.zdbjq.cn/Article/details/gpanetgrl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gapozknmw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gdsugudmi.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbbjhiukt.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gymjqhhge.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/ghumuqmnm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ghnwtpzci.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwqqlqtmu.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gsdcjgqhw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwyrjlywm.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gxloipfme.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gyboimxuy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.fehbvm.com/Article/details/gsrpovoki.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/glizlsocw.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gudaggseg.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gkovyiizk.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/gwmrpdshe.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gcvnbtohw.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gjdqqmved.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/ghdomtenl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gkkommjhx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gxaxzdmvt.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/guqbkcyta.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gbutmsbyo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/guyzimdzg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gkgeibgbd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gmcvdtsug.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/gplfwbeos.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gtifpzuak.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gcikruhzf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/gbmmuohky.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gthkzywhr.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/guhjuubit.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gxmvgtelq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/gvfoxnebj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/guetaxyba.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gjvtojszp.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gfetvzzyw.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gfkxnwmxj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gvtljwpqs.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gfbubruil.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gvdmctqdk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.zdbjq.cn/Article/details/gngabhaut.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gxazhyqwg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gpkvyctmg.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.fehbvm.com/Article/details/gszvkdreq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gkyukkhre.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/glcjmgjsm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gcsxytroi.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaadgigue.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gscjcxxxi.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.fehbvm.com/Article/details/gyttzzdgz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fehbvm.com/Article/details/gljtpkfgt.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/giqitmviw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gxdbemvej.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gwdfxbhso.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fehbvm.com/Article/details/gkpjzksri.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gwkvdlsbq.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gscarartn.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/glchmenis.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.hesvh.cn/Article/details/ggywixfyg.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gzyxwaqmi.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/ggwkihxjk.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/ggcozeyfu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghzpzkejt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/geibazknt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gltrsojsj.sHtML

[P01] 生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gkwzntrvt.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gocftrmyq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.hesvh.cn/Article/details/ggstlwayd.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gfeohwafk.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/giveypjvz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/ghqzhlccq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.hesvh.cn/Article/details/gjexbpkin.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.hesvh.cn/Article/details/gdsjwfktq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gssbcmkeu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.hesvh.cn/Article/details/gfypmgvyp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gdqthupeu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gjadxybel.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/grrstgpuh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gqcjicbhi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gcuroiqaf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gzrtuaxjx.sHtML


<!-- 参考信息 -->