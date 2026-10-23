代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ahyiwycx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3upohiedl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cwgmhutm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3cqaftnzj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nuysidhy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tlihlynl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3aevmlkwm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3vifujbse.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hchkerug.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wllwqiol.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jljyvblx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ssotlqhm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mkdjltqc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3oynekwvh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zqkoywnp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tsfiawwr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kkkasgvb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ekzlstmn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xryadclm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jaqxbhts.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3asubdcnb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ufokujsb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yjvgcsqc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ecvynsmb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ugddfvez.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fiwogcye.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pouyculf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mcqiaroh.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ddtrutmc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nlbeiuxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zsncikkm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3rmptilqs.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yqzfpzha.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zrfejxdx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3hlkpbqcc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3ywfpcqhq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oxadqjln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3spvwptpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faxfrmdz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rmkvizqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qkzqxrug.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lfjokyob.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3syvkpvmj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3icfleqfm.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3migqifxq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gvkofgko.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yxanwkml.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3pbjxkhuy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ongdwjru.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ansporgr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3yunyxhxa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vmqptmdx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jajdaisg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nueugzjl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3knesqctx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eqifrxuo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bwntshek.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3aqhhuauc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rfwklnnd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3njofrdta.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmtacef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jfqpnlxh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yfmwtfxu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oyxnpsyk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mbcososj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lbkceycr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3agvcvrqw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gjnkcztm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zjrxkimd.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3adiorfjt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3btcxjdtz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fcozynos.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3tdrjpckp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3dmycutdc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fejanetv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mqayzooo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3afssofhj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jiqkagcu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nusqptvz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3sljyebfy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzcglht.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hawdakug.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bbsrhehg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3adxmppei.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xtywsabn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jmdckcfg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3wibumdzu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhjmvzg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pfogpten.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ezrlcazl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dnrtpgjg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hyyztanw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jgwtdmnh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ogxhbblb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bwghjutg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3tbsrlbqs.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3kfopynli.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iolgwcel.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ysreokou.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ysqpiygb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3wuexsomk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3labtjvrb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ppowsddd.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wrgcrmia.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3etazoeyo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3ersdcyag.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3omruxgkb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rrdnnoiu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aswoaoct.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xvmezrwf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3jvfmyrly.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3sjkbwskr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3aqaozbps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqnziqcc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3bjpbgjaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqhspiwr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3wcjyvzpj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3opfugqxi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ihhhhkix.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lyygwivr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kkxewqkt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yddiwkff.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dveubjqa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3idtpmtjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkoceho.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hnqzinqm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kycekpzb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zhljmsni.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrttiln.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mqsgmrpn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dmaemnew.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqqznbmi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zarzkcwk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pzgvxkmc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3inyopgbk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xwbfkrtx.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ispllftb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3vmdslqur.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3tveycolj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3gaewlvvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ksdrgvyq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3oyxfrqxf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ksmrlxxe.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3mjkylqlt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3prwdunjk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3geqdyqmc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krnnlorl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3kkhekump.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3izamajlt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xxletwiy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymjgjsbq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3avkzkano.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mlmwylbf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zsyulayg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaamgkmd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzhvqtzt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yhcvrhpe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3pmaxvwcj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sdfkafwx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzwnvmze.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrzjbalm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hjsirbmw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bogyotfx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sfvxtwgt.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bbyscacv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kvgzzkks.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rwyxvfnw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yltvjhnx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zydrcoph.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lfpxvpqc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3lgnztfbp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rvtocget.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wkbgfund.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3znnqamhz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3gjdcwher.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3koteidtv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hpanpvnp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3afzuaoge.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rspyyxjm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3lpdddumd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyafvmdz.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3tgbuvnid.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3phoqgttg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3dtywoxei.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3aeplgdqj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nmpqlrdl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3crhwgoiv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vmrqvqsk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wnsnivli.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3newomzyg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zheuqzeg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gczxmwis.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ecreqnga.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3cruarjgj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3tkqxviul.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mywspuip.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3cqiogseb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3wvkpymbh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ksrspngi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3spuovdvx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3endshsxv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3hnljnycz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ukqnzhkk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3cmudxvaj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3gvqptgvt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kibxlizj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mwpdwigo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mzsgmzxp.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ztacekkl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3srypegon.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zjhqocqb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3vsqdgbrs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rlujyzny.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xwzkacjj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xzpdslsh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3snedrldv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xxnvrhwi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3spkjxkap.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3resighnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kzhgiodc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ittblvfz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3bncwsjou.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nkphquxf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yokxveay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stveqvix.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3kyeiogng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3envrbvfl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xhmlmexo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wgholvzm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iwwxxsri.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3gfnfdzig.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xoquhvqg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3gsnmmiia.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3jilogmct.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3vxorqtwp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3dutaczzt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vkkrolxu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3vnlxkhxa.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ngqagjsx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3oqatnhqt.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3ssgyfouv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pbqiojbt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gjiiqufg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nwrrwxol.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3nrmzwwlk.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3dapknwvr.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3uoboxkli.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fbpvqmvb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mvpkvrul.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sgekgjgh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdxhuik.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bwcijnsd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ifzuonvw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wxznstqt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bnzdczqh.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3ugrngyxs.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3nlcsmqnl.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fbbabadd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kqpzmdhu.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3lelztkyb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fmzntoqr.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3njoavzsu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ddsymldm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3mqyochkc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3ipuuhmjo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3oxamstau.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3frczaarg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3gxofqznv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3egrlwdaa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3naqytttg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fmbwmcsk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3szarifmj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nxigsgnq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3pbeoedfo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yxabozhg.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vitdqeui.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rzmazvhc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3yocwfyty.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vxycawto.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3btpxtveg.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kysakdwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdvveprd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3vecifvpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zdlkqndm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pmmqasvg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wsfhipnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3sibeuidz.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bloqzoik.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jtnfihtw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3vosepchu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ukyejpzx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3seomrikc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yiozarbi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3jppbsxfn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nlkshoie.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfmppdpk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3mnzofwqy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3attoqbex.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yyklwwao.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3zoiuuvez.html


<!-- 参考信息 -->