代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbndxmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zlvoeqay.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uqqrikae.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qokunfjz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2cvshsngz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wurzmcuc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqcpyvlg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wehtnygw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2chnsvpgh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2oqhrcmmx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wbwszvzq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ysgrvzci.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ykibmffw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tvoftags.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zfzbcsif.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hjfzusfh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cemmrxjz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2aajhumwz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nfgonfqg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cmuypfnf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jnksqlyb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gdheimjk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xbxvoycd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2xrvrhnrm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qvtkdvcs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hqpvyjag.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pbvhvvbp.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uiyegjyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2escimkjf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjnbmodu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2kmwfxsdf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bhxmkzfr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jffydykx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2slqpfqji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmqommpk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2beqhvnja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjtvstsy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zxkzlrsb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pfxokjru.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kuiblaqe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tlnbbvwp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tqwsftpg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wrjihzbn.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wplihaak.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dfigtyrg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rbszkfdr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2uoeluwwt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dwlgveve.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2koosodtl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ntrzfytd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dgwsrnmw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wxzkkrrc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrnboh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2blksgmur.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tbehwlsn.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qgaehyhv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hcpexhpg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2epbezzeh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2pwrmdnne.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2flcocrca.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qgvyyvnb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lgfbgyoe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fxhkcykk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zdvfisbp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tsmnwoqz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tqbyuoat.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2fdpcspyc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufhlmtfm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2szothtqw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2outtbiug.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bjhmwmdd.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jrqedfzv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cbdqxojr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2moxaplvy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rgggjqzf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2klbspwhr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2algfqhjl.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xqxhszmh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jazamwlb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2brftztng.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2stpogzgm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2bjdmvfdl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2naieixmg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2sdibruir.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vghatqfa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nbptijws.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vcvoyjui.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wjpdgzbe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2huvqqawi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rxoihrck.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rordbamz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vbrjmixy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ccdkjblr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2phxrscad.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jrxrsgws.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yuwppnrr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2myyfvaqo.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wkasmjst.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vdhqwyvn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2afhkankz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sjnmeapn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2pcghjjwo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qcqcmynw.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2milogacf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uqbjmdwl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mpieykpt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qzeeafdl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2pebwwpnl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2kcjslacp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qszwvtkb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2llmtjmow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfbkurlr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xwogdrld.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dpozjzsc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cptmoryo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wygptcky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msdpowjv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wtgekbyn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ngcuwfct.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2lnwufazv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nidnaurr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dwvwwdkh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ywpxsdtd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xqdspbdi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzywoiam.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tyypzxmn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2apxjejhr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxtgjad.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vcudxejq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uffwhskl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gdllwogp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2sknuuegv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dlyjvrlw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tbngwksi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hadlgzeg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cictjiji.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2izyqttno.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ielfreod.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hctfynkm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pihphvks.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdabana.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2onvggucp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hajtdnic.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2alybwcao.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2maacvsar.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2uiyewmcx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bgtpkirp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nycefrao.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hejvyzqo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dybhswfo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wnuceuul.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbuzarnv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ixtmboxw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sxstzfru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2nypdegqc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zxqfkvsy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgsmxwrt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwfjjwmg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tfrdbocn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbwxoavm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bwnvtimf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zqudtpts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tlirakak.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cnuimcph.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iosdufzd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2shyjhoje.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2agygghqx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wufltgnn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rhypebqf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqdmzqg.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2igqemlik.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fagzkkls.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zomkahid.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pizkwplj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cjjcxmjy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2echpvsgw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jasbmysh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qnmuvwlz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zncfpntw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwaninpu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eihsplwl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fpapjjph.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wnyaevzq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2icjtjzct.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkhqocyi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nmkjvarv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkqcfywi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iromlutk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lpclgqne.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2alyoaipq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ikofnrjc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ijmvoght.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wglqphcr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2iaysxevs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tmzapgae.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2arqeqmju.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2muoyfotu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vneolfhc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hphzcslc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2slumkjqp.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gaqgdgex.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dgjyeqxr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dfrwxwpr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2inajxgjy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2uhdvsfxh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wjofjasn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2oupjotiu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vltleebh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ochmexef.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wycaktpd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2frzrrmel.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ghfzuxpi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dncjdmqv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2aqssaowj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2caixiahk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cwgokuij.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zqjwenqj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xpoejkcc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtzppsgs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ozqiheus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkibtnjc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kpzugbyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyplbfly.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2txubtshq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zsbdzfpb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qbewprkl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vtcrzyhx.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fhxiaikv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2otxioldg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2asesfaib.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2csduuyin.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2auniayca.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hxppdjkw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bfnrkenz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hhnbhdww.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cnbzrngv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2trgbkpmh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2hslhtqqa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2htggbvel.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xjockrsk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2vxwlbjgn.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fkwfsrsz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2vzcqgafi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jpnbqssr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2vdnrvvtk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wkaacgha.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2frvjgyao.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2quhvreta.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yrskbtxg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uncqvghh.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jaatygrk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2njpamuzu.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uotjxyvo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ddudkvaz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2wyobtigd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gtgfwzbs.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tfmqmwdu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2upbjgdhx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2dctgyrmp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lwgdjupz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2obaathpm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2emwsknck.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeicydv.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2hdfaoyjf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sztedrqa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2vxzfqbdc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhkmcrn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2dqldjzzo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wcugcfue.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wtmcephe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iaivgzgx.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2pcxguczb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lsdthytm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2oqqwfniv.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2bneftksb.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mfszjiql.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uzrkwwzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inqwjelp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2qkgzqkrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxznwvds.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2btbabcmm.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qlvtjauu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lefquaak.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gwwrzosz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rickztyj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jlpxumfu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lrhvesgw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2tqqehfjx.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kinroqic.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ysxdvupb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gubjwvbv.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kbdfyngj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vquaqtlr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ykqpltzi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2duuibrfd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2dyjklaor.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2jqdjukjb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2kifkrmrk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xzhkqafo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2folbamuo.html


<!-- 参考信息 -->