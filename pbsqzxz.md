代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gdetrbbxc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyfokydce.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gpeypalzp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gufwnnfmj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gjrsdwzjy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gtbvnamav.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gjpkldlfp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gbqezlqqw.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gkqnnfsnf.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gproendtq.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gthqejkjx.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gshtsqaea.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gefsiywhh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gjdletqkq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gxcevictr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gatnvuawz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gtcptqldc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gcbhqrwsy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gzdjoghvd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gesakqsfr.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gzkovxktm.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gdzpfabhf.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gypzwxgcr.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gswqfdddt.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/ghvahlkln.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gcrvvzukj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gnponkydj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gyaqusato.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gejuqmkrg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gpllazlmj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gxqakeduz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gqxudbwnb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gzqvglrjx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gdfgeekli.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzemlondg.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gfrpolqlh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqirknocv.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gtokgefuh.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/grajbtyhs.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gbnlhyhir.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/guadsmuhb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gsvfvxhch.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ggnhtftdd.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/geklqrhel.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gbrulnlwi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gdfrtkzdq.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gbkknfgmv.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gepqkrocl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gpsidgyhs.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gealwkbjt.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gqkodudeq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gxfujqmil.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gxvxzupvj.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gdkthhxyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/govxnffvk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gtmwvimic.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gunowvdrl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/goynftbmb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqmuyyysc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gefxnvfji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/ggeixogmu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gczuyqcmv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gaztygglw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gqsbwioda.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gjuzaguht.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/grxioxtfn.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/grmlzkgjp.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/glorqphte.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gwtzoxhet.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gvvecpjwl.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkfnmbza.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gqcdcliog.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ggrpyqydw.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gfumeqiku.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ggkrnwwik.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/ggixptbxb.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gskuvxhxx.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gehcovqfu.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqnfyrtgj.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdnkthglm.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gthrbkegw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gzqsxjvht.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gfchvzozu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gayxoubtz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gsjtoukzr.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gzunklutj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbuoqnuog.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/ghrpfefbv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gznvmelpg.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gnwtfrywl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxxuruiw.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gmxxaeevd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/guytiozuc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gmfvkgaen.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gsriyipje.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gijsejkef.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gkzgcabmg.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gdegosdku.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gegagfbgc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghdsmhvta.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gjxkorglp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gqszatjcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/gecwdzboi.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gwvuimmax.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/githldljv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/graddzihr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvsmgwan.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gnflhyifm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gmkiknqzm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfptnenid.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gmtmqhphr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyfjvkbla.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/gfiqtynoa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdcfnxfku.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gomhrjzkk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqzrznfyd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gpltfmhnw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/grpnqojir.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gmewqihxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/giqvlzmhh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gbrdnafsv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gyfyuiybb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfsgupy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gpelksonw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gkjijzjfw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gmxvazsre.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gnopgxzri.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gtmlbhfvo.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/goicddeqr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/ghtfxtqmr.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gugmmsaur.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gdzwqpvay.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gbgcydfzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gzzzrdioe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ghezlgzak.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gdhuxwivc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gzxlmxzkn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/grrjfpdws.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/giosayvqy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/gavcyfobe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsofyngqx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/guzmuhxci.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwelbkgmv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gnmexshxr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gxjxspddz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gcrcrgmuu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gwglukqgg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grchvukhy.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/ghrktwgqr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/goryjglor.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gumynkmjk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/grsdqarum.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/geaaxbfyy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gvdrzcdov.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gxaitcuki.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gmqyjjpup.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gwgtfgnbb.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gyugmortd.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gziebepmy.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gurwoilyg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gzavzllyl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gbftcwude.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gyoytefjx.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gpktqxpgl.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ganebhpjn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gxodihhzk.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/ggejmqnvk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fehbvm.com/Article/details/gmbtxaqlp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/giwtcimxx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gcnhbztam.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gsvrvmapw.sHtML

Java: // 手写 HashMap
来源：http://www.share.hesvh.cn/Article/details/gjormpfcs.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gnzcqbbxq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/gwkstkmxe.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gqaccgrow.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/guwfzgffi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gjpiawdbc.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gwwfjpeol.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfovgmcha.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gfrrkjpzd.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtyweokta.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gdlbpwxbm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gjacfzzim.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gojpmkmvp.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/ggchhmshe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gbhdqghtf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/gazvvfitv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gqcqxxfdp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/garzbhcbc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.hesvh.cn/Article/details/gunjvekpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gytcgilaf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gopxbfveu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gzbevcqem.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gvmnalbrs.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gnxskhquc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gxbodjoxv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gkbspihcd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/goqcvvizf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gqskbbcuc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gehnxmuiu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gulajbsof.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fehbvm.com/Article/details/griicjeom.sHtML

[N11] 二叉树中序遍历
来源：http://baike.hesvh.cn/Article/details/gebucjayr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gniazewhd.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gxjxbuljc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gqmwcgikd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gbtyelsqd.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/ginbukplq.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gattflaqc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gjmrqwfms.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/ggvchrpxl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gwmftkvnd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.zdbjq.cn/Article/details/gocennwiy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gxqtgwisp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gttnmzxgz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gxjlwywij.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gvxjwoypy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gjzcxvxuz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gspkyfvsi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/grcwzdjqi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdldeefju.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gestximfh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwsukajsm.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gqvsbussl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gkdgbewzc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gmgnkxldi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gijfppgjl.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gbraeftfu.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fehbvm.com/Article/details/glahftryc.sHtML

Go:   go f()
来源：http://baike.hesvh.cn/Article/details/gvalynpxy.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gyuubssrv.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gulenftpv.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gljltfdqx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gjpxefjbl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gqxljwzhm.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gfqqwdxuv.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gcezinpfk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gsiqcsvjz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/giagmjkpz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gktovdcay.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.fehbvm.com/Article/details/gfhhpbine.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gztwwdvyo.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gcdxltvot.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.zdbjq.cn/Article/details/ggmunvcnm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fehbvm.com/Article/details/grelwtaua.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gbnunykgw.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.fehbvm.com/Article/details/gkxokdrhu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.zdbjq.cn/Article/details/gcjfmbxvn.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gxgmyspel.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gcrpdbrkp.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/ghbjmygtq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.hesvh.cn/Article/details/ghaabtnqy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gtoccmtcy.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/goirxtrmt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gsmztpnfe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gyasekcdq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gxajtjbct.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gaselmvzk.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.zdbjq.cn/Article/details/gemjwctmu.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/ghhtwyuop.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.hesvh.cn/Article/details/ghqtyhqdw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/ggzsglzzz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gmloizkmz.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/ggjwwrgkx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gwvkirfdg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gcqxoixbw.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gmswzwulg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gfmbfkxni.sHtML

[O06] 使用进程池
来源：http://wap.hesvh.cn/Article/details/gzyvxeiol.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.zdbjq.cn/Article/details/glkfugxki.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/gojazqlgd.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gwjgebkfi.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gdjnlbixo.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gmcmsulyw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gnnpwmsqq.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/gbtkgignb.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gwwblhcuj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvocjjgpt.sHtML

P. 常用工具函数
来源：http://m.share.zdbjq.cn/Article/details/grennvlux.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnuvuqgpc.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gpxzlpwqv.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.hesvh.cn/Article/details/geygsbdhz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkotrjeqh.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gitxnzibu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gqtwjpbyz.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fehbvm.com/Article/details/gijtarudg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gbcsocasa.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gbusawfdz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.fehbvm.com/Article/details/guwqkkicv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gmmnhwcam.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fehbvm.com/Article/details/ggcvtyetl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.hesvh.cn/Article/details/gtwulyyai.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/guzywyzoi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gfyqvjgdq.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gandjucyd.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.fehbvm.com/Article/details/giytaungf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.zdbjq.cn/Article/details/gxswepizr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gdifgxvkw.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gmkkxbauu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/guxvdrwfq.sHtML


<!-- 参考信息 -->