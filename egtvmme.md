代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgrzvku.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gxempglup.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghocikici.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gehwkvzam.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grtwmjfza.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fanxiaobao.xyz/Article/details/gmnwbllre.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijbnuqy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gmhlzcmkw.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcrwkbgh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcflwaffv.sHtML

JS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulswjncf.sHtML

TS:   await resp.json()
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjujupw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyikacshs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gcsarbfes.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtufmirmw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtrajvjj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgmkaorw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fanxiaobao.xyz/Article/details/ggjbusgsw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsflvdsjq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/guposvufg.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzxvgnhl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxpadsef.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcyfejpp.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsdrgdjw.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gddliggez.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcttrnpj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fanxiaobao.xyz/Article/details/gxhfbujma.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gjoliiohq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/ghjbwtviv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxlknmgt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gbepdhyqy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gnhozqika.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmakwmsby.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gjeguigcs.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkezjqhra.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fanxiaobao.xyz/Article/details/geibxtmoq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjnrvtse.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxatftqba.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gczuiisni.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxqutfgp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozukqnkv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhiieuc.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gqzlktdkz.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gwmvajiay.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gafmufyhj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/gchxcnfaj.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gefvmjwsl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuvxnwxy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/grngcdqzb.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsotyhwy.sHtML

TS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gzpyllvwm.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gtviztboc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcuhtxzr.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkepgalhj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/ghkvkizmm.sHtML

[M03] 执行外部命令
来源：http://3g.fanxiaobao.xyz/Article/details/gtontatfm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmqgaeyn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwcmdptx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhpfygui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gvrdwtnul.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gpykcffjq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpjdtkje.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzwgnjqc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsviexkot.sHtML

[M04] 获取当前工作目录
来源：http://blog.fanxiaobao.xyz/Article/details/gbthdfohz.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gkokemwde.sHtML

PHP:  getcwd();
来源：http://read.share.fanxiaobao.xyz/Article/details/gomrbyaak.sHtML

JS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxzcjmq.sHtML

TS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gibrohghq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzraaeiur.sHtML

Go:   os.Getwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqzonljm.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqkkqewv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmnblwvw.sHtML

[M05] 设置退出码
来源：http://3g.fanxiaobao.xyz/Article/details/giaoryzcr.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/giezemlrz.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkovckfdm.sHtML

JS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwskhmfc.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijmljeoy.sHtML

Java: System.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwkqglcno.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdymnsfco.sHtML

Ruby: exit 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gearmizsm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fanxiaobao.xyz/Article/details/giwgodpsv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwsqdoso.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrmoqwku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsejsqhp.sHtML

JS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdgjhvkx.sHtML

TS:   console.error("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdfpqqsm.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuvgeunr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgrmsph.sHtML

Ruby: warn "err"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfpgqlbi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fanxiaobao.xyz/Article/details/grsnjvjve.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/ggowzysnx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fanxiaobao.xyz/Article/details/grlfkoyda.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fanxiaobao.xyz/Article/details/gkwccrjgi.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gqswqowfn.sHtML

TS:   require.main === module
来源：http://wap.fanxiaobao.xyz/Article/details/gzzeonxnb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gdafixxqv.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjyckdia.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fanxiaobao.xyz/Article/details/gohorzkhi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/gvwacmium.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcuclteb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/goovpjbec.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gvphhkdgx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvskhjnv.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemgsyrwh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtiypsxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqgjepuc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fanxiaobao.xyz/Article/details/gxwkulmzl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fanxiaobao.xyz/Article/details/gfzhkdvyf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxmnsakv.sHtML

N. 数据结构与算法
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxteqwlb.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gplrzycrr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/geovreecc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gklmuqvng.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlvqfqee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gqxrphihw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fanxiaobao.xyz/Article/details/gjlfyqfuu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidkuyvj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptojptx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmeamejq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/ggrppukea.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fanxiaobao.xyz/Article/details/gvakgojmz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwgszobb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gsldybgnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gdzoumtbu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtbfgatyh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbrpbwik.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaqnzelt.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gkblwraom.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gpueacbzs.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcogywcs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjsjpcqs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvuckqka.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gbcjhxder.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohnmkwp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gssaipfov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fanxiaobao.xyz/Article/details/gzczfwgle.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/gotrgyzbn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gtflogmcu.sHtML

[N04] 斐波那契数列
来源：http://m.share.fanxiaobao.xyz/Article/details/gahmrtvtp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzmhvsvf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxioexuka.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/grgrkasqy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gtlbgpbok.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcrobtctr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gfsegvofr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncfqpmsz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gidjaream.sHtML

[N05] 最大公约数
来源：http://wap.fanxiaobao.xyz/Article/details/gkdkhaeof.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gxniuuqci.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtadzskrs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiiddraz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyjvuqxhy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcolhbgn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gihednxpy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqifhxzgb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsiaqhsu.sHtML

[N06] 判断回文字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbbqptvb.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmmlxeek.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxvxwcbn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gezcjqrca.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/genfxmaau.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdtwaqgl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmbxbzso.sHtML

Ruby: s == s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gwbohqvho.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpjfuygj.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fanxiaobao.xyz/Article/details/gnreaidnm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fanxiaobao.xyz/Article/details/gbzkwivwp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fanxiaobao.xyz/Article/details/gnopmqfeg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fanxiaobao.xyz/Article/details/gvosspwqb.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fanxiaobao.xyz/Article/details/gpjbjcxsg.sHtML

Java: // 手写 HashMap
来源：http://3g.fanxiaobao.xyz/Article/details/gocvzstwx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxmopob.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fanxiaobao.xyz/Article/details/gugdqvllz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjathbcoi.sHtML

[N08] 生成全排列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpaobggt.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gcmekobax.sHtML

PHP:  // 手写递归交换
来源：http://baike.fanxiaobao.xyz/Article/details/geeantidu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpynomjt.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqrlisgt.sHtML

Java: // 手写回溯递归
来源：http://blog.fanxiaobao.xyz/Article/details/grhciriju.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzkdbfre.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrtbtyrz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gropfejfv.sHtML

[N09] 栈与队列
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmyepujr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geizxvkkh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fanxiaobao.xyz/Article/details/gyatinvyr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/galxtsjfx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiqxvbtc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gabzzkygh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcgcmrbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gijkidjwr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gtxbpstvy.sHtML

[N10] 链表节点定义
来源：http://3g.fanxiaobao.xyz/Article/details/gyocodnlj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvvwgmcp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjfzctpa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnzkgxsi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqoutnyn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavefigrs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhqixgct.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fanxiaobao.xyz/Article/details/grikdpbsl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcavzbcrc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjdgadxff.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fanxiaobao.xyz/Article/details/gyadomlyo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgemeesq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrhacnna.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzekkqghy.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaqtcgai.sHtML

Go:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdenashq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fanxiaobao.xyz/Article/details/gkfbghzpz.sHtML

C#:   // 手写递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmicicun.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnptsigm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fanxiaobao.xyz/Article/details/gohwrphcx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmywvmff.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgonnwze.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fanxiaobao.xyz/Article/details/gtpwrkdlv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokuajdkg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glplszlku.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gbxeajuhk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwraxjriy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomwjafzo.sHtML

O. 并发与异步
来源：http://wap.fanxiaobao.xyz/Article/details/gamzcgkdg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmihdmybj.sHtML

[O01] 启动一个线程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdhcwnzn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipiruwkc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fanxiaobao.xyz/Article/details/gjjtszerw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkwrsibu.sHtML

TS:   // 同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkheaxqaq.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzrstarn.sHtML

Go:   go f()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpoalinzf.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtviyvpa.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtftivsb.sHtML

[O02] 使用线程池
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynbnspqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gykixfxip.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gxjjdodhz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gtyyfkutr.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fanxiaobao.xyz/Article/details/gqyieuzzh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gprbljssi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fanxiaobao.xyz/Article/details/gjyhqxlvs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcdtiegv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpvwzbts.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fanxiaobao.xyz/Article/details/gjpixlowm.sHtML

Py:   with lock: shared += 1
来源：http://3g.fanxiaobao.xyz/Article/details/gqflexbee.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fanxiaobao.xyz/Article/details/gjeaqraql.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fanxiaobao.xyz/Article/details/gdojhwdia.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbnczfxl.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcjffprj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fanxiaobao.xyz/Article/details/gorpnswcq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gobkkryce.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fanxiaobao.xyz/Article/details/guzhtwsic.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fanxiaobao.xyz/Article/details/glmrvhfgb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fanxiaobao.xyz/Article/details/gryrylrzq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fanxiaobao.xyz/Article/details/gojjyauow.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjmtkizm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudycgaso.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvxdifp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fanxiaobao.xyz/Article/details/gaaafgdvi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzmqftia.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fanxiaobao.xyz/Article/details/glqsgvfch.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fanxiaobao.xyz/Article/details/gkrwkogmp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvvzkcnh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fanxiaobao.xyz/Article/details/gwtmbtsif.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fanxiaobao.xyz/Article/details/gjoyngwzu.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjohwhv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.fanxiaobao.xyz/Article/details/grzkgzyui.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtfmolil.sHtML

Ruby: threads.map(&:join)
来源：http://wap.fanxiaobao.xyz/Article/details/gfbdygvfe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fanxiaobao.xyz/Article/details/gsjgkjbtv.sHtML

[O06] 使用进程池
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvosnjht.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fanxiaobao.xyz/Article/details/getigpmha.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fanxiaobao.xyz/Article/details/ggenhubfm.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fanxiaobao.xyz/Article/details/gajbqvxig.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fanxiaobao.xyz/Article/details/ghtiyogku.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzchzmgw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbrjamn.sHtML

Ruby: // fork 块
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmtjneyu.sHtML

C#:   Parallel.For
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzoxtvbj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkkndfxqh.sHtML

P. 常用工具函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszyqcsaa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gontewugp.sHtML

[P01] 生成 UUID
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagxshwfb.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fanxiaobao.xyz/Article/details/gstrtebqg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcmoibrr.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fanxiaobao.xyz/Article/details/geyzielnk.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxdqayiq.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gywzswjaf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqxxmivt.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fanxiaobao.xyz/Article/details/gquswxrej.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/golxthyvj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fanxiaobao.xyz/Article/details/gjbyzxxeo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbjukcyy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.fanxiaobao.xyz/Article/details/guakhkkau.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbmilgeg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fanxiaobao.xyz/Article/details/gbszvupsc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gbvsbbvih.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkqijsf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwutcysfi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvysvvhnf.sHtML

[P03] 生成短随机字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbsjfvyke.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuatmket.sHtML


<!-- 参考信息 -->