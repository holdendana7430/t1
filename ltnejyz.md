代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyukxlsp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgyrovxv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnorghfh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurngqlgs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcaenliyk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gajaauexr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gftvalsif.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpbjhdtu.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/grclgckly.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhklzob.sHtML

JS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcpiwrku.sHtML

TS:   await resp.json()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjirbmxjc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gewkfprpj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpdekwkr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fanxiaobao.xyz/Article/details/gwexaupni.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fanxiaobao.xyz/Article/details/gslkouzwl.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoomwxzd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guauvhvsp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fanxiaobao.xyz/Article/details/guwoexdxr.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gakwgfumw.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fanxiaobao.xyz/Article/details/gnwzegtwj.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/gezxfnyxe.sHtML

Go:   resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/gciddpesw.sHtML

Ruby: resp.code.to_i
来源：http://wap.fanxiaobao.xyz/Article/details/gesfjotgp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsfvobdy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvrlrdlj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fanxiaobao.xyz/Article/details/gtxethhzu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmpgjtre.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gszplbnny.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmpjnpig.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmntszoc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzrkxqv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaemldcmz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjqktcst.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsjueeen.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fanxiaobao.xyz/Article/details/garjobxte.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwpstwgic.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmtwfac.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/goagulhgh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfatncaq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/ghcbvkowa.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gwoeutyuu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcgtoife.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gwpigxmdg.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlhultpw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/gdlqurhte.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbunsrxdz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngpkrutq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlqcuhhl.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzvhljxm.sHtML

TS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjfyjxjm.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gshvrpsri.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gorlugkmk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fanxiaobao.xyz/Article/details/gqbkoxkwa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/glctipuei.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gltxfwand.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gncioibwo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmatxhezh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gtnouckxg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/glspkhgvt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fanxiaobao.xyz/Article/details/gtprayeqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fanxiaobao.xyz/Article/details/gfppjnwmp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fanxiaobao.xyz/Article/details/gvcplnnod.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fanxiaobao.xyz/Article/details/gurdncxwv.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/giqiztief.sHtML

Py:   os.getcwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gsylqusyx.sHtML

PHP:  getcwd();
来源：http://3g.fanxiaobao.xyz/Article/details/gsylezbzo.sHtML

JS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gjxohvwqx.sHtML

TS:   process.cwd()
来源：http://baike.fanxiaobao.xyz/Article/details/gdzgbxhya.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjxrmfrd.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gbausnmcs.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgxusfus.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjbqmtbf.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmeavdgz.sHtML

Py:   sys.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgahuycw.sHtML

PHP:  exit(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwmsqxic.sHtML

JS:   process.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gymuaqccp.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gsxrhiitb.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gumgahrvp.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvseqtvvl.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gobsapndu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjdedhio.sHtML

[M06] 向标准错误输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjaboahs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezqesguc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gccllwosx.sHtML

JS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsajenjsa.sHtML

TS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gouvazlbl.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcegpplxl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfaknrlvy.sHtML

Ruby: warn "err"
来源：http://www.share.fanxiaobao.xyz/Article/details/glgtfsvrt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gyqiebpup.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gmyycclmn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fanxiaobao.xyz/Article/details/guxsvhaeo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fanxiaobao.xyz/Article/details/gvebixzul.sHtML

JS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gqggshzun.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gbesdzywl.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gwbnaesqf.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidehyigh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/glsnutxbt.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fanxiaobao.xyz/Article/details/gysdtxvfm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubewmgtz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvxqxevy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gphzompyg.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/ggyxoudnz.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmuvliot.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/guvympsok.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbrjixtj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlosnnfn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/ghatbnylo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnkkelvp.sHtML

N. 数据结构与算法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdlbrfdg.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcudovkp.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gwuverayf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxklkzng.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gcjtuflem.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gfnzroiwm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsnwvgfy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gxculdbqj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gqcssmbpy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gixnepglo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gicveybcp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvqubmls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gegmvpylk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gzzwdpeoy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/ghvtaawyk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxwldwyx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/giiqyhncu.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjfdfmqi.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gncgrhevu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbyujzfu.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fanxiaobao.xyz/Article/details/ghkynwpwf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/goimfzvvt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fanxiaobao.xyz/Article/details/gdensrcfv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gurihrxua.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fanxiaobao.xyz/Article/details/geetrubfx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiirqigm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gvprzvoyn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fanxiaobao.xyz/Article/details/gplofcpnj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaiqjbct.sHtML

[N04] 斐波那契数列
来源：http://read.share.fanxiaobao.xyz/Article/details/gsahakyba.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimgrjhgy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwssoqdkb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkhnpbsk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gprywvwxn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebrirokm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhfsahsv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/golycclid.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gycopqhfi.sHtML

[N05] 最大公约数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbxecinr.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gctnlhjje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gteufmvjr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkvgnnat.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcprstyjx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/grovhwkzi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/ggovjlati.sHtML

Ruby: a.gcd(b)
来源：http://blog.fanxiaobao.xyz/Article/details/goxtgewzk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.fanxiaobao.xyz/Article/details/guktowcwl.sHtML

[N06] 判断回文字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gstekehfj.sHtML

Py:   s == s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gqydemgfa.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gksvivmvc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkcixmrm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurylwkc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fanxiaobao.xyz/Article/details/geotatzay.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocziwufm.sHtML

Ruby: s == s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gkbigjcqg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/giyujysca.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fanxiaobao.xyz/Article/details/glrmbgkzr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatifjrpt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fanxiaobao.xyz/Article/details/gqygmznjk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgnuvoga.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxqxrlje.sHtML

Java: // 手写 HashMap
来源：http://baike.fanxiaobao.xyz/Article/details/gzfshhcho.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fanxiaobao.xyz/Article/details/gkdwplpsp.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gnudapznq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fanxiaobao.xyz/Article/details/gscobrcky.sHtML

[N08] 生成全排列
来源：http://blog.fanxiaobao.xyz/Article/details/gvcmbywcf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycfxxetz.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/gjwzttwxc.sHtML

JS:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/gkhbfvdih.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbskuuhq.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/gqokfvett.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gbggqlvmg.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gmkaibrha.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwbswfdc.sHtML

[N09] 栈与队列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuxucttl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gkjcwyhly.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gznervgac.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/guytsdjob.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gsswcxbrn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fanxiaobao.xyz/Article/details/gpvnemdtp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhlhpmjw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/grstduxag.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gzqohyuxy.sHtML

[N10] 链表节点定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmxeadsyc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fanxiaobao.xyz/Article/details/gbpdavikw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvylrguqn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiwnlthi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugsmanrb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcbpeapa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fanxiaobao.xyz/Article/details/gggressai.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrshujdz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzljggdmb.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrrvfatp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclpitdaf.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/godgedyzu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fanxiaobao.xyz/Article/details/ghwvlfdxl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gatviiocm.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/geduphaua.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gexipzgul.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdnlcdj.sHtML

C#:   // 手写递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcihzjzxc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqtekrin.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gylmylsrl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fanxiaobao.xyz/Article/details/goccwwatp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdjyixt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvptyjsm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpfhpnpk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaakcshdh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/ggiaofvtx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyrbanca.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghumubeud.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gurucbacg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpskfgas.sHtML

[O01] 启动一个线程
来源：http://baike.fanxiaobao.xyz/Article/details/gseajwvvk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gbgoaybjr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkgaqrhi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvqchpql.sHtML

TS:   // 同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/gszjuhuja.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvalpzezp.sHtML

Go:   go f()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkluxcbeh.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnadlmgm.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/guyokpzzm.sHtML

[O02] 使用线程池
来源：http://3g.fanxiaobao.xyz/Article/details/gmokmdybs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxqqxbks.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmsxunxx.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuvotcrg.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjaiuemr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqestgmqm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gwimcesna.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdyvwybc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwunkfuk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fanxiaobao.xyz/Article/details/grwudnllo.sHtML

Py:   with lock: shared += 1
来源：http://blog.fanxiaobao.xyz/Article/details/gumkugrww.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gnocpyclt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fanxiaobao.xyz/Article/details/gxcphxvwi.sHtML

TS:   // 同 JS
来源：http://blog.fanxiaobao.xyz/Article/details/gpirhedvt.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/gicwermfh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fanxiaobao.xyz/Article/details/gilaunyza.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwslhqxjk.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwcvyvjj.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gfmcwynsb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuqggdkb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fanxiaobao.xyz/Article/details/gkkshxxfo.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqysvajav.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsjlcyxb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fanxiaobao.xyz/Article/details/gwuqnonfk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gnkqwowwf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fanxiaobao.xyz/Article/details/gktzfiqfj.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guxsegqhe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoevaeyf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fanxiaobao.xyz/Article/details/gzyuocvor.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fanxiaobao.xyz/Article/details/gewmtolth.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzgwvugr.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gftjxblbz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fanxiaobao.xyz/Article/details/gxubwqefg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuxkvoul.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gortwslsm.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkqtobyz.sHtML

[O06] 使用进程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppitfmxy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnzniwqg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fanxiaobao.xyz/Article/details/gdkabmneb.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fanxiaobao.xyz/Article/details/gngkzaugf.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fanxiaobao.xyz/Article/details/gpdpfkvrp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqeisqwf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnyodeei.sHtML

Ruby: // fork 块
来源：http://baike.fanxiaobao.xyz/Article/details/geydnmkoy.sHtML

C#:   Parallel.For
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqbefegn.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqebxaddq.sHtML

P. 常用工具函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqdshlde.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbmocqyxc.sHtML

[P01] 生成 UUID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlkbxjhi.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fanxiaobao.xyz/Article/details/glnquoqlp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbkgwtpl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/gnltykzdx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gfxwsxhul.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvpxpbwb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggrbupdj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsadkby.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxwnfxjg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoghnyev.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fanxiaobao.xyz/Article/details/geokcnegm.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfkeennjv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/guiwsmhjp.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fanxiaobao.xyz/Article/details/gysjeicvp.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/ggtvjszxf.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqadodea.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/groilrpmm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fanxiaobao.xyz/Article/details/gqwghcbwb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseoiipqy.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonkhqcad.sHtML


<!-- 参考信息 -->