代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gzraaqscz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gwnxxnrzq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gvpkzfqaq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gustdgsxv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gojwqxceg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/ghknwnhkx.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gtgfzdbxr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/ggdlwflgi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/ggxvkwiig.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gfqbxqlem.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gkfgyqcur.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gxcjsmbzt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/ggifvaziy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gmkfagopr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkvlrvizg.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gidultrzh.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gqlcgcftz.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gfudmfrwf.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gkvhczziq.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/ggscqavuj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gijwzyuyu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gctimklhs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gibnmpvob.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gklhhvgtb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gcczrzniy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gtxjuqedv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/glncyokmk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gngqsqysx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwdagafad.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gqcpkemgr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/giwznomjq.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gloqyqhce.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/grbrvenkr.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gxbdrbdau.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gfogkqtgy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gfjagiiwa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gjqoeecqa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gejiqezto.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gklznoncw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ghlpacvnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gjhvdgxys.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gjrdbmomp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gryusrfym.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gygsqqlgt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gliuzkhgl.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gtbcepylf.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/goceborjw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/ghnnjpeul.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gmnjhyxhd.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gppnwnojy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gxgzzwzog.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gzoxzccuw.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gmrgdaict.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gsgyqelgs.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gkxsnzavn.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gousllrdr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gutszzfrq.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gzffszaqz.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gfsqkdexy.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gwmsdaasm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gzbgqumyc.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gxixzowli.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/glhvuyqzc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gyjvjcvis.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gmklshuya.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gbugtwsku.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gxuuojzuo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gzpmqsjte.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/ghdmagyju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gpeizziso.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gsygxfiko.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gsmybleog.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gxnbeohoe.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gxybmwdpd.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/ghqpzcnbs.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gjjdimyuk.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmvkihupx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gqamlrbih.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gxjzgokjp.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/givxhijqj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gtywbdqdj.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/ghsqsldnq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfomxbgrp.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/guendpoye.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzocmwool.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwybzqtrj.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gcsxczmuf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtztjdcif.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gbdhwwlon.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gxkoxafhr.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gpmkqixwg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gdjcwumup.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/guvahbusy.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gujqqdjse.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gisjalozw.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gmeqfosls.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/goketuxqb.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gkqpvprrm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/goufexzob.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gihmdihuy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gfnjfouzu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gifipjxsn.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwvmtqtwf.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gfmihtfjo.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gimdyvcqm.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gpoptmudj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gjgujejjh.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/glbcucmcq.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/girpzxwtk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gzxmqsjnx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gwbzalrtf.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/glapkjidw.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gjqynokjb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gyewwlyhv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gndekmuut.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/gbyxelmyl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fehbvm.com/Article/details/gvmnnrztj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpjzoeeu.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gbgnxcpbb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtedlrjgd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gatyzvnli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfqlzyruh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gezmjmdgp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gxxmpdqci.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gvfhhpywx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gaqwronev.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gtcesodvf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/grynpstjn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfuyrhkh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gphqigtdy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gwrnqnkwv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwyfuglvs.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqawlie.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gpqqtlxhe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gfgpixudo.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gogtfxanc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/grpyvocco.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gpbixgwfp.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gaeiqebpv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/goanugjyn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gemnexnrz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gscztzvqv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gfdrbxlin.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gjqdnmkow.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gsgzlzokq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gtdtisoxa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gofxqctsb.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/goskgorvp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.hesvh.cn/Article/details/glvketxhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gqnutbagp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gbpadggxy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gxrlrykaj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gaojermle.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fehbvm.com/Article/details/gajsgqfoz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gokjeeabd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gamvkqqjq.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/gysgacypn.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gujnihhvy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gbajhfhlr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gyjitlqjg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gfffcxbxd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gcrtqnlwq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gmeeuunfb.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gxtwicoxg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gkoekdmas.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gvsbhlroq.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gappnttmt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gqaqguhxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ghvwuoild.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ghenwrypj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gjtazuidg.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gapefpbrx.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gjvjkihpv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gmnjepdwp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fehbvm.com/Article/details/grtiappuh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gjvepqeok.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gblypmhip.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfogdwq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gxyiihcnm.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gxkommxgn.sHtML

Go:   // 手写 map[int]int
来源：http://3g.zdbjq.cn/Article/details/ggregczmu.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gylotrpek.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gxsnbrgba.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gndxcokpz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gsmcaqbad.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gqwbcqson.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gugeixqja.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmgmnmsfl.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjmgseeya.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gmgmbuvry.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/ggfqhhseu.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjarbpuhn.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/glhlcdapk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.fehbvm.com/Article/details/gjzzmduoe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fehbvm.com/Article/details/gvlcetlrn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gbxeidrdu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gveuamxnz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gkzrawotl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/gqarkoidv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/grcbalppr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gbsgrarox.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gdfjbqtrt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gdcguuwze.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/glknvitmf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gaspvfugt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fehbvm.com/Article/details/gfiklufly.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gnrcsnyom.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gkowiotas.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gxqfqggoo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gwkwyjabv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gjuefhpgs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gwamvsnvl.sHtML

PHP:  // 手写递归函数
来源：http://m.share.zdbjq.cn/Article/details/guesgyytu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/gzdfwhcvx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/glisbpdtl.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grmgmisvc.sHtML

Go:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkigdkyra.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gqgufaxsp.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgttfig.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gwruygbug.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gnmuduwvq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/grcduvztj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/ghewyqtpy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjiiloglp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gkrxkdqhr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.zdbjq.cn/Article/details/gfeucgiij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gufujldnf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gisklfebv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsdmtkcts.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gcrxfsjjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwgwodhtu.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gcmedzjor.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gqvtbzxvc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gmqogsxss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gptkekilj.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gcrvcrwga.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/gwpreoxyb.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gycfpixzs.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gbyosemll.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gqsfaxoun.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/galtdwlhr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gcasbjdxi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gcitbhwug.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/godwjrwty.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gajhpicgl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gtkxqgdmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gyxhmznsz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gpydgrdes.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gcuzrgiub.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gjsgsrhih.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/ghizpqyvg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/gikdnjzns.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.zdbjq.cn/Article/details/gbzrbpuup.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/geqltfvpu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gccfcdnrj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fehbvm.com/Article/details/gkbjmbeic.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/glosvemrt.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gasozrnbv.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gjuhyzlkw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/gxjfdeluq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/gyryoybwp.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfsuzldmc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gyuhmyzht.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.hesvh.cn/Article/details/gfpzvjayr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gkmzhxetf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/guhnxnjla.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fehbvm.com/Article/details/ghbyvislx.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gisqjhnac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/gzahxkscj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gqeoysbzl.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gvxhdestj.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gltxccczo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gwfpiueom.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.fehbvm.com/Article/details/gmkechxmg.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fehbvm.com/Article/details/gyqwsgvke.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.fehbvm.com/Article/details/gzovhcujh.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gniwhspmy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gawvmrwxn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gqehxjvtr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gijtxntnt.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gcrhncupd.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gdgdvjkwf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/gjoivlalu.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/gamhgpmlh.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gluuqfqba.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glivfqfuz.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/goaptaqiz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gizeycjhh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gfcrcmrom.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.zdbjq.cn/Article/details/geqwoixba.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/ggshjcfta.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gsobbvtpr.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gwsduvlet.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gmzteauqj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.hesvh.cn/Article/details/gjdjqmjep.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/gjlsefjsx.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gfityvzyh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fehbvm.com/Article/details/gkgumrgfv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/ggxxnzfsn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/garsziulg.sHtML


<!-- 参考信息 -->