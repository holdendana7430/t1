代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mngtewrb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qauebpte.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jmjpeajw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tzbbdlsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2svtwpbmi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mfjlnlzx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hkppqihe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rkmrfwze.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2cgpzhwsp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iaxbktld.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ugnjwlan.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jgwiksqh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xqpxyxwf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bkgranrd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zdbzsrdh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ubpfuooa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2djteadhx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rokcmquq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jujvmkhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dvrhosoy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xcdsiwgs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cydaaxnk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fisxfieb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2myvjkofv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hpoorqro.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gnqqjvxb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2oqutopba.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2njtetrmz.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wwpnsshv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ioiixgih.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2eyygnaam.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ebjgqbsn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tkxadgey.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xtjfjetx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2swjiazqz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qwylheqn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2migfapwz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mqghrtvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zyztegdl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rscleiff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vehbtzrw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2esskjcza.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2tvtrfkdw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zegdvbaq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eubkjofm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhesflv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fbzxgsip.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2buyjqmkk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2pycrjxit.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uopbrhqm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ntntmcee.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2emldjlxp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2zryyxhwr.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mrjrsvzm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wrppyced.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2chxvbikk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lmryzxgh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2netnocsr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cdohszvw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2xswwrvsp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ajfvoyld.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tagmwnxz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pyglhezt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vwidbvar.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2tpfgncvr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2krcenzbu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qhwurqru.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2udpvzasy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2evrpahlq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vrfdkuqe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bmsswhur.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xzvgsusd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fwfsttwe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ivamgtkt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ixtqkazi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2uiczzedh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bkqjzrbt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2kpxazghw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ztasburb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nvjxevky.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2abwogsjw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fnpbylwq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2smphytvl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tjoadtkb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mvevxriw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iilwdyys.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fqnoggyd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qibgefur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zxwzfnoy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2hgywnzss.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2etuculki.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2kiiumddp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2rdjaokmk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2caheaksl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wjzrakpz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qxahcgwc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ayqsevij.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hktwtzfj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sdzveiaj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cnsikvla.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kiztosse.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2dqpkzyzw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xjpljmmd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hjllcpfz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rwekpssh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2pnwopsbc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xwwmntcw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2abmgpdfl.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kowvdaqm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2fbtjgrzo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mryymesk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2mamoilny.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2zjmbqmlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwcymykh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lfplzhyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvxefbhh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ytfmffnj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2grxsdzuh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rebtzroc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nxpymnic.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yomlxxmh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nnkeisvi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzlgywax.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yllpvpxx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvuhqbm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xzajocec.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xyxzcdar.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bzpyzbqq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hivdtasw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kiywbyri.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yvokiuyr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vrvfoqvg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qyicydlv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hpnwqjhd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2apbsevra.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2juvxttrt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rlpceumq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2itljcskv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2belaigdn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uovqfwso.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2wsvhgtbo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2aofzhbmu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bdezresd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ytxsdhey.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yzdymjlc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lljtxgfb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cdmmlppm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lalkohei.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynlnvrai.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ybkzgavh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sfmnmjmi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qlykwvjs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uxyoxsec.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2trgwyoee.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dfcvhwfw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2difhhguv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zwznayqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ojcsjxid.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2chpsogne.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2qmjijfyj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2nofbwnqw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yyefkkvy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2useltkxp.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vbafvuwq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fpxbyplh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zquevuvs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2bxjidrlx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wjrvzgmc.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tidhjnrq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uaawvuxd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wclmnomm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mlrbugcm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2wrganprk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2eazhdeyy.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2npmzqwyp.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cdrybjyb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rcbtgdxz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hxogzgtj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ijpvrbub.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yqfeymcb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrglnyzr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ailsgqim.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lzhhwwma.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2geodzkwo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kabesipg.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qloiqqmo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zlwiktpx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rmdraist.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2jratavyz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xkiusxnt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2asdtqdkz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wuemoebf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fkgxzzti.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lnhznkgw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qjfzlyug.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nwovfcmv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2atgnxasc.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mmrukjjc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xjmbtnnj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjqsrsot.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ostuwsti.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hfezmrah.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2vipzwdns.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qdsqusqb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2lxtisbzc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zwowouob.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2spsuyzed.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vmfvsdis.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqhepmej.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rulbefwo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cvfrozwp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2abdmrdew.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mwdxjmyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zjoibrao.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2onpitohu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yrldbuqt.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fqcwrnkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2gnavmani.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nxqjraph.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qaqqculn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ponfkmqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2cpaszpsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bktdeqmu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wegudren.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sszyxvhe.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2whyipubd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ofjmqteg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hptanllr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vgqjzkmc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tiaheelq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2vklnmkfy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2sduojsgq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fbpsbuhz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2engkgsmz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2yqrvnogo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2grlurixt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2nrxcyzlq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ccawcxbh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gsadbegu.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gxdirrxx.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xcsckftu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2jyuxcmlq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2umqlxuar.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2mxacugme.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2aktbguox.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xbcjyzzc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zvhqdbld.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hcexhngp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2gtdikizl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vqxyqhoa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqbewvm.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2skhfxool.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rwyhpzvd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihupefof.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwnguo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2mmbyjjxm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2mpzlpowa.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zapwzeoa.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtovauir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2skqjocdb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2knxmujbh.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2iwyoanfm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrlumgpj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ebnexnik.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pwjmthtq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2npjblanz.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2waxwqexq.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tdudgkey.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fdjakcwd.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2hmtntwsp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hyqbnitu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ysssqhux.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2yyoxcjma.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2cuccbpuc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2rtppjgpu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2egyzforo.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tyxfmoek.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2uggvqajc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2imzcazdg.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pktutkdh.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qwbfbghn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2arkrsydl.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2tntapwql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndfngezn.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cuhyvvpr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2emshmxvp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2yvsgtrfm.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2relmaoqm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jlmjwkab.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2huepbzil.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2snyufjci.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2dnfsjukn.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vdlpwqwi.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hlwcdlsx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2gklestgf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2rjkagwuy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yixozwoq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ntejyqdo.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ezswjjpx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2rxzvlqjy.html


<!-- 参考信息 -->