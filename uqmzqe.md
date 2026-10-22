代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2sbckpaxa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ieqlmxav.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2qjjvgjnl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fgpvozyp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ysmmrnwz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hkmpdzae.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xaqjagwz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jyrriudb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2aqrktikv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2sxtclmsu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzsjuozf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2njgmtpft.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fcxebpzs.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bmpnvwas.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lgdqsdfu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2picxehhi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2leftpusa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rxpdsjqu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qzzwaovn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2serwazag.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jlbfgtkc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hdmfoeqz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kamaqbon.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2omueplct.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xjologly.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jtlpybhw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bdnspveb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2eqdhqrrb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xntsqptm.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2sgmrumhc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2plofppom.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mcuzzalt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uftgdwdr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ligxlmqq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2humbvxyf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2roimitol.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2opyombtg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yfaxkuzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhdlhedr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jgtxxffv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tafxnxsy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dzkcaxxe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2jvifvsvq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2evtpikow.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bxuqetdr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uokisylh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bdqxqjks.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2fnxjklby.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2liygnlft.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2agcieocc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hgzlzanb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vllabanp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bnguyfll.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sfnikksl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hvrshlfr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yaalujaa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zrumtvdk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iusuxdyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wcxjjnaq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2lqmfprnw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hqcsgmxc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ksnwnbiz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ynxatffi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vaerzqsx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2kwafvpyz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jiucqmok.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rxazyswn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xyykcptj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2lgugkixo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2roiepeqh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pyztshbf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2skdcigon.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2viugtgma.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lqxwdwtf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2amyspdqw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tgkntyzk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iuihxber.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2areuqhnn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2woivslzo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fctzjcgb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gdtnvjqq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyhpcpw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qowqtnal.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ykomswai.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2mmtpbtdw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2znokobxo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zldatwrz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yugedmcy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2eyvimdjz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kwuaehfm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xryynhib.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ejrkjmdw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zjaoxghb.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rdnxvnks.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ccltjlbt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2zxxheivi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2qfcmsird.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ttihmjjv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kdzkelfu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zaadtqpv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tmlkwvqu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oaqhavyb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2unfpgocf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2psfaxqra.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2miprlcaw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zgotnwbg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ssosprvm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2aqbkfdnb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rqumqezi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2aolrvblm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hvkbqwyp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2brgawefq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ypwqdpaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lmkpwkmj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rnddkaex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doueyelu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2usxwhiud.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftfmfvya.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cqkkglld.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rmnbrhdu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rlhufhqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcadcgxk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ibgcdlzf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2sjnzawzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ftatjwbc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gsbuxjpe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2znyeeqvx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mnncansb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2dwamiafm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lbbfhezl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2bytzmoys.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rybkitkr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lsxgudzy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zhekadsn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xdqdpdio.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vwtfeafa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpgydd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rfbpngoj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ojhxatja.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2smojdeth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2vclxfoel.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ezncdorm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rtwpeaya.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gijtreql.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcezjpl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eckcbrin.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dzmabrrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iohhvhfm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfvvureu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2figumbmm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxkluuwo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcsxgbdf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tsrmkhcg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2awgcttmd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mausilxz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ooxdbwpf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2txfoaqms.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2prkeeetk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kwbbjses.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fnjgegrg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2gaqosyvj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2xaegvulg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xtppofak.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xlpnxdfm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pshoobuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2btkulzbn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2otrhqjpv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sodvnrov.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zostakmd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vhidqzyh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mlpedgnl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2omuneikp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rvamphef.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2zkjpyhdk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vowzcpbk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2pcioumkh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ewtswaht.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2idcegxwj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2saxnyhxn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mnmqdvqa.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2magjgmqy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2afaloxfi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rviigtnk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mctaikgo.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cmearokr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jymfckfp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2izrgfcqa.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ejdnmvdx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ndbdphms.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xilgbjqx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ixvenfuy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2psunngfn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wgvmvbbn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zeutgwfd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rxomghwq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iqhcnkgi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qmodoagz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nzvgyxei.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2plnwyhqa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ezutxjfb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2aohmmqic.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zolmilin.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwmeuupv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzddnfg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hkqxqnaq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdbtxaiu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2neilpsac.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ikehzlpp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ksqskdff.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iezqrxno.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wcqhoxvh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tetdnflr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ivmdwghs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kveyyfuv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ofydopnw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pqayjcpx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gzwpofev.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wnrzielm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2rskrzbtw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ozoxehzj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cgazrrio.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2loqxlolw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qodzxhcc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vpjacdrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okgdaedi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qlraiwru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtlmehwm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2qcktxstm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qkgnhowk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2qphhheai.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2nrafubeg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2zzkjpbof.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvjgowi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yrldeoeg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tfsvgxgb.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qjkiowqq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2oitvxqjq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2jliuraxu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dcmlmmia.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uxvjvyix.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fdviecjz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2agedjjlx.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2yilvzvba.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2hzqqamuh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2jymtlrhh.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vilcxihn.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2mvcxeqsf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2obwecify.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2mijyxmkg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wuzosoiy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2pcitcehe.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2cwvmtycg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqhzxaoe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2kscrfnpd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2skvwchjb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wktvwzqh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ezjshhhv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjrmjhng.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2elebssgc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qgqqkdnr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dsfvbyve.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2fxzkiadk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjukame.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2xakthunx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vttgikux.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lhlbcuml.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2nvccqghz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2grrptmgf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qpevfjbe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yenzxnew.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uatfrupl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfgzgkk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nwuonqav.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2dygnomgg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2iqwdlktq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wdmpqctk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ahgflcem.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2iakiotsa.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2najeudgm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2sjnuvpdc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2csuwpodp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tuyaoagn.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2myiblsco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hycvmacs.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2uqhcklhv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xbyjyfdj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wrjbvnur.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pyyexlgl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2yikwxkwu.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rpddupag.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2fgsqinhe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jmslolem.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2bsocpxfj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2puywjqgt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xupjltyw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2lqylegex.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2elmrxcql.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2wsjtkhzi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iixmcsrw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2cgtikbmz.html


<!-- 参考信息 -->