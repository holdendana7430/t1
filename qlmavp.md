代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3poafgaxz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wuvbtukj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zojnivfz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bwarhtkb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qpgiggoy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3hqcbjuld.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3dydrljje.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3pjfradoo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jxjibnjq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3klfqidid.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yxahklug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fczicjsx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zguujkoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hrqkoyxj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmaqyrcb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3npdieflm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xkmucgph.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rsnpbune.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3irbvcmjj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3xeifwdii.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmalpqd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3dneboqxs.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3oefitwyw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3pppgucvp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sikbdelw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3azzvfeur.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zivonsug.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3idqsirsq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3iogklszb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3dkxoynes.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ksteuxmr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uqqjilhf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rnwcohlr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rralsrlr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3iepwtizi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jeuyjvml.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ecszmlbu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wkulyndi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gpvhxpzs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3rknzjttm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3powwedcz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3deavhkrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsoedjit.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ydbrjprs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oihammke.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ooisqnhk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qgipjzxr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ddutaycn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nvympdlu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxtyqujc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cgjrmwci.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ikzqocli.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3arpshzqg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vnrxuggh.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tjojqyvt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fevhlctn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yzfbybzm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dxvqpzcw.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gqaamvez.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ixmqgksj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yxpfccbr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jyjodfvx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kzvxtmea.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3caggsuxo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kvauhixe.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oocswwcc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pseyppju.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kxdlvacm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qsrsbkzt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3jmmpaqno.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dziiuoaz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3hxquppfc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nyyffhsb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vmcsbksg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3nzfwfzrw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mblgpqqf.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zcigkfwo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3lznemupw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ykyfbrwy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xvbptuvq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3stwpkgkf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3rrplsgmx.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrsdllco.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mqolfptu.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nlitcmai.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kkekwurv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmalugc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kzbqwjjv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3illvumnc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xjuvccqt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3jqfxiyub.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pnatmlhc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vrvmxkem.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aabmvimc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mopgfiwm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dmenwdkg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3shkufyun.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ypeaofna.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3klrvzocp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3nbdguhpf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3frphvatf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dhxpihyz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ypxrqhgp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3fkpjubdg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3gferuinf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3atgmbfax.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sntygamk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ehuvxfno.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3pdivaxwq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3vnmyxdpo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3swurzije.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3baxkbpxh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uvvnxzjv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lrtpstuz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ahahpjsb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ycmewkmf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3zdcbmgig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgzshjrc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fnulblgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dnrtbfdm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cdpcijwn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jkocvvpm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmuwuoh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zcwonrcp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3sedvqvhw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdepbbe.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fzxjfrbr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bpeeciuk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyqjvmf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fermsfru.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vwiiyzeg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ghrrsaqs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rveygdmt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dbhjtrej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3nnysfjms.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aayracje.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rtxdrtsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3koxusmee.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3aiaogmfc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dwshydfn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rvuzttlr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3etwwotme.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xhfzijew.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vhsebwmy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3qbdbsdug.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3huikpgqv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3lwdjlmsf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3uldurgay.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qzojtfys.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnhiklfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xqyectrp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yvzlfrzf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fvlagioz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3yunbqgcn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fpoakbrf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lpxdvjdh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3cdoyznyb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3odmbshat.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cszerved.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ujvkrmic.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgdsjvlt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cfhyhyum.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3vbxkezmf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eombrysd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3pnbcfbha.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qbdzabkx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3mvecfckw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fgttxouq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ydhzhiuh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xeqjnveq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zjmqggfh.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3zuabxqth.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xoxiloxi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oyyxzowd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3orabswta.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3psjxtqwf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3kupvbyrh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3nukxgcgu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3dhqkajxm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3qkssfgzh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3vaxdwvev.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wdldwyoh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3nycfdhgl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3watnfyrp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3dmlcgcgb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3anknrkzd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ogiuekqx.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3myhwhiqb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bhruhosq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bjtqplyb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yznozyen.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mhgcrmbw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wzhgdjjj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bmwviuhz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mrwqhfao.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lbcjeqpd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ezocdbfr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3qgqiigvx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ankwrsgt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ifkduplu.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jkzxrwxd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3gfczqhsx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zjzichzh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mmibfugk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnoiszl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dyizcjhh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcuvyxwt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dtmyvjvy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3pcggzmco.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3owxuvrrs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bwrafpor.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ssgphupp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ffajlgwx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3trwrdhrp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gebznzgj.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqokfohf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nxqunqae.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3veokiipi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uljthkdc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jbvhrnar.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jvfdtkot.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ckvvoxgz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sohfzfuz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ekjrquvm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xacevrht.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3hpdgzfwc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3luphmtif.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kcnyouue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlpfkquy.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3ibptfsvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3molhesrz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ywsyvefx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3fjfzefrt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tnbngxyi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cvsfyqqb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sxsetqat.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rrvatlfh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kooxvybp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3dhczogtv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hfojksyp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mgiijurn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3cvjjeyzh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ivqziknp.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3nxtgiptq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uchfadqo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gidfsrxd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3lutqqicq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3entutecg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3rewuwnod.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3jpbemvcg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ghzfwqrr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3cyvmktvo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3paudeuln.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ejwwptea.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmxptsmh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3zpzbfesb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ggjkqzkr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3sjjznbzj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3rlmcwqxu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3iqqagstv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3deinmwsd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vqvzabky.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fjvneimv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3hqpfkkkz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3gqbcgnnz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3kgidfroi.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3fqfhonyz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3pbnorxlm.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3qyfzuhfx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3keccfhoh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uucruoel.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3insicdfp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3rcummybv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3zlbxrava.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3aaqzfxet.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hrxpmiyd.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3wzvdlpnh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tjyjnqcl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ufofdrrb.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dmxgjiuu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3soxhgjfi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3vlxwepjo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3kmknwudd.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3pbmwbkgk.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3nyqjdhta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejcivdwc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3puakapvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plgogbsd.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hwcuqrfh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3vqnknygp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3xpqgfppy.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3aplxtjot.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lxjgybtg.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mtftkrwz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3visrkdwo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3jwnkcuzw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rqujlucd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3hlscebkl.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3equjnaoa.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3rnvklinj.html


<!-- 参考信息 -->