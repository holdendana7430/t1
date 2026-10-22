代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ybiinzqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oeybjmry.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ctrgjciv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2obvhrrvk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2cnkldjbx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2tbdazmxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmczqohc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bjnrrdbi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zyakjbcl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2uanzkpoq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nwycwcvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ycthqwdn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tplgodsn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2iatgcppf.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2itviucdd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2eimukvcj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2luxrtsmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hcwnjpaf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2geahpuhm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uwdqzuhq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2luldjccv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ksazcsmg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ezjawmqz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yhubudoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxgtvcm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2adgrjokg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ireyxcxr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2joaoncbr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2imwalkft.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jbayohnk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ycfyxdek.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2pbisfuey.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zdpshkzc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2prvjyepn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gqtkabei.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pwvdftiv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrxgpjq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gkfmspjs.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2tiyeljhe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bdsqyexk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mcsqdbqh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mmbkpsba.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2frljtzoo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pvbyqqbe.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yyvajatv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fvypyili.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2xonohaqw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2rohsvyhq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qyicefvi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bjueddxd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hccmzkql.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zizgmblk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ehuyjqld.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dbwtrdit.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lltmcuxn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2smlubfwo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zjpjplmw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ylqjvxhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chstrzvp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2riizryyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bztpksug.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2gtfrxzmt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2yixpxalk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2nalaiuqu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fwsfengd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vlhnjfof.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nqkwxryt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wtamqryj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ofaumbqp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wsmklvll.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vdlkgsyw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2onzfjbdx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hhauilel.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hbzbrbnk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mzdyxcko.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kltqanni.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sqqbhcei.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2gygpishg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bqimpfpk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qvlzpqlg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pgjelzsj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fzvschci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lflxdqeq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yajgsego.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2odnqoxqc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kjnngsuk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rbqgnqbh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2btxkthux.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sbiflrvc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2axahbguw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2axhoaphh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ncdoytsj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jxgvsmxb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wgmrekit.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wujlgwgt.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2krgypvjk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2gscqdvws.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ndpmzrmb.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksysespv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xolkmzzx.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tfzkhinq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pdtdlbvs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jguhrllz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzdhxqe.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2pjxualdh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2evhtqefe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zputfrpa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2anuixilt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2crmtriyr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2abnwpjsw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2sivevtrn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mfitjycp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mybntlyr.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eeskmsmq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wwbbzdze.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2shieylfg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fvkzscec.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tjysdtcp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lxcrnsyb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dwcttpzg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2fkylqkdy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fvcwtdgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2csnwvajj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2svxkldxp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2avecacgx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ltmnflpx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2plrulqvz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bxoiqfor.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2edfkbhlg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wqxcdqvx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2kmfnlzfe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2gyamitii.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hammytfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isixsziu.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uocaiyfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgchixzw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ayfywnyf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uywaywuo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gaaxhecn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fobtqaal.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ctjoxzgk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fzgjvclz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jsusybvx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2srfiiutb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vasjbncj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2komfkqzg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2upkjeqyk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qozlbpfz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pnzanmzn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcymvxud.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2uxzlljgu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jgnrxsyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wxaidpxk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2sqosdfww.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ismmxlph.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2pduytysy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mwajlhep.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2shiswcuy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qaeasqtz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqnmloww.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2rwjkvnba.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2opjffisj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2tqtfuvei.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wdgrkxnc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjgyqvh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ywncbdwg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlqmysgg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qnlmegdx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xfmijvfp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qwxmddcz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2twvbecgq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2movgkysf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jkhzlnxm.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qyttjzlk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2czbccqtu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qanfcauz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoshwwtd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2foaetice.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2njtlkywq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpzhotx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2onotyxcj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2conhorpa.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ybuxxfao.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2maxwrlnh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qmbmgsjj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vkxfxsqu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2flfbidct.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iisddyor.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mwddrapm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cpiswypz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qqwryccn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ntxqrjai.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2qyjbrtul.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xchwlvce.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xllhcagc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fdfkbctd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2vghxdlmd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2zploctlv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2orjulels.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2smqqnctv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgghumw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ewqplboq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kzvzytwv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kbicqydu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2voadtyci.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nmzcarff.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cuylxicg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mrfxiujk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ioqgyqkf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2srsptdks.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xleugdrm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2irgtqepz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2otoafopk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ozomqaul.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2klzzkrjc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gsljkhpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2htxrfaku.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2imekgqcx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zvjegglk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbaofgp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jvecnzhm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2oxbqzovy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2xoxrzkiq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ifuxrxla.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2aemhzygf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdswpagx.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2srvnbdeg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2juddfqae.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ikjfhxol.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bhzpluwu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rozxyzue.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bepjstpx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wvrbrxup.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pwfyixcj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hsyjzdit.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ilvyntog.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kloiuvbc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2otfpkztd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xkzsvtmf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jtlvmklj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sfckfccc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fnzqwodf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gerrjqgd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kvjschcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kegstour.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zrjvwjkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtnyospv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ttxihnsv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kcnbwrir.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2chfcwnws.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2trixenuu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tfxbhzkm.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2qdhnywna.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2tqdgaheu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tbgcljqq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2eetndgaw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2kpbgaaxb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2lfrkejzw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xrzlybzy.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rrynudzs.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2cankjqpm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gflnfuhv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2zkzdqhoe.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mqbevyml.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2skrfnrph.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vtuhjqvo.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2wuodxfbq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ygqthwgi.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vmvipfwn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cgwaatij.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mmspgsmo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2pblkwkbr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjgbqoet.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2bqugwfih.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mwvzvisr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2mxtxtneq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2pyayaxoh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2atktlzdl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrjpemvy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2sggmxfna.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2dsmqxhxw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2tdlbkbjr.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kguhmeuk.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2cjjzxilv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2admcktao.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2lcsysgbh.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nviyaxfy.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnwbuyp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2wupyzner.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2zngozbjj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mygvvpmr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyjdhsk.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2baijykzm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2phubqjcb.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2uhodfqng.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vzjoadaf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yajhllah.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2gdufndjb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rhdebeoy.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2hofasbya.html


<!-- 参考信息 -->