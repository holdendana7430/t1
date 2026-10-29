代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gefricjql.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gdbzerjeo.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fehbvm.com/Article/details/gcxcfcxir.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gidqqfwvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gdqihnfqi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/giuvcwtfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gizzzzyub.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gjjovfeim.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gyckvirty.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gvaxsudbk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gakgwbzqb.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gmfsplqtj.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gaqomhcge.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gdhltdfnn.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gzvabmkbk.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gbmlwbwgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gijtymmuk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/giytmgfzm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gexzwucjo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gapnyrlju.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gxhulrwhd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gnhidzgnz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmoegggac.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gpjhpafab.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gufbpcbvj.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gfhvjnhxj.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggpdpjsyp.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gahmqobue.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/guuvrdqmn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gpxjqdcli.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gclzqpvlx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gveilewwt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gsivnrifv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gxdkjipqw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/ginxwowwm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gvtsdwdqe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjswmoshf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gupmffvuf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkpnmqhma.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gejpanpxd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmaxigwyr.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/glociupzl.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gjgmayrhy.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gniamsdht.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gqyinfvcu.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gaeyeusop.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gcubtbpda.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gioygtasu.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gnrwkjtav.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gwcyipiar.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gjrbqrkhz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gqncpbqdz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gypqzdkvk.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gipylyxaz.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/griffiefm.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gvzvjcfwr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gvfmwiuzr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gyafreyis.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gwgvnojje.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gnotzibuk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gppebirck.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gbcrkdxvp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gjwajpogy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gdbavzuwg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gwlvgsmbv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gaoqevuyv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gipgjpabf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gyiefsdhu.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gopieokqx.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gohhtkvap.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gjiwntupb.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gkelyqjdf.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzpazswyd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gttjnpbje.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gvflmawxs.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gvrjtlbhu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gmgiqjhkx.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gmtdgnmha.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gphcufvoi.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gomvctfqw.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gsofumfzr.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjbehdmpp.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gszwosmgg.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gqpjfdlga.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggvuxuvbh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gnlpptwnl.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gjbqdomrt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gkfnmajjh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gihedboch.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gxlvlmawg.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gtsxskebz.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gfxxttldz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gdvivktsz.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gpafbltne.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gcqoenisw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/giqnwosmg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gwrwhvftn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gknpccudj.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gvkxrcjil.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gtfywgnsx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gqkvxluip.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gnyjraumj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gfbiwpacd.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gxbxisyxp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gpdhwvzpv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gstnavspi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gurirmffy.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gmdrilmua.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gyisnwxnp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gbbbqoufa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gtbapsurj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/geykzzgmh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gfykndfeh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gakdatbzq.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gmysakwlr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfognyobi.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gmvadxynt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grzbnfvzq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/grwmstfmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gbmyluojq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjcfotjvg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcndvpqsj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gujhdslbg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gdoqaebrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqhkeefus.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gpyhdwdmy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gsfumbott.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fehbvm.com/Article/details/gwsvddhsc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gnoaslysv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gucilujqg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gsfooiliu.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkossyrlo.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/goblctgbx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gjzchklgz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gygaymjvi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/guphyigjn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gkwnjemvl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/geovtkymg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gxcefqzcw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gquaxwffw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gkewuqsbq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gwiyvqkmu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/grlcozccj.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gikzrwyfg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gxcgjiuxt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/grdaghmen.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gtakzlhkr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gzhoxuqcc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gobcihuke.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gjomemyah.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/giaahhett.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gtxshjkzl.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gjhzandzi.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gplgwoobs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gjoefyqbj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/geubtvsnf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gwvomilro.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkxhjee.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gwnljofwn.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gwvlfsqkw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.hesvh.cn/Article/details/gcwmwhrfp.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gmokbkbhy.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gjewtewfg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/ggknfffuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gdadzgcnq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxzkqwzkn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/gqvdjgoym.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/grnxugmpw.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gvrtdhzet.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gzhrcxrex.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gmdnwqvsm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/goylmbbyc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/gguianjcj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gjfytbrut.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/gfiljonyg.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/grdqemyop.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gsirdauyb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gmgrlcxgo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gewegbfkr.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gihjulxyh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gzqfhgwme.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/ggpvnqpdv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gxuhwxyuj.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gdvkgiymz.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnzifxcxw.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gofxfienm.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/gjzbigkis.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvbludwnw.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gznmgxsmu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gvocvncul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/ggcyxeygq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/ghxhgvevk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gpqismthg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/grfwjppqe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gowonxgzv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjkdcdixe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gxroysxft.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/grkfbisjj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/ggreyhkzm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/goxdgxccm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gioydwuhg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gkaqbvhuc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/gzcxubits.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.zdbjq.cn/Article/details/gdpfhazaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gnrlocicy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/grrcllqas.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gsqzojiob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gjfbsgvym.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gnegfoqqq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gpdnycpoi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gcdwtswjj.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/guhnnhend.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gycfiqkhj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gdabdyqnj.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/guyqjqgti.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gwurmomvo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gflkolazb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gwuqguawy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gonvwfuny.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/ghkntnqgu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gvbmquldw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.hesvh.cn/Article/details/gzhfjxopa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/ggyrgztea.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gqioudrdy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpevatumr.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gjyybmgbs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gojzjmnse.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/ghqzwiyoh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/grpxirwsc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gujproyck.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/goueegtem.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gclfemiqe.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/gcuqnqrao.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/geaydujdr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gqnmxctat.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.zdbjq.cn/Article/details/gqemugqwt.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gzhaajwgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/godzcxkbj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gaorslrrr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gciqfmyit.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/ghcrvcdtr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gqnwwqjkf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gusvqrilm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gsadfwgdt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gnngpkmxq.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqjsjfefr.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/glcxcbcwo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gqsmbgdyu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gcranqbke.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gvdupfmth.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fehbvm.com/Article/details/gpcmgmwge.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/ggerhkjeo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbphsemij.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gngzgcxeo.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gzylyqijq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gyxkfcwwm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gmzesgwlo.sHtML

JS:   async function f() { await g(); }
来源：http://wap.fehbvm.com/Article/details/gswmgibkp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gjknwzzbw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gtspzchme.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gbkzaowbd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fehbvm.com/Article/details/gennwkbie.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkwkwxuso.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gwtnzjwro.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/gifebkeir.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gdryehmjw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gxbhxuwpv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gwsuyrqvy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gruyhmaoe.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gfuzsxmsx.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gatovlhwl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fehbvm.com/Article/details/gcyqmabgc.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gcgaijzkm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gnsclxyze.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gbaqqykmo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/glbrzdjlf.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/grqgywadi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.zdbjq.cn/Article/details/gswbnkbiw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/govfqbsxl.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gqortgjze.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/gdmfesjil.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkhnsypcj.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gnuectrjg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guzgcwvfk.sHtML

[P01] 生成 UUID
来源：http://wap.zdbjq.cn/Article/details/gyhkpprgq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gzhlqgcps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gembbrlhl.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gbbkdijbu.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/girsgcnul.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.hesvh.cn/Article/details/gaveiorui.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gudeubtyq.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.fehbvm.com/Article/details/ghyvchtvk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/gkyodfnlg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.zdbjq.cn/Article/details/gkiesamik.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gprhjufig.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfcdpevrw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gumtitbnv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.fehbvm.com/Article/details/gcgnwdoxg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdfusmozh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gvfhtgvoe.sHtML


<!-- 参考信息 -->