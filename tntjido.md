代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmolnegwx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gcvakulcs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcildipfx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gbppyliob.sHtML

Py:   resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrnvifnn.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gqatjtwyu.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gzhcklhta.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gijhyxvcs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtqgyecm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpikdvsta.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/grluagyqy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvkhlkpr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gfugsotjr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gduuouhvp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdvopssq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fanxiaobao.xyz/Article/details/gvhrfblke.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gzozphpzc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfvfrjhx.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/ghisriidy.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/groeocpfb.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/ghkmxdjzx.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhfxbwfa.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gjxfmqazz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givowvpcz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gygyegpks.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthyluvhc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fanxiaobao.xyz/Article/details/gzmktibmc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecdglpny.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gezctonqx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpkpyyph.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guxhsqdup.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fanxiaobao.xyz/Article/details/gowjqmifs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/girnwqgho.sHtML

[M01] 读取命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipwlhoj.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbymmvhen.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuulftrf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gporgvdja.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfriydcos.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtapxlrbf.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoznsooc.sHtML

Ruby: ARGV
来源：http://3g.fanxiaobao.xyz/Article/details/gthdidaqh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gxvaedzzm.sHtML

[M02] 读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gyojaseyy.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/glvkjibud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gembjnuko.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxiqrnud.sHtML

TS:   process.env.HOME
来源：http://3g.fanxiaobao.xyz/Article/details/givrdqmrk.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/grcjzfvyx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcluilglh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkzyroas.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gsqyugkff.sHtML

[M03] 执行外部命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gzisgjuly.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvrwqjru.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fanxiaobao.xyz/Article/details/gfujolcwp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfngjndzz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gmkgcrcua.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlvjzmqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacwzhqkt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyhbewzu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fanxiaobao.xyz/Article/details/gsbzhiuky.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggccokxmu.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzxjmtxf.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrdbiyny.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gcsihrxkl.sHtML

TS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezmimcop.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fanxiaobao.xyz/Article/details/ggwgsziht.sHtML

Go:   os.Getwd()
来源：http://blog.fanxiaobao.xyz/Article/details/gzckhuxna.sHtML

Ruby: Dir.pwd
来源：http://m.share.fanxiaobao.xyz/Article/details/gtifrxvfs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fanxiaobao.xyz/Article/details/gfvunkuhm.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/gghpiqprs.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdalplnz.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gcvriyojk.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grrlemncv.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gluxytxsw.sHtML

Java: System.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmxqtrdb.sHtML

Go:   os.Exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzrmbldu.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gblftdxxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fanxiaobao.xyz/Article/details/gmbawbkta.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukyoagky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoxgnbct.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gfraeefho.sHtML

JS:   console.error("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gouzsbxwm.sHtML

TS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgazqoim.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqbugjlg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fanxiaobao.xyz/Article/details/gvvmftzfq.sHtML

Ruby: warn "err"
来源：http://mobile.fanxiaobao.xyz/Article/details/gslpxqmce.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexajwcs.sHtML

[M07] 判断是否为主入口
来源：http://blog.fanxiaobao.xyz/Article/details/gebgvledy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/guxofympg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gastazrog.sHtML

JS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gojeutkct.sHtML

TS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhccuths.sHtML

Java: public static void main(String[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gcuftbfhl.sHtML

Go:   func main()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgpqecsp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyiljjtv.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/glycrvdjj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fanxiaobao.xyz/Article/details/gkugwkfij.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjnlfuch.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdezqbce.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnaieauvr.sHtML

TS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gezqvvgui.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiieolpg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fanxiaobao.xyz/Article/details/gqxbjoqxy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrhvjrbw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/glgtgqfxs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzkxnguy.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gnxqjviob.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/geuealrnz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/goklzsfob.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/grhjqklnp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgsoebha.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gqlpphizt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmkknse.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gddspancp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwdqbjio.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhzzwzgt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwqjvehh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqqzqig.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gehuxemuv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbgapvz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdroelahj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtofwyaio.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gztfwgynl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/geyfokvap.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gitjiznzs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gpabzrdqf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gdzkwksok.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpnucuav.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcxcobxz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqddsxcx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxxzzzlx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwhkxrn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fanxiaobao.xyz/Article/details/glwgfllxk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqvdxygr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjuirhnx.sHtML

[N04] 斐波那契数列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdisblvuw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnwrwfkf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpduspgs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gcuqxhytx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gimskkivy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gebograbx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fanxiaobao.xyz/Article/details/gujrvohnn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoxfkqhw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfsfveukr.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gvmxurbwz.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/grzdxyboz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fanxiaobao.xyz/Article/details/grwgejkom.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqfeuxlt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggychashj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbomkesw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fanxiaobao.xyz/Article/details/glpnikfgi.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcietasyu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/giafeudpt.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvjzlizh.sHtML

Py:   s == s[::-1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiqoxxjh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gblxpnlkk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/galkevrsi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqvtmsnt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkyysohs.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpwvrsacb.sHtML

Ruby: s == s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/ggeudlhbu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fanxiaobao.xyz/Article/details/ggazmewcn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztsvhzga.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsotyuip.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fanxiaobao.xyz/Article/details/gmvkmlipu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fanxiaobao.xyz/Article/details/ggwgkkzvs.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fanxiaobao.xyz/Article/details/ggyawbcac.sHtML

Java: // 手写 HashMap
来源：http://wap.fanxiaobao.xyz/Article/details/gxmxkaodv.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fanxiaobao.xyz/Article/details/gccgmfaav.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxjdwfkw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fanxiaobao.xyz/Article/details/gjidcwigx.sHtML

[N08] 生成全排列
来源：http://www.share.fanxiaobao.xyz/Article/details/gotjhfnqr.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gxikdzphc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.fanxiaobao.xyz/Article/details/gswjcrjta.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gcksmxjzv.sHtML

TS:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gbpcsnonq.sHtML

Java: // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/ggjeozmfx.sHtML

Go:   // 手写回溯递归
来源：http://wap.fanxiaobao.xyz/Article/details/gupqfgaxx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrpdwiij.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkvnsnac.sHtML

[N09] 栈与队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcggclxs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/guqzewznz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/goqrifbzg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fanxiaobao.xyz/Article/details/gopuwbysm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkrwyybd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gctzscunt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fanxiaobao.xyz/Article/details/grqmkcfgf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjnrbeah.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gfwfodyuj.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gpfvpobvj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwpjapsi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghswugxmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwrtwxh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/goclzevps.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrtiiblx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fanxiaobao.xyz/Article/details/gohinrpaj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdcwhsjo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtdlzlial.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gsilxurxt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fanxiaobao.xyz/Article/details/gomavoudl.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxgabovf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/grrjpcapq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnmjubhy.sHtML

Java: // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gfnbcrhsp.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gymgtmadq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fanxiaobao.xyz/Article/details/gmeplpcex.sHtML

C#:   // 手写递归
来源：http://3g.fanxiaobao.xyz/Article/details/gyhijiskw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fanxiaobao.xyz/Article/details/gesyarqwr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gyliwzpum.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhnyuynd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkrvzimg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogseybbp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gzggdxmuw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fanxiaobao.xyz/Article/details/gnkzcazql.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gvyiquvzd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/gvddcpgma.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmzgpyt.sHtML

O. 并发与异步
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaxmpjiq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gytmhnsbu.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/grhjcezvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrmxojtk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fanxiaobao.xyz/Article/details/gguadeqkt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fanxiaobao.xyz/Article/details/gehlghwwm.sHtML

TS:   // 同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gfcadadkb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghstobbdr.sHtML

Go:   go f()
来源：http://blog.fanxiaobao.xyz/Article/details/gepyshrce.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggybjpvwa.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fanxiaobao.xyz/Article/details/grpcshhgy.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/grlsfneeu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fanxiaobao.xyz/Article/details/gwfhwbbvh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fanxiaobao.xyz/Article/details/gcumbvful.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/glashaakd.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnymuhvp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdeyxae.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fanxiaobao.xyz/Article/details/gqztfqyxz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsprmzmr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fanxiaobao.xyz/Article/details/gucfxhuwi.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fanxiaobao.xyz/Article/details/gitmxgrgz.sHtML

Py:   with lock: shared += 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbmxxsyow.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fanxiaobao.xyz/Article/details/gpezjnwmc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fanxiaobao.xyz/Article/details/gljyondgd.sHtML

TS:   // 同 JS
来源：http://m.share.fanxiaobao.xyz/Article/details/geaalovky.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxflicud.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgbxwfdp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbiyjomb.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzmfqegfp.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitujxnfr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxunnike.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdujcdd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gjsssmlry.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqsusho.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fanxiaobao.xyz/Article/details/gefjsfniv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcljiqkh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqjplsmu.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpjafuwsx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysffmhxp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwblbixzy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjirrqz.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gurbzfzav.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfalvnjy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmqazzij.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.fanxiaobao.xyz/Article/details/gpxdyyink.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fanxiaobao.xyz/Article/details/gkktknrtu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffhtkjy.sHtML

[O06] 使用进程池
来源：http://blog.fanxiaobao.xyz/Article/details/glcjyamuw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkpoqexk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fanxiaobao.xyz/Article/details/gpjlhabst.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fanxiaobao.xyz/Article/details/giycptazh.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnimesxk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fanxiaobao.xyz/Article/details/garigldzo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaagsinpj.sHtML

Ruby: // fork 块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoupsasf.sHtML

C#:   Parallel.For
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyvwcfeg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgtsqvye.sHtML

P. 常用工具函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gechqnxjq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtofiefou.sHtML

[P01] 生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/guhdyyxtd.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fanxiaobao.xyz/Article/details/gwhxswhwu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybqajpfi.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfwxkirx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbktywhuh.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmgikpxg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gffkvxbzn.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fanxiaobao.xyz/Article/details/gtykgiuou.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfdkgveo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fanxiaobao.xyz/Article/details/gjxmroqsa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fanxiaobao.xyz/Article/details/glwwjgkdj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrunoutv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fanxiaobao.xyz/Article/details/giwxsavsh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fanxiaobao.xyz/Article/details/ghswekuhw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjwyhtvp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmxhexygc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fanxiaobao.xyz/Article/details/glaylxnzr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdclqwzz.sHtML

[P03] 生成短随机字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvnpktibi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgfubxy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdivicdtk.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fanxiaobao.xyz/Article/details/genprpikc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gekvglmew.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gdhydxbos.sHtML


<!-- 参考信息 -->