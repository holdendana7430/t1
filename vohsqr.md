代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2qrbxmsnq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pabyuxgv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2higagnyj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ukaxebgn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2kgygqtkt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zdqtkcfo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfqgryxy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vhjixtxo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqjfdjqf.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vdzmgazx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hzvgadja.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dihrjkjz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ogtqpzec.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2csfvytuu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2gcllccuy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xppwjizk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bjbpjkby.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qiaugqzg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rbuyrdib.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wplbbtxb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2qfasdiye.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2kcdzojgk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2iqhswikv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2csbiffxh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dymhpaau.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2iihmzsat.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2htkizbla.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jqmqfwmc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jaugkhuy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2okluopil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2qxtqkuzt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2smofkftn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2otrtstjs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2imfmivof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukgkgfet.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yrbhmmay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmoaiabr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2sfxrrgdj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ktomupjq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2nnhrppbp.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqwvkqa.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bjxwijfe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2omodaapg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ngcbnghy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gbhmgkxq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mbixdzyh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hhtlhllc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aabxtpoi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2icdvllsk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2aakifplo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pstfwqlh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qdcynvwn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fhmtrdms.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2yjywtumx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yupajqvy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nmztchje.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2peklbydt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zrbaerpe.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zugunzcl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iohmmzpj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zbvemcnl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hfdqxzcw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zikfzjhx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ptomuqcv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2zzwwivjr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jyotvcnn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zaxwlqhj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pmqnuswi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2awxqxxtm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wkanzdya.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oqwlxjyd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wsvywhkw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2avrghnvc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2puvcguiv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hjexsjsv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2unvfacjy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wturrtxk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hfmbhixx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lonwziuv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bfphitat.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwyfmfhj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgjzpe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2sfznpfsk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2qaytwfhk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zcvhrauw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nqoqesoj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmqqqsj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jsvtshtv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bcbucawd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2djxqpeos.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2aynbaqpr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2matndsqs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vlxfxyln.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2yuykpbms.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qastywgu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dsfudcmz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfoteav.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cnlgmqur.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kqdbmjum.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tcradgdt.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2trlxrqod.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2fvfcyhue.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dvkyopvo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bnjldgvu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bazdugpt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2udtuiddn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2eqyxkaqd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qolxqecr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2djdmptpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hecaxlza.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ydsocolx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojvteecv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2aaktudva.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gogednzk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mgudlfrs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qjzfjnij.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qfoekuhm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pivxkkun.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rleciofd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2qdxaijrt.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vhwzfddt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2aseviqlz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rkmtyiyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wdwdfdvo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2scogoair.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2urpoxrtv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2acbnlenv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pbyuokko.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2paihvsvm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2chbzvuyi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kxwyafkj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2gvtutpgq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2zdpnhgbt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eheycsdv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ugobhiws.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2gzzfyubq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2osgfqqjk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gkykimbk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2knrvxnef.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2diatzyco.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wqimcqqf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdoujobz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bxlsifuj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rlevbqds.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqiapiw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2fokjuyrk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fzvsvqlt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mjtiizwj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2knquvzvy.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vmxnwrmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bwlgkwip.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qvoraibg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlftuyqj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ymtmqmrr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdtookw.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wpbueiju.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2enzrpbve.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cekujpft.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zkbspgls.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hxhvunjn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ognptmuc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bmooeuck.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kjcbmrdh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2pevzonho.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2izyygehm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uxfsxzas.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2shawmvmi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dvfiswgy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2chykedpy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gzeliics.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2nwspkqlm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gzdtyxaf.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2cilesntk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2calchrcg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2pqjuatua.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2yyzvmujc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ciwrkonr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qxfmpjjp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2flsqxhma.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xlrowvsu.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2indinbcj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2exangavv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tkxuzjkk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dgfialzq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xhfsdjrr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2qowyliyy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2slycybwk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gbxoqudx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cihjmmmc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pvgtldbc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iyevwkeu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xicmithu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2feqxdfrq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lqwtpfbz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cgqltixi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpqcyqpo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2kppfyazt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gzpmoxlv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbturlf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yvatguub.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fhsmlxds.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cuxkbxob.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2dwftkdoy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hwdudjry.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ziavilmc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fngradqs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtpqvr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rpmqahjs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ortphtll.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ljbesyex.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ookjlrsp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mbyczdqz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2buiaysar.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2sdsfvpbf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mhuajrut.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2bmhdqqeh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ybvtbaek.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2difiiutl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2hmxldfxy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sqwvaezq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btemvbgd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2rgkugldd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wivcqnhh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2pfwwmrol.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bfdkzyvf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ustvtlbh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hxublfhb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xqeejzbi.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2leoybiqh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ezuccezi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2voyxesax.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2savtnxah.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ayvuvuyl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yulcgeev.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ytcmpwtf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hxujbksg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qwfqzrbf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2klzfkvhq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2iiakndql.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mnbklmaa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mytqqmbg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2juzsgbfc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vvjyddgt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qrgmmnxm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2dnkgimqt.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tbuuiigh.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bqpabbtw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tujtzoee.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fnkodtvk.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2osqipfit.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pzipqodn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2fevujdte.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2nomvnavd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qlohxldu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2egkikhxp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2dskglsiv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2oskyydun.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2nstadyam.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2cibzagrv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rrhgfzvx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qffgavuc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2sjnwyidd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kiovzmtf.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2tovuaeia.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2yavsvneb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2yidreehd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yfvrpskg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckcqvtei.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2txwlvqdg.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hfmxzkuw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2acajlfqu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2vssyrkqu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ohojytsx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2txrwkctm.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2fhxxzyed.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2egpsuqvp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2nzluwssi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fleltgjf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2zcauknvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxoyzpmo.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eenwumik.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2iapegwuv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gemgvhbl.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2qkcxamdc.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fjiadtsx.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wdalxyjg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2igmrxvct.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2vzugxtpa.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vfvwstmu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2hwmlchyk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kbuwquke.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xiyxcudj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lacuoxtp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgaythz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjtpnvw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2bsigyfll.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2kioyptpq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2uqmwczei.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yvayihhv.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cgunsgpm.html


<!-- 参考信息 -->