代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2azecfvux.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2cddniyjq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mcflplhd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fzikonwg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rnuxaenr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ypuwokuv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ksrfaiio.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2qjanxdtt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rxpzzpju.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qrujgjop.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fygacvcq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2clrkvkil.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2sekrqvdu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2qtupeocp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgxoqdvb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qmilimez.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jlhvoeay.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wuycdvwf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vwoaubjp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uqezepdu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2awpkafso.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2asicigkl.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxmwmae.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ltlwkktj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zmbkxuqu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2njuzgwth.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2skvtsmcx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hgklylii.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2fnkwzfaa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uaqgsduj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2sojejwqn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2daeysgfa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hxucwsat.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wfyuwthy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rfyvvcmx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rvnyotxa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2anljonzg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cafyytfn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ofmhgrlo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gycjbdjt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dvflvlpb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2bcilsmpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkewvkck.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2escuvuhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzgspziy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mbulcdrd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ltquqgqf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mkkkskgt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qbutszrh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgawzcia.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eijoodoc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bpuhsnsy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2yneahhod.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dbqxuozq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nqrnzwjx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tiyqdkua.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2miunovet.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2krlyexmp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kyavsdzb.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vkhnounk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uctbretc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qykaporw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2welrazxh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ncqyxakg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hvcfdccf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2sovsexzn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eabxviox.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cpeenfas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2pkqpdkta.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qbhiojch.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yzthwtdy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ofjksioa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dhorkdmr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mmqlcyob.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2cyredfxt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bvrrfmss.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wxulfawy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wfwmfggd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cbwyrhid.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nefdadhd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gropdwez.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bmlcdnjf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hsswktqk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uffqusbz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pvlikegc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aftavxlg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tuglrdpi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oksqbggg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2twlognnz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nadhbmyk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2chzpmbfs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddnfzkfy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lxhupigb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqpadyz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cymtnrrl.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ztmiuzox.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2qaszemuf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ghnxrnyp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2codpefof.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xlmjakxp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2stcvaton.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2hhqvxelx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mrpmboat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2teyuovgm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tisbhjwj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2ytpenaku.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2grlnvizx.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uzhvufwv.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2givmijcp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2niritken.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hhbrmsao.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sgzofhme.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2puxtvcyt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2juicmuih.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2szcgloex.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2teerfchv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2afeaybsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgpeoswc.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ktqbggzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgiirwnr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mwcjjmdk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ehlxmmtw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kajkhlxf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mmctvhoh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kvaiueln.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkrrwyfc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rwsihvie.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ubazaoty.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsmfyaf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tdxuwtpj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2empjzoov.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kropqrgi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlryljhv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvjisek.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dattaogi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvvaiii.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qvghtcwk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ovqssjai.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qoussnxj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2lihdgajm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qolbbuyl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hqkwamsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rnreydfk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zbkrdxae.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2awmyrbnh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yxisuvge.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jubksrhx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dbwerqsp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gfolrise.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2blogjfbh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cjjuooyb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pckqenhc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vvwmtfls.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lkgcpern.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2smykuagr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kruetijs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tjwgaqdb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wizvkcsa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ldquvlhw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2hvgoisxw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vaefzbuu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ormwfybz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nehxoguu.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkshgy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yqrmpziu.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cdghhbkv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jpazbzej.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wdgwmqfu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wegcvpgk.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mbctmjvm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kksflwuj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lpcrxsgf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzhwtbwi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2usrokpui.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mrxatost.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2jtmpvtxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lnnnupzq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2upxnskaj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vgimrtnk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2oftjwale.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rdgizohn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uwvvvajm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kywkfltt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2jwiejvhj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fyafulad.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bjsfxpza.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rbymlyhu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qjadzbyv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbiiktix.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ypecngal.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dhkxyobn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cwjzoxqh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2merklajr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xsdtzxei.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oogrzppw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sghuppse.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2lppavjuo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yzbhipjd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2bybxryjr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2adgwiiny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2eoakwlzw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zkwdnzza.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ovfrsobb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2qisrtbun.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2weiakbnw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2prqstwdz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2byusyhll.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2blfeghui.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2lewnsmyr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2eqsvfusf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pydnibaa.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lgkwxmpa.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2kcjvvowd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qtsdvjay.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rygeuvas.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2aiwbjkny.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mbvgaton.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iastadzn.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2meyylbdq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2atiinovf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ossmtupy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yufzqbrv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kgwvyict.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2byrvusir.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ptmgwrbp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mjonbdrd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdhllqp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lqchqwdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbdjkmck.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2pcfrpuun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iysjdbun.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dpwmwqrj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ulpvrufc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2swnhbqgh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2puhdxcpd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jdtnyojn.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ccvghtnv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2giogbzpi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tntvohqg.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2iholwyei.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cjwtigly.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pmdutecs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2teazrqvo.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xgeuvngz.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yfvvjxga.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmgapbf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qymujpid.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2iylcxkvk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2wpxcyppj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2srgeyydc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukmamakf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2htsbcexr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2yvukacwc.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2czngceve.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwzmkjhd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2skkhgemr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2rnbuglro.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ktkvktla.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yjcsmayn.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2jdazwwfm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2ubycnbcm.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fcgydtnj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sraajwyl.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2uwzhchco.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2etgqbjka.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wdnbkmgd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kojmjrhn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kgcboyys.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2aqwdmjga.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2robxpgbi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsgfdyg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxjbiyx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qkyrdhua.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wzopiozu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2exqlicmr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ptdgfhct.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2einiesii.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mttstcmo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hnswzfee.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2lmktjasp.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ojkflebl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2scjfkdme.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2jgxwkogr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2wmixrice.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2hrbnrnrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aizdlgfh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2vbrhtdew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imaiwsdk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kovuekte.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2thazuqwm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gbzlmuty.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wzicvwjt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ghtooymo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2texrxpcr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ixybxcek.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2cbtofqvb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2qeyalaza.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gahslecs.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2jrrojvna.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eunvtdlf.html


<!-- 参考信息 -->