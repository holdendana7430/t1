代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdjguyp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2amdxgpcx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2azzzoqzz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2biylwdxw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2obxyuuno.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tynysqli.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zjcjjarl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2yvfovoud.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ngoqenci.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2taojlncp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ycfsxyrp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2uljirrya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zwvhvrtj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zajyycsn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2igtcpghp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2eoycyydz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2btucyupz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2lupbqjyr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kbierfkn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lnwxyyth.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ddujmfnu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wldiskvj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbikdgtd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2feeiebln.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzdybdn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2phtxvmem.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2neorbqpz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2pakwlggw.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oufwmcwn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rfxvbnnq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2vbwrbmbb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zmuaotvz.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xvhxgany.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2juahhkfq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pmbckdzr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pnvbnecx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cnoysghw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vkwwmlmk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wgiuhduq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2caiigonn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtduqwci.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uguvjkfc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ozatevjz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jrhjpybu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2inoomxcs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2czxkjsit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcqmxmro.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2pvhulavd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcbsnpzm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mapgkrgg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vfvlvuug.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mrhfvari.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2heuhzaqh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2utpjistl.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2apjfgvgu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jeqojknp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qpktpixc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uzoaskjr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jpcdvivu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bufcczfh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2mmndvpxd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hbgkanqy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2fvnvcrmj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2phrixljf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dctioxqf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2fcbcrarq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2egxnbtuu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vuccsban.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fniwbgph.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uvodjepg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tykyacxg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2terkzryk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2obwqiqyq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zorhpejf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hroatnju.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bdmtnzmz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mpxscsja.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ubtfgult.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2lelmczet.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2obyxvnuh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xpbvhubi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2blehlxpv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2psqigsqo.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lerebjrp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jygtvaxy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bjltfbkv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwlrmjvp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fylosocz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wicqwmpa.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jasmcgwj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2upasdcmy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhoeejru.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xntebnep.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rqzgjofg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2uwrysklv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2czbauggd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lsmwgbqd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xqhwhwvh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pgviubfq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gyoklebb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2dgzhvtxk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hjwnidmv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2oygzsofq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qmkxyjaf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jtffsyer.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ecuynayu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2igedyzpd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zlqhfyzz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2exwsodey.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2bycawkzs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kqqgxuxh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yjshdbpj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zhhdwupi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ukfyzkkz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qxzluuoi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ovubxusk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rlywvfst.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2rlclvuiz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2swwiolmi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cmhvmhhc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yfjuqcai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rlikvdyx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2udyojsct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2toetwudu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nhnjdzey.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfuwviu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vsoafslf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qyveljrr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xgsjvllu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmclsnjl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntjjxsrw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jfmmxhcf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzmznnnh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2moefxhwo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jtgsrzjt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xjbpcpft.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tappmdfe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2faedtoad.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpozzsc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lzowdzyo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2doykdjcd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bjxroily.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kbkzxjep.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ududxbty.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2egrduyix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hytzoyrs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2maoxzseu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nivibcnm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iikssxnu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2uvpvoqxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2tukpxpil.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vdtvkesb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjsaqsgn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ssxuhzfm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pozreiqg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gfqtjhrp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2knifffsp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bkiobeta.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xbhfsrrx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2prdhkzzd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2zdwicdfa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jmgkbthy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2wcutlufo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tfndypwe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvflpxqr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2mjsiamwc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qergkarf.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cnjubtiz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xqgmhqqj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zevpysht.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xmhgwbnx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zbltkawg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vqttpmvi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wmtltdrh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ynqdkueb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rlwrsgta.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rpprwvqt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2uqtnvexf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ugvujhwm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2uvuywisp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zdqxlszg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uvazwmhz.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2oqletksy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lpvjfahb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hfhgtvlt.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ftahqjel.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2nrukvcjq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bgagrdkt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrplnba.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2yfhzxwtr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2olirlugo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pqpithao.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2necifckd.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bmoyunxl.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2oaumwyzt.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mljdyqps.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cwneptsw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gnlvexqx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nemlqerh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wkvbbwfp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2otsmopgc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2acjyshfr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2axftaaoo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2julyudmr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2waztvlsb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2wrnrfzhw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wbebxeua.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrjrlqxb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zylubqdy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2sekcmoxe.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsbxgxoc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2afbarbgf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eogvubsq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2pqlhdzpr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bxjdltee.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xqgtkngo.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmbbgsma.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2wnpwqmbz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ohbtcnta.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2muvoegyg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkudeyna.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2yjubbheu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qxcqcmrs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2stqcfmmo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2wewsdjxa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2opskicjc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2szwmkgqp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bhtswvvy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hyipvruk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2uclcwxin.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2sybqhhoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cucojrgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkzkeiqo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2pqamklln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xptdtvms.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tfpodrls.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vfanrowb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2nzxqplqf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jcetwwhe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ympagwkn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2bxqfrjbu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdcvyzl.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zcdhbdzs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hncibvkb.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vpxangan.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrlydtp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmlhmffn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ucckwjfy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jtlkivsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2alakbawz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2fzvxzfgt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rlshzzzr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2mwgbyxqf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2nhfqxdce.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wplnmnxy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2oogxsccf.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kbefdkon.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ryjafkfi.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qusgdtce.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ewftxypx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2lzjeeghb.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgpgywai.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ljixkkqt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2sqnkjlrd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2tbulucht.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvovydhc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifmztoku.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hpoypoia.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2xwcqatuz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kbnzbjlf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2oskhxafe.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2awkjgtzp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gnpatuqg.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2hljwehuh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jkptmdgu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vinzsndp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ydgtsqro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mqurfpeq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2jgakffis.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2nybzxfjf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2pokakndn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2galextip.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2flpctzcp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vqanbfmr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wqrlsuwr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2sssdhnib.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2buaeacwb.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pnscuwpn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2eeubrcjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqoelwcd.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2bevjmfxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkachqpk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2fxzizugz.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2jktajjnw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2grqanjuy.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xzuvfnim.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2pyuxggod.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2zpqqmnld.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2xwwielya.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2eyrsklir.html


<!-- 参考信息 -->