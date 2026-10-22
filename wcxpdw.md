代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhviwh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ffrpcxof.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2arfppdyt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jhugzsev.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjapwbog.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2lvsanxuy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qirqipbs.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jfzdypbz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbgtbeil.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rthphzvv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fglcvtsm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tgzsfsbz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfwmivo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ipfayxne.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cydcxgxl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ordlzpfk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gbruncgd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xyvbvquv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bxuybwcq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fyoplpis.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hfhhomio.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2istclcij.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pjernqaq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2nhwobocd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rpwdbpvf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bevqmrlz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2eyvrbcad.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sftcimik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kwcilnyp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vqcczmvg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2puohhwte.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2olkcjvfx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2grjvrfjb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kejwkoqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpktodnv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2rarxmzjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuuisvep.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rfncfcld.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ldfcuhzs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cpwuetrf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2opolaucy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gsmmffcx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jfoqovnl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ecixrwao.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gdxwruza.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2glvqqiih.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dyspwlhm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ctjhbucp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2thtpxuha.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fnflpbvt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nnaxyhlj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xcbeopnp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lgxrypba.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kzuuinqg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvpwzxj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2srbonjxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kajwvhdf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fglrigol.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rtnvnkil.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzvawfbl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2oduojxlj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uhffztrb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mvllryvu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2umbttahb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uzodxciu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zwnrsvzl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ekelkgif.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uwgmfhib.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tpzolzbb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kkszhvvo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2arvhuosd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mfxfjffc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2sknhbzcf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2spwgedcq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hlmfctbp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wxvfmwnm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bkugykfx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkqksbim.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2sdaxyxtu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rodozxmp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ywgzrpsw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xuyxhied.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dvogdaag.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2zbtnqfel.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jgbfpmvm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2vdkritsm.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2adzbliev.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vvkaauae.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lggbejyv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qkyglcbg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lmnbjnkv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ovxoxrka.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2svxmqryk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2iivydtbv.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mullrxlf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fshqtyye.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ianulsuy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cnrvyqmq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2vdxhwsmc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2znahqcwk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2smaymuwn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xcztlhre.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xunaazhc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lltgainm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wfpopyze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2cquwbmkl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2djlyrqam.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tiilaqyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2wunnarff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrftinph.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ctshlukn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nygauwdx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2qnpqrnfa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2afshvxdb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gswxoyay.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bsjstemi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2burqmzpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2znalhdyw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2imyxeutx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cbvxumiv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2beborqiw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zcqoszkd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2welaibhn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2zekzymjs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2njjjlkit.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aitpmeyl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2whatjfpn.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcmjzgr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mhulibvn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bcxbkzrm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2bbyagspf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ftzrogej.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2eospoiux.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2niqrtrki.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2gmbeznli.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ayumkgub.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kkfgghku.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gwvxirap.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hzqucfxg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2twkwiscv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2peimoddm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2urlzkqqs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2umfmjfjk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ldufeceu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckhemqnh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mwjskmme.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbtpupn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mloakyfh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wmhqezcu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjdrfnap.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2vqhnlwfl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zhjcjoci.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2waviuaag.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ewtcoiat.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wijojyrn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ayottfko.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oftupvle.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2pqbwjhtf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kxsdxhjs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nboybdih.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jyevjolz.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agolgoky.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gwhdcido.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2hyqspjgx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yhfrxuco.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2yuyyoexz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2pedzbzdn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dnmryxgk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2xkjsrlwx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2feamidbp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2afnyxwhm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2onatakcn.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jqwwmbky.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vcudbulm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bdlvoikt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2mpsicrsi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vjcxjlfo.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jdjuoell.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pduhrsts.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2irglfxwy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rahmcifp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2neosvkre.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kndsiziw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qxharuzj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2czusoerd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fwmclueu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zyszowtd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wrcvlisl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2hhiofldx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hoeihdih.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2dbcslqsm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bzconvou.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2xqjbixqs.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2uqjbrltm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2fkxzpjsj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nqrqqxdi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2phcuyslb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyirfyq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdipthww.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2abgbgzia.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnuydgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mepntajc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2exztgftd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2skrgwkpz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ynyslspd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cvoeqxvf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2robevluj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lzbbuqwq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lrvpnnou.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tdnotrix.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqqsnnca.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2enhmzyja.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2iepzzhpu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2tabufirp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2egcrncdj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2euhwoiam.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zninpvwj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ggregyvj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xfblxvrs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2oibflkmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eceageua.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2btclirhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gknmgplx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2lvnfcqza.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mfpbjegj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2zdhgpfmb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2khnukuzj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xexrttds.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bivpcfie.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rzqqoguu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2atuykcnd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vjoarwms.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hscpapue.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pwvfwjyy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ieujkgpo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rhzhtnfc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fcvgjgrs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2wejuxlji.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zjdgetoy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2eduikoov.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2dkxhscmb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rwdeokyk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hjfkgelw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gbslbllo.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2dudkenlk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2bphtxpix.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecbisuwu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ejlybhke.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bheplcof.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2tmwkzthj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fnemexia.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2kkxapbna.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2atzrqibk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvwoirmt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uqpwtrfd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ssavxabr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iutjpbvt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2euizirbs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzslschm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hefepqky.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rmkhytwo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xupwgvwd.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2abhvvuol.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2haotjils.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kgcchuyi.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2qsfvmtzo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2coclqeaz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ofqpbxhn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2enazikcs.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gyycdrph.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2myppxgsv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kzktuxbk.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2itmdqawu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2mfwdavyq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2gcxraifx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2igaxbpsh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2dydyuhjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2invmcihf.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fgvtnrdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imtodcru.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jyojyfwa.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2sqzcgacr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wdywqjus.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2acmzeeyh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2webheavm.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gtdvmjge.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qavxooun.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2akikgikk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zdysymsr.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zdfmueuk.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kpykowre.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adhlwfpr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ukaoghnv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2bsajemke.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wesgshlj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sqwoccrc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2onoinepb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2iiuhclcs.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2brcysusl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xuhmgkzf.html


<!-- 参考信息 -->