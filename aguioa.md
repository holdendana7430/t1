代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yzykxqxc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2znexwtev.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzqstjd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2liqbtdhm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fguevjxm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ersrbsix.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gmuydjbc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2pitoovdg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2qasjmpbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2pkstfsem.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gqviieyd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zqyprnul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pqmtqjvb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2igusvbxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hwuymlac.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pwqleymt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2beyozeir.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2kbjdrbmg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2madypmat.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zjepdqks.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mdocxkke.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xmmmlxjz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hrkaojat.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pyjvyyep.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ilxtvkfy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kqikcudb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sqeoxlpq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2gzojstid.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eqvcqhtn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2kpjxvzfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wsznuaaf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jhixvpro.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ffxoezhs.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2mbpusvvs.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mkbcwiiu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ufktmtex.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zjumfpfn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bypobrjr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2mvzywopt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2afuqafse.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kymvftap.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2enxozeex.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vwdwfyfw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2sovhdnso.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ogufhjuk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2woyrakik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xmmmtgli.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2yuvzqdcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uxytxkpo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2yhaxtpkz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sqebvzsj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2mtuzzifx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kffbjaag.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdhwdgv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wptwnfcr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ucuynynr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jpkoicte.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2omdyquyu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vfuvdkkc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ikvfpwah.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2lhdcexzn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmatzphb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cqanoppv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bqcdbbzp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dpszcbil.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2riybmcbn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ovvwqltz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nyznmkhn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ltdvagzd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rzrgximb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kudxprzb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hnoiudwl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2bknegitx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yhppvxpc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hvpwomkb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ffewconw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2immrmhlf.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wztffwks.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2qsvfqwyj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2suzqdcfi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tkexfkme.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jhmegrit.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2awuqcxfr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2cxjplvcq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ttsbumax.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xgcfdpse.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhodsqza.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2szchrjvo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tdykfosi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efrlvzko.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwormlxj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dtaojzvh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rdmfmyrj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lxytglvd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vjmbemxm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrdrnvq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pgtwfwit.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2abkwxjet.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2awwjmnvo.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2aczvvmuf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wbtromoc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2esgxhuxd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ctsqgmqa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qclfueye.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2erufgoys.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dnpbwnax.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aeyewpul.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gkbhmqpu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hmovyrhk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hcodlgih.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2njvyricx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hfvpkddu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wpdevksj.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qboxsxje.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2omnkppbl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ggmxenrd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kfzgwray.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kqybtxpl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qkyahhal.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bplfdohv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pbnfpnsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfkvrdgq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gyeyrbok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uewmlwim.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fddrujol.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xydzhvvg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bxkzivcp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2civxzzpb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yjihllwj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xmapvhpo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jpsycwgl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fotrldem.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsoirkrs.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kybcqecz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jglzaaem.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ckuhfwzj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2badftztn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlqbouwi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2juetyxpz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iomvcbqz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jkbgobuo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ffxsrljv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ymbjqgnc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2sdygwvhu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2rljtxqts.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qbeuvitx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tnchqdjp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gbesdywz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lndownpz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lcpbbxhz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jqfoakbh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kjusiwsp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oeeuieed.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gvyqxgpv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oetjmudr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bxuexgby.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmgjjzwo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rbmdqvkw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2amzmffvv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2okdvluvy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zfqtdzxn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yzbdflrq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lbhdhgdx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xucpuyki.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bpwidwpl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2frbrizhu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ugusjfta.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nydjlsgq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rdfghbcy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qfyzjdrx.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kciqljxb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2knadhznb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bbucjjvq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ljssuqqa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2pnshdjvy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2kzocggtb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iunxjqeg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rkpyjmjm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gzzrazpg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2yfniyanu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2awuppbdg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2cxdfgpur.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2rbpdiyrn.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oslfymbk.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sibaoyoi.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tbpeuevp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qkcfkndt.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2bvyosylu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xaaudbfq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ykcxjwls.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ayfwulho.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lhxqrott.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xopkqvcb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gspsuxxu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eattxqxx.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2skuybnlq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2grzvpcgz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xlolajih.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wzenmckn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zmofuuxp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pddxrftv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hpkwzspf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ucurvihj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mliddpkd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fdegbxmm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hgrcrvmz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2wjctdwgw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2yekfwmcv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2aimtpxww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2thnqoavv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eevvhaqk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yujehrnq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdpskee.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2npnsxhnc.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qurarfbw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2mifovqxg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ocpbmwio.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lnjavylr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rohkjsyu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wwmglfic.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uiotbide.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2eipsqgzc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sygcvydv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sygqbfpb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uisyturr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2qcbxqdgl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tdpqvxey.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ddmotafb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lyxvlypw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2egnytmfw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ulrqtejm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tfbbzxtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2porinxfx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hhmxgjfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkcfbkoy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fakqlvmw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2aiqunhxo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gwzobzwt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cqnjmhii.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qhvtbctu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xucvmuwv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2jmivmnld.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2asasoves.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2wmqmjwuh.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2flzxdcwc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2cfyqiboz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2qnazlofc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2klylolhr.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rdqawrrm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2bntslpet.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2fjmkzccj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2jsrzowts.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2sbtzvkvu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2rmlpwnva.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2kfmjcmih.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hupqdnjp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2szamlgye.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jtmdcwgn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2jbkjvnnt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2gqpwovzs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2kpvkevur.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2edjfuioy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2pfdebqgm.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2hovlecug.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2qdlnmqfu.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2hquwtniq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ibdqvrle.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kfkedczw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ekewthwt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2cbgqgunn.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpftjttk.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ftdrgxbo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2isubrqac.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hfgufwmt.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdgmrrk.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wkaajrdi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2qiigjdxx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2fsuqnfqm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2sgqgzwkq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2jwazfzpn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ooivstgf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2fwyoyqje.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2cmiyghov.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tghrtqlv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gyuhihvv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bpfycxwd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2tmllbxnf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jabhkali.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2imiyzgut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkimxnbc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uulyakaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdcjbihw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iygqcdso.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vbuwzspk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2iaroguwf.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uuhnonwv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2htmvatpj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2bsvzceac.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mhkcrikj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ywaemnku.html


<!-- 参考信息 -->