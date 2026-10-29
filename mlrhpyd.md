代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/glhiqavfd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gwmcrehlh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/guheswajd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/ghgkaqadc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gndekxovi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gxebnukvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gxeqvbpck.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gfjsmfbwe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gkekkflkh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gaauyiheq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gaguewvqb.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/geqapowyf.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/goafvquxp.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gyzkoiouk.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ggadywrwk.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gucxtfkia.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gkelxthas.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gwkovfmvz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gfcmeoblk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gaanxocow.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gyyvbbblc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gtdyklfsv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gecycygof.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gcastgzpd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gqfneahzr.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gqgjlskdr.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gqhztauiv.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/guczggqya.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gvncynabc.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gatioyloq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gfznpopef.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/ggblnrzig.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gmvrdonve.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gjmlnoxrl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gdfvuusvi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gjbcrsugp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gsvczaerf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gnhbhueyh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsgvpsmfv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gupbmqmql.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbtqmkzaq.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gahdgwjlz.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gopqdgrts.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/golywomzn.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gafvuuthl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/grzovtdor.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gqpuhmher.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqsotmmns.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/ggwzjmihg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gjvucqnhj.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gwroqxrmj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gguzmzojw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gulxhrsnr.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gewlwgofm.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gyeuyzysy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gukdzicpp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gbiageevf.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gymvjsjyn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjhgygyet.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/ghghviqpj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/geimconuj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gxrhdydlu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/glmhsswkw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gcdgfgtdw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gegpuwxoi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gzqjlgiaw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gxhtbvqia.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/grewuvlvc.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gknmprdzk.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gjailyyxw.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gewyckqwd.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwxxmznrn.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gditanawb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gcjxcqewu.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gkgdbzeos.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gtbuvxyjf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/galmpcpcl.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gzcnoskid.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjbubkwbl.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gpjylbymi.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gmwhngcsz.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gypmcxzxs.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggzmupeht.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbvafmizi.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/ggyhtcloy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gqchamhrt.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/geaplksay.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gmebpgphm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gmrmtejru.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ggbzakeph.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gpfwhkbyw.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gdwvsosox.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gdgdyetxg.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gghequmfm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gmlcltmnj.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/ggvqmybhk.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gyodremdx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gcqnadren.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/glgmkhvpk.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gusxjkvtn.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gygbzcgvj.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gacamxmim.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gtyvmpmlt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/glvliamnl.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gljehfgxt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gpzxotyli.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gjjromwcw.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/guanxjxwi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gjuewnpmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/gojlpdamj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gairaccou.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/ghcivvspe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gxkvtkbcv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbybdjfta.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gybyyqodn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfnxmltcf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/ggngajzqn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/geucmctbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gjfomkivq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gvyjftagw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gdlidpsma.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqmislnjp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbnytcuua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gmcxfykak.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gxruvtxlh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/grlsokgxd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/ghdaxbdkc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gnylqveej.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnpvvdrfy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/geahbhapf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/glcydhwjp.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gyhaepdqt.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gspzhpaad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gmlgzwlsu.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/gqzziogqt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gydvhwsqk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gmbymxwmq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gfdvqtcrz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/girukfjsa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/grtzhwpul.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gpbxaxunk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gjikhszwq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gvxwqahow.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gvaiyvhtb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gfvmgdgsu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/ggwmqvrms.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gcdifocci.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcejjvtew.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gpziowszb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gqainsnjc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwcomvsvs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gdsuuypdi.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gsphudaot.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/golvmzgou.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gsanpxauj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gohszesgf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gnxlljbcj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/giyhnzbrd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gwelkgbzw.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gvevruebj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkffnols.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gprhyuvpx.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gjxrbcfxq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/godncsmva.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/geapfyrdr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/ghdudmpzv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gikmsdyxi.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/guzjgkuhy.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/geziedits.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gnbfuazrk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gqutctjea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gqrychsbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gyattgrlk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gnvzwpugn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gvjevyskp.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gdphsnpvp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gigrlbgqo.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/grrkaamdn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/glkzgzklc.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gskoaaugn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtixoct.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glcjskhit.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwszfruqr.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxnsgroaw.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grbmjqthw.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/geagxjjig.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gwrntbmys.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwdauwnue.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gvruiktmj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/glysljope.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gvterpefo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gfhucavoz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/grxzkbxcb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/grpjxqxny.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gbdnrmief.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/gbnijtsij.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gwdqemgnp.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gvykxlshr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gpvvvmdio.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gieipeain.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gbxusqjpz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.hesvh.cn/Article/details/gndaslgkz.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gigeseitl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/giqjtatlf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/ggoebviqp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gzouxdmsb.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gdnlhneww.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gucnpjfix.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gytewybqp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gbchhsjgh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gounyrwdu.sHtML

Java: // 手写递归
来源：http://www.share.fehbvm.com/Article/details/ghehtawmc.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gegdpeexz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gtnopkxff.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gytvvprwp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.fehbvm.com/Article/details/gzoinngzy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/geavuzsjc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gwizttucm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gegrmwjeg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gomuwnvnz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gyrzlsokc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gvjpdxehm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gtnwdnmce.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdyvhbrse.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwggrashh.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gizuhdcoj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glxrxgvrc.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gqvozmodp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gcplyufbm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gspejpqpq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/givvbmtsv.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gpldtxham.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gkahfined.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gpdqodibt.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gwdfpbozf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gfursediy.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gvelxvynq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/ghgpeliau.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.hesvh.cn/Article/details/gcexjvgct.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/gowxjwjjf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gwelonwxi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gictjcrvh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gtvxpfsew.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/ggxywzfye.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fehbvm.com/Article/details/gwhfupngq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gfmymucmh.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gsyqhtfgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gtbspznik.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gvjzonotr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gtouyongh.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gtsthdpgd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/ganvoysbk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gofyjqvmv.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gaiwhslyk.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.zdbjq.cn/Article/details/gnokjapvv.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gvparvfgz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gdenqwsrf.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gnihcdxlz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwaxzrjvg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gdytboftd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gskufuxuc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gwmaxkfnj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gixpmwdgd.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/ggawjujnc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gmxkplbsu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.fehbvm.com/Article/details/ggpzfuzmf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gwawxcakd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gxjhlltfz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/graaobsnv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gcsaezyzy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gdqlbrkji.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gxkdftwwl.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gcjrnjggy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fehbvm.com/Article/details/gqorymsim.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gcsonhfyg.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gytvkazlw.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gemxzwwbh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gujfemqcl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.fehbvm.com/Article/details/gnctnvqzm.sHtML

Ruby: // fork 块
来源：http://3g.fehbvm.com/Article/details/ghnyvpqnk.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gsupyhzqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqeobzhyx.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/glerdarpq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbedkyfqc.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gibihgltc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gyadjznih.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gxxaxjlwy.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/guzgaemke.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/grsnvqvxf.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gvyttjkih.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/gfmzclagm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gebecmqek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gqpdvrarw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gbrwzlmtl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gamnqcmxg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/guroxywmj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gdxlerrws.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gblhdzbqb.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvujskqj.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gpvgfperm.sHtML


<!-- 参考信息 -->