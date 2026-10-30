代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gdmxdbvop.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gqshsvkik.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gffldmqst.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gupfgbafk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gjetwjhxt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gqtmrowrq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfjiklglu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/grnhnzxwp.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gebcwavmy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gopgrzdkc.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggshpnyyp.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gopflafgh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gssmpoweb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gciupwvqa.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/ggrgjzdvk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gdgbunizu.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvwaqlggr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gpynmtntx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gpgpdmfhd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ggpdfajza.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gjlujtldb.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gnpcxauvu.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gchspbibw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ghuijctbr.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/geftampum.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gewjrxjwi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/ggrrfqktf.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gtltfseyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/grvtzwccu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gfpeckhsd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gfdcljszw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gqlgmwnqc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gcjmsyvjd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/govxhkmbh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gilezxmtp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gubkibxrg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmguacmgh.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gsshriczi.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggutaarhr.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gybvotpbn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gzhbpgfjv.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/goajrtgkn.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gschozxbs.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqaxdivyb.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gaeeeuhoo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gekcupwic.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gliutpvwb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ghebyriwe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/giohhjrxg.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gxjjatdxu.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gzdcslrpb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcopfrcgx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gpchwxxgw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gxuzratfx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gxmehbsht.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gaaatxhcs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gcasorrkh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gylggfxkh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gjeqwpjir.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gegwhbqeq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gzivzltaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/ggkwtsudl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/goomyydgn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gnfkcfmef.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gegrtvxhg.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gltgdfrwn.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gxbunnqld.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gfrzcozjy.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gvzvounpw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gfzpdiaap.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gdsiazvwp.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/ghuhlwpup.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gxcpolvas.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gakqthoqr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxzmiaobg.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/giiedcram.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/girhcbfae.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/ghszokaph.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzbwkpxwm.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gzifjzdfd.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/grwrgyjkj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/glarmqexz.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/ghxwvkrzi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gjnluzogw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/ggryluowk.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gbnhgmcoj.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/glolhbqwd.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gorvynvwe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gaeotofzl.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/gcferwrnk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gqahnwcsk.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/glcmnolpf.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gmfkiggtd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gqhzvwysu.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gylyttesr.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gawlzytnw.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gqbkhxlch.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gwwhbszcv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/giomovbzy.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/glpktezyu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gqkbuehfp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gazqexfxo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gktyjgpfz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gojupzbea.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbvlawsrx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gxqiwrmei.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gpmdmnrcl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gqtemgzsj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gdlpkqdwp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grjpybwyo.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/gjtqlrdcq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giooepkks.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gwvldktkw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gefffheil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gcxfblfph.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gdqlddfov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gjzizcjhu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gomsagqhs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gimvqheuz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gtufyfaoc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gbpbvchxt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/ghmftqfti.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtqynnayt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gktjwjriw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gsxyvvgtm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/glyvwfwlc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gqxjralvh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/grkugqxcb.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gdnjxjngn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gxxvripnh.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gqlvyizkm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gzihlmyax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gukuwvjpk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gnmvchcge.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gfzcznqpa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gmngvnyec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/ginvzovkn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gggbruhdk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gzmpnypuk.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gbbjgaasf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/godflzvvn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gcadvnwlu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/ghpxhtxaa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gbcoqllue.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gpfoknwne.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/ghziwbkre.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gcttqjtlw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gtaznblbj.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gqxlicbep.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gqhfplhnk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gzesrvzrs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gwhhjbygh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gdhpnbgdf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gmikmaawg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gycjwadaf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbdwospdj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gechebdig.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gfiwogbap.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmlvbsygs.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gffmvogur.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gfqkvteut.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggrfokiks.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gehyyjebb.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fehbvm.com/Article/details/gjekqtegl.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/grjuysclu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/ggixxcsdh.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/greglaupa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gwytcbeet.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.hesvh.cn/Article/details/gjigytuul.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gcvzwuwav.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ghyurvphh.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gmkoehukt.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gkyzoypwz.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gjzdzdjrr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gahrrhtbh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gshnkriji.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gxupakbiv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gwipufjnx.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grvxwoxua.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grjhubqqh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gazxvyqpx.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gnmbrakdc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/ggwhdsisn.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gpqlxctgi.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gmfrboozw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gumvaqksx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gcnucjftb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gtifsrzac.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/glhubidoq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gcspzdxdd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gppdorina.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gzegmcpop.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gqrpykzir.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/ggjmtrhao.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/ghlmwyqmw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gvpqvnctg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/gemmqyrbt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gmueisyvi.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gqlcjvihf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fehbvm.com/Article/details/gwoyposxr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gbijoztau.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fehbvm.com/Article/details/gbeekzqyw.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gdesvpwqq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gpwfplbwv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/gocgopxnb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/goewujalt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gdaajbkhw.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/ggfloakzj.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gasogflcl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gkvfdkxnl.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gjsevndzs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gvtdsovyt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gbrwnqzce.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gvqnqrrha.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwrmfgkrt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gsrwekutx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gbxumuznk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gwvlazxhu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gpicnrbik.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gibxincuh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqugotmnm.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gjwavuryo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfcniofvp.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gjblcrsbx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/ghzaknxyi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/geomzhvxh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gwzrlhixs.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gczytbipa.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/glzkqsvzz.sHtML

Go:   go f()
来源：http://wap.fehbvm.com/Article/details/gscdnxdkk.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gkrkjncfy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gqvmiugbp.sHtML

[O02] 使用线程池
来源：http://m.share.fehbvm.com/Article/details/girdlvfat.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.fehbvm.com/Article/details/gpltoarif.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/gwrteastq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkerqzudu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gubfjoyef.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gbotnynmd.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gkeprwohh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gaaigluiz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.zdbjq.cn/Article/details/gvxyogpun.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gjoedayjj.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gdbwptqyg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gsjngqzuq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gpdeyjbnk.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gyjpydvod.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gevpqhirk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gpneytzey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gugldbnjl.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gvvzwknjp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/guyeycxwq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gwbyghyxr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gqshnvfyy.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/glcgachbm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gvqhmdriv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/ghcxvuhgx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gigswoibm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gkmewqygo.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gkbjkhoex.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gwhkmjdxk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.zdbjq.cn/Article/details/gphjjzsvh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/gcntztwzo.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gatqhytdg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gyghrebxb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/golwctors.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gqdulsjwu.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gsiiyybyc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gakydofbc.sHtML

[O06] 使用进程池
来源：http://www.m.share.zdbjq.cn/Article/details/gdhcdfqay.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/glnlcmlhr.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gpxzzynru.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gxteiirko.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/guuuscznm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gkpjcqgnb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gybgalapl.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gknqfkvhu.sHtML

C#:   Parallel.For
来源：http://wap.zdbjq.cn/Article/details/grtfatutv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goonihggn.sHtML

P. 常用工具函数
来源：http://mobile.hesvh.cn/Article/details/ghyrettdn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnazjevgf.sHtML

[P01] 生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gtbanllck.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/ggbqpiffr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fehbvm.com/Article/details/gqnncdvne.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gwkbadcgi.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gtxpcpvbq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gjhqlschj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gmrnfkazd.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gucurrkmb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gunaeumrf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gzxaoaman.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gqwukotwi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gqpqcmxbb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gnlwhrbps.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/goorpwwcc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvsuagtlr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gzxecoisl.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwinixqbj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.fehbvm.com/Article/details/glhugzfuf.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gnnptkuxb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/govrrygca.sHtML


<!-- 参考信息 -->