代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3vivdczyy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ljxmuaht.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ddkakrsr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rudypfad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lxmlikhg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tbhsrbba.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zhyfjxbt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vnhtcpxi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3guqcliev.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ttmhmabo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbwsvzox.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uitcbomf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3edutjevw.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3lhwcfmoc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dbqpaywi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yocgzuqz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qrdwzsju.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kkbuceyq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fxvqcuns.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cxekfqcs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rfwxvauf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3icjrcomc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vujjavee.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bmdfkygh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yjuumayq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3tmzkixuu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xtgmamjg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3bzaaemja.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ixignzyj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3szdbgivm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3sckwjjnw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wwgckhwi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bfdhxtwm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zjnzuqhf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3zoxkhwwb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tepfjcaa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hzfqvlgp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jfrkvjdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hlhkepfx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3apnxxdmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvbhbicz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tvhjbjzp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zdibubdr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bmkuezwx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3uezoznvr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqvtpgk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kygjhcpi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ypdxvlte.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3kiqhvtpb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uckcxjsm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hitvsumt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gfttdvnm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3peribxlv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ceklukxm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bofaamiw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yzxtljwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zkdxovqf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pcspfstd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dmxemsca.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cpxpfubx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3axdbsnqa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3braknbxp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3egirouio.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fovnsgpu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3luuneada.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3sxsrvrtc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3eyrhvvmw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3lvzykmrg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3haxtosrd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wwbfrnqy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jpjylewj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zlpcdifu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wdxjfyzi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3eicaxqgq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tbdftvmu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3qvvedloc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xmxjnsbp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3uownvvbj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oceepfzt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tvsyxxka.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyucmqlu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gorejenu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwwevnnr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtlsqfgf.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ridktnjr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3arzfdjrm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3hpvtnqxs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3czcgtxuj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3binwavsu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jivbojka.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3syjqesvp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ffhrbdct.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cjdbbsxm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3iodhbzmi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3brjziphs.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3gmleqsts.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kxazldgb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3alooqbpa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3epoojrzd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vqoddmjm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iwwxgmed.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3mouqdjzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3huskrvgl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qewdnulo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3vmsceajf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wshlzgxc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dzwntbiw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hvvlyzwf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3oiagtuvh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3itearoqk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qywdvhbn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3tckztgjn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tigjqrjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrmylxyk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3pgnmzdad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyunhogk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pcnmmqog.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dgkmnyhc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ucyzpxbp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dbqolntc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oiqteaab.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrbnrcy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wxiwjznu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3hmpobntx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zytowwxo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sgxfunzo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3judfkenq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3omtpjjhu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jqxgfbxj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ftomnnbt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3uopxouag.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3isznbgqs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3boutdacg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jgoiizoy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kxnctepn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gxlbizgc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3ozfbcjwl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfefwj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3wiutwkdr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ufrtyxga.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yfgrnjtc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3clqnuqmi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3kfdwycun.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dletpldt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjvkin.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qnmxnoar.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3otpocabi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3uhaviodo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3nhylcsdl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ewvvdoxd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlidjrxx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wzalacpj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3twdhxonh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ikgzscnd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggatxiyu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmxtxnnj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lfxunttg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3afvtnshd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pphloyao.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rgzknjad.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3nofantar.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3atslhumh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3prctlnob.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3lgscjptm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wbwjmzvk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqrexhyr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ybnuglqj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3tczjdfij.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3upttebto.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3gmbgwdlo.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3jnaieayz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vjvdflao.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ugpbxjdt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3hbmoghsv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ytlxvjmh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3hkipbpwe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xjyckkum.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xzsrynxm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3momxtjvk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3yjqvjgwg.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxywxhgj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3gxysnhfk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ndqncxio.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3osgaxfhe.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rjhejwlh.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oaekfprw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xerdyqmi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hasjyxcj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jrqgbrxl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cvkheael.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fxubvnnc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3smtdiezb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tdcjlthx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gdafoqhg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3wljecdsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tyufhgbx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vrbkyasi.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3bofurvua.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3bcmjkckr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpvkzugw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgoorevo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3kuwdgmji.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiysjvoz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3necqzwxc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3eutpeysk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3wqtppqkj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tjkfyosn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3nlnrgdgo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3vvjdkjbr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3rrpuzola.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fsxhzzua.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjcnfdwf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mywyyeoc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nwsjjzpq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qwoznuow.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mshynvxg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3eicyauda.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3dqoaabqq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uignzdzl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3eurcpdfh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nfkttctz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wsgcucie.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfcewma.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3qurgvfpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtwdcdss.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3almgwmbh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skzdrkyq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3yyxgbrzd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ljejqkta.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3dhvpfscl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3dnzvemqc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vacrguro.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3hlfgkzov.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bpznfrku.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nimqbtqy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pnqwwipf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wevatqan.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3hlszstdg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3rxjsilbb.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cntektkd.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fhiwbxdt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pgfpqfzf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bqxtcnwx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3vqsoxhjb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3ywoxvgaq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3ivvveexs.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3yuafbmyl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3iifrsbvb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3wuikhhfr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3dxmhufga.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mabatizf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3chnurhuv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3doxacjlv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3iwtokudf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xurirdnn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xuxukerh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3pohfnigm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmgmfqxi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3qrmiwgag.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3wgnxmkdm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3nmpqvqgi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3pjavlkew.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3pwgytiur.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mtuftlmx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3dttzeklu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wjminvkr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzdjeta.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dykqcdmu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3slukgzin.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3tsdfgvov.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ewdigrjy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3qidqbxrs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3krduevbi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3jqxedrcj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3wbyxnjnq.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jfxziuts.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3cdcemqby.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uzamylti.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ulegyqul.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ymfssrxp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3myoeddnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsrudgos.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3koncwjwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frdamdjm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3xumjhmqk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3vtuhzcbx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nycvreio.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3oirrpevh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rwwhctrm.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3fldeacmn.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3kefzaqgn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3ssdjolnf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3sautngso.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3czfqdbsk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ctthdpzf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qvmacjzm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3adwtxwzb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zvfugvgy.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ekspwsoo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3mxgiglay.html


<!-- 参考信息 -->