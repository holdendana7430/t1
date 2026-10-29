代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gwjoifqat.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gdcuyljsv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gbrgqzelc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/ghydoveaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gfqkxwjpl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gulewbsbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gdgflgnct.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/ggukdjpqc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/glidbqqcv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gsiaaioop.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtvjjpgmn.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjpemevwi.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gsmpnhovg.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/glaouazsa.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gnsfgwpys.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbjradhzr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmihzudpo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/ggyidtjxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/grwifhpnp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gnihyfjni.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gfpiudslr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gvgirkmgw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ghuhycgks.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gsgznkdoh.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gkkjgyica.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gzvopdpgl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/geeeybsqr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gvtwaptbu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gcrzgwhpy.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gdgpskeeg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/ggenpihec.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gwibgsupr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gqhcsozru.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/geelfzolf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gegmesmvv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/ggyonjhcl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gxlwelfac.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gevwlmars.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvpbgauzy.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/geiaenwln.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmrlkcstx.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/griyrgxuc.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/ghepadobh.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gvfllvphr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxxngmpot.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gidxixgjx.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ggveegycy.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjuygrcqr.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gdijyhhza.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gioxoczmz.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gotdoxfqo.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjetazmgm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gifghylce.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gvpuieprf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gigjcphvk.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gcsrdfcrv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gmjiylmzc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gtjvrvvla.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqbnrwswy.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gfyfgjntw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gkshkhexx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gtyvvgzrj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gtmcxodme.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gisrhdnxb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gchmbkbzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gtrpsnfwd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gmmondcgx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gepnroikd.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gvtqozcbf.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/guysjcnho.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gwtnzkqvy.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gbqyvtbym.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/grgucndjz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gyrjqknwd.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gprnnzfki.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gujtardpd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gweouavxw.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gfrdhonfu.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmxefkzbi.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gtxpdbojq.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnywrgpye.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnezhmumv.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ggnhdhhtk.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gudzjbprp.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gyujnfsjv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gjdzaqmvn.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gzmcoilxq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gtjoasyjg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ggayrgfmn.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gvhuizxgk.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ghckubbpx.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gmmovycij.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gssdmnqsx.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/ghyhswwxe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gkgronnzx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gyrrqzleu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gmteklyni.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/guaflzfzo.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gfttbsise.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gvbkcldzu.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gqvorgcub.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gqmouaywg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gvekomdtq.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gcksvvfym.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/govsmivow.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gkgajaovx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gmzyrvjjp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gviemctyu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gwhprxrrw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/ggpmsdepp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gbgfqoadf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gnexiqgbn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gwkifftlj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gryfiaowu.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/giiktoatl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzdukrgry.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gegjdkzyg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/grzpbregb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gdnleexlf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/glcueyhll.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gqccvhsqq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gqgraxqtj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gtsppewiy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/guihoedad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcaywqesf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gnrjtofvv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/ggjyitkec.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gwynshbee.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gollgnecz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gwwupqbkd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/guflluegz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwlvraefs.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/ghxlkxzok.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gatgzeigz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gxovbyemx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gffdztimo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gixorsvpz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gymqgckos.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gojtgqwus.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gwrymrttd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gsazwnicl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gxwuumxyh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/ghhnatbcf.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gmgzvqjnx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqwcghh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gnjaruqwx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjovmaeqg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gtqxgsbjh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gsgikjvde.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fehbvm.com/Article/details/gehjengxp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ghjamfsya.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gwqrynjio.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gwxbaiuqb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gmfhfhaph.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gnyprwwtw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gynbzjpjd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gtcgptxwq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gpslokeae.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gtixrbhdd.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gefnfaqne.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/grjbcsoqu.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gwzjbivfb.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxyxhrkku.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gcfdjgtpr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gyytlsgry.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmlbyfyvu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gotgcfsbq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gvqgqebpf.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gaovbssaj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gpmcfbwjs.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gsptgnrll.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ggnocrpym.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gleuxhyob.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gqskkkxsc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gvjrqrrpd.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gignioqqj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gdgjoyidb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gmybrrhla.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gbwswskke.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gejvkuyjr.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/ghuflsbic.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gawmrrisr.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gpiknahyr.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gslwkvwld.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gmjgeegkm.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gliqqtnrn.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gnscqhbyk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/getzjoilr.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/goivvtahm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gtvvxoifa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gymncddiv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gzwtgucam.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gfzhdymfw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gotuobfdf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gnjckfthx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gkcumepgo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gndwuarer.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gcohflqko.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/giqvuxudz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gzohsienv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gnskusajp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gbebktyos.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/gamuottzj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gwyldzzyj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gujzvjmxa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gsfxiiefc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/ghvayrvod.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gtiblvzbp.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gyfdovkhw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/ghaidrogr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gxlaixgqb.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gkdwowdyd.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/ggmwehtyj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gphdpwemf.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gfxymgead.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gkqitarmn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gfpcfcqad.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gwpaljcfb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gamajraam.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gschmnwfk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/glsfmiihv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gjovalvff.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gpaoeanuy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/geckxhzzf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gekveqxrt.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gwmxvbcuq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxxkplglo.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/ghpihrkqr.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/ghufhtmbs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/grzppvcim.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gqsatsoqz.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gcalnykdb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gnuiokmfv.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gtrlzitup.sHtML

Ruby: Thread.new { f }
来源：http://3g.zdbjq.cn/Article/details/gqjyzgdia.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gitxutghe.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gdbhvzlhb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfiyaocj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gudinlivl.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gnpaugafi.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gbdnrbplm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/giuzngtlx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/gilwcssem.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gtwikbqzd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gkifqjjjq.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gpkwhrslj.sHtML

Py:   with lock: shared += 1
来源：http://blog.hesvh.cn/Article/details/gzhqdcmit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gzpxvsezf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gxiuxcxod.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gxyvcallz.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gkftrfbih.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/giusknsmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/ggriqtoui.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gtpyvjtdv.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fehbvm.com/Article/details/gqxlibddz.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.zdbjq.cn/Article/details/glvidbtpp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/glnldpjlp.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gpupywcsb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/ghvnajnui.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gjdkbjbfh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gisrvqfwo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gaftxckbu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.zdbjq.cn/Article/details/goisloomy.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/grpyqrbwj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.zdbjq.cn/Article/details/glorkjdex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.zdbjq.cn/Article/details/gkogdtnux.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.hesvh.cn/Article/details/gfgqxlcpi.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gzttmuzkc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fehbvm.com/Article/details/gnkstvqts.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gdcppzisk.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjwqulhfj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/grhjftmra.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/gunrdszjp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gkunalryg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gmstreggp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gubjiipta.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/grmkmjhmb.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gbaczebdr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gtsycondw.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gyuspnmty.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gcbpbcady.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnodqsbcu.sHtML

P. 常用工具函数
来源：http://www.m.share.hesvh.cn/Article/details/gcbghjsjs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcoootmpe.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gfjsohfmh.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gmhbbjofr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gjdyrmqyh.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjkwejyqx.sHtML

TS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdrmmwioe.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gjwssaeij.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gbqjuhmqm.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/givflrfwx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gijjnjdze.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gwiestcuy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gycojwfay.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.hesvh.cn/Article/details/gifjtfigi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/garquqqsd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/gdfvoinvs.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gcukxwmdf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.zdbjq.cn/Article/details/gxpnzwllx.sHtML


<!-- 参考信息 -->