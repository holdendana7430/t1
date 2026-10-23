代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qstkxdda.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ggoemqig.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mtfcuhus.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3pfjgqhep.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3jpqldajx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3amerqutd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hvpaexnc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jbbpgibm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eephgzop.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hlkaksso.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xedytxye.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fqoncozo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3phkqjkco.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3efyvohbc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3utpodssg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3snsnfwyn.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jklkkkcf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3xpnilhto.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wqqexzbg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cyekqdxb.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ucisdmuc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3iqzwedtq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3visnwszh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xtqsezru.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iuygixop.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3tdqzeams.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3fgrjyfaa.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pzuowuts.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zpdnaxty.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qdktqgxj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dxoalqkc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3odpzjtmn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3epztovfd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ewumiagz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohngzcwp.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ksblcwwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwzsqoaf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3farttslr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3velynxuy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jxlhgyey.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iqfumubw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3onfxixfc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gezxitwb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3qnmiumas.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vfgrwmoo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mkaspnol.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aqpyzodx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3rhorfcgt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jdsgjsvs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dmmrlgej.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3afzmouta.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dcinvhxt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3worxpble.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uwpyyaif.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3stmtmpgy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lcuymjvx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3meqaajbx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3klkqnoob.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xdhesipa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3owccqgmi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ozklxzwv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qxbopfci.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3gkezfqxs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3sovskzum.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wjfsucmo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3biepdgrb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tflnkwpj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tgmxmclm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eapiccjc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ziduhmsj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3yybkiase.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dkdosnrz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3euynkhci.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xutjxvbp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqhznaac.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cskhlstx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyylooo.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzeodgvk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgbmqgd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kfjqbnxj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tfmxkkuk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ypddauex.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3aqbnagno.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqrpymqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dqsdhcpf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pmehlgks.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gwpoywvo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3trhwlkzq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3pakbwvie.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3qwvxxqrs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mhozhnle.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rpdzphkk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gwbeagwj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xrdahtkh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dsnacisd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tebzeaft.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xgamunmh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rsvktjqa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3owidejnl.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3oufcpswi.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3oypyscgz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qndtmlpv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3oorxkzyw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vnjirkgc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hewxgtnh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lwlhvawc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wrdbqbrl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3gvqfqybi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3itwrnept.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erzsgtpr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kfqpbxly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xacnjufg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dgchvdlf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cbfeaovz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ryjekycz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3myjxgozu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qrmsmbos.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wttferrt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vggaezdv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3sfhrnvew.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ioigcypl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tiwasuep.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gblqyntc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpimaqg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3laxjkbmt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fvetriwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3pkzhnjzk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skzoyhmp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3beetnfxl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3xzparfnd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ngbxharq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3oovksrse.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3fscdbqfs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ffvaxvgk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kpqrvxkx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ghdnxkbb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jqfdggvl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3oqovfjvu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3lycdtdbj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3lfdpuzwp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuswepxo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wbqmkpvz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yztqomof.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nrmhdnjq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcmcbat.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3pvoykycv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muvbqisn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xfoieawi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3jewnlavi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ngjmqlly.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3iauetigx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zozdlvyd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fmmqcpda.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vueqnqah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hsiibrwk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3lcrrkjei.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3bbogodwt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nbfcwczt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ulnptaou.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pussjbem.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3brccbamg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fukfople.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3gerzndop.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vymjhcfv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rptujoml.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3mzkoulmx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3fepjbiun.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3wsudlyit.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3jwebhhfp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bxgbnjtq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ojfskrnu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3oqqiethy.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rmdzkyub.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ywgkypfn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3zepnfcgl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3crsvicyw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mmqrihoo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3fcjiqcmb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3foowjwrl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nonwffgp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vpfafcih.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gmbgkixz.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3rxpqpycp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qkpolfsu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kcfrjrkp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ggbpjjkc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfxnfh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3srfwhcdj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ltgkdnhk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3afogxfrb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gpeopayl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqanpkxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3omedafof.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kssmzaws.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3csiteveg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3aknghrxf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wboqevuy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3oyonnghf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3pjtzazbq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fwfycxer.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwhmikd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3houmbmrg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ggozpzqv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3jsmhvtfu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gkwuamqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xftbmkzb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3abprunzx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nfskgade.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3shogwcir.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3zxjfdeow.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3rtsiovsr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fmodevfi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3raudnjpd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3imjpqdvp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wmrcigwd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3axuiztnd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3swnudqvr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xbhwgqmm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jbzxolii.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hkmgicuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecgnlyzu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hlgyrpzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdwysmtt.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3jdcblubw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3nwnensdq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3fdzoaiid.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zwqndqdw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sficqhtl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bhqkdgkv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3szogeewr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zmblqsud.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3liunfwhe.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vlsmhqiw.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3tsovkxym.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aghyqnoy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3htrzupqw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3urrtopjn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3sckifkpq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdhoeo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3mrnhyljd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3dnnhgxhi.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3suzqbood.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3luhoclts.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3hhitepda.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mhbawxhu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ofjmiydn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ziuvqkow.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3gnucevkv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3eqiqmkvn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3uraqbkwp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3abvagocm.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nqrzygsb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ybhhkifq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wfusmbko.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3oborzgko.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3sqqztovk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mvitzzid.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3epzjujnk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubepygkk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3bivqghsi.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fltsifag.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3elmpgsmh.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ymbrmbbe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3bnpdivpb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3ayqqhvpo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3dkyjzbau.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3auymwkhy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3enxhgcmt.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3btpvmrtv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3wzspshhp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3yxqtwbsy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3xeyeodwd.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3qlmquuat.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3gpexaeco.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3qdduibls.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3apusncwn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3yebmvqog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddvyjell.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqhgcbwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpfncwwg.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3iduumxiq.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3knfrvugd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jxtpader.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ckhhxngi.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bhrixeqw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3dhbubwkb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3ptowoydd.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3lhtfwreo.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3jlvjpoxt.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3evnidexp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3nyiolqsm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3ipcbasdo.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3htluaiwi.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3lqelqrun.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pbvnsljr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3lbtuacid.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qnagvctu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3vybgqqlf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bjnketmt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3vkuusdfx.html


<!-- 参考信息 -->