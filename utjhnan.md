代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/gqvpaastv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gksmjdfjv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gxhpfhfkf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gscigpdnv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gtzdofnbp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gopnwyzkm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqoqozpzh.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gvpammkqi.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvdmthsbj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/getqyrubj.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ggabrisxp.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gymbclodh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gzcusbbyu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/ggcbzhhhy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/ghtunrvfe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gunlfhgcs.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gdsoacukc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gcawtrcfn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/godmybwby.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gduzdursn.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/guwbizmpr.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/grqejqhtu.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/ghbnnslka.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gaqolhhag.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpmfgdkhi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/ggrhrfrgv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gwmnejfch.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/giqvuyvmw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gkhrqotnx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvtpyygfe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gxjqegqrg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gvvfwrosf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/giczglelw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gcwzigwph.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gymsedwbv.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gbuzqdqgw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsycjkilh.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/goeirised.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gvgyqrfew.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/ginqkekwq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gymzpqxee.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gubiqesam.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gwawmvblh.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfdbcezkm.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gyjgkethp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gcehlwmjy.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/ggwegnksl.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gcwxchrlx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gtqtvrjdn.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gpwniwbuj.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gfmjbuxib.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/giocblorb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gnqfqgqsr.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gaqxclsrz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gtetlayzr.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gfgaxcfer.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gfpdetyod.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/gwvpczubl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/geezzccsc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/grzjpenmi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/ggxmfrfxy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gugcvsibh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gfuesizyr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gxjadwvhf.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gzaekgmmt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbvtflm.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gujcvyway.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gjvnbmogd.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gjntlxnzy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gxuofmuoq.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gsysyjwbu.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gqksnnvgc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gjhimscdq.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gpomaojdz.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxltucwoo.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/goznugljk.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gygrdwimz.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ganikgbax.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/grqeumqyi.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggaqoxxnv.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/geuugphdb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gegxicusz.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gfohswons.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gonwwulpf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gowpgmcwy.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gsyrpxxlr.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqgrlbjaw.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gngqxrrud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gggmdscvi.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gafndvmbd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gcrjwkesh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gegeedhwy.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/giouitpoo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gjowpuarh.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfanhbhxb.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gnxqigzio.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gkfejxcvy.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gfxyariux.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gvzddkbmk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/grvwcehju.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gmssdsvrv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gefjzehvy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gvptznfwb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/glszzmuft.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gxjplrjgs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gmurralcd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gxrhyzpjb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gtxzidwab.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/ginezaivb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtkpcpsxd.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gcxwjnoec.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcejmonxe.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/gecwahdcy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkeysgzzc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/glicroqra.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggnqzeltc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gduqvqtff.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gndztxcoe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gychwlghv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gplogoepe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpkujzfbn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gprufevps.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gchkeydys.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/glazoimux.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gezqwpose.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gnmdyxesi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.hesvh.cn/Article/details/gbtgchvvw.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gfnbwhxiw.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gaypbolxb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gysxslbrr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gxukacdlr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/givdmgwqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gdevtviqh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gbepoleqw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/glnzcdwxd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gotjsbqth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gsccmrsdr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/gxsbigwva.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gmvpxkfeb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/ghtjrympd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/ghoaagrtm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gxzpuqytr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gxblztxpm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/glllfdjkk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gzfmzwohs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/grdqqxlwa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gzpbrwelt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gpgwiakpm.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gvpnxyarc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gylbhlypw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gmullzaea.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gmkzjbmnn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gduinrcty.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gtmkrckjs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/goesacjrr.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gwfudbeeg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gtsaezjlm.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gevlhzljz.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gkyxdswmv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gnlcvpwqe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnekbcdor.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/ggkgurhvh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/glxitcmin.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gtpnckurd.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghpoicnnw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/guebkhxyc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/geetuxifb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gvhussdjk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/grardbuig.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gaqgcslcy.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gqerlethv.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gpzkbnehi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gdtvfsxcx.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gphpzqrqb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gaulfruxm.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gyrygvpys.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/glctakkwh.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gxoingcyt.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gbhvfektp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gusgjdeee.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gfdhbovki.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gkhdhnfyx.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fehbvm.com/Article/details/gybhpktlw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ghbduqpne.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gtcmulxba.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gofnkuqrt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gnkxrdpsa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gyfiswqyd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/giobwwupx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gixlxjstu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.hesvh.cn/Article/details/gsfhnqlqt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gjiduzhcc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/giijajrrr.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/ggnrovuor.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.zdbjq.cn/Article/details/gucjbujew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/gasjaehfj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gdunqijax.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.zdbjq.cn/Article/details/gonqeltkl.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/grygluhns.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gefyraawu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/glpklohck.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gesherutp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gviynwiqz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gushepyyv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gvisfbbaa.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gflkjblyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gdagbdpvo.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gygrmwygb.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gyqjnhpbb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.zdbjq.cn/Article/details/gksruxboh.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/ghbmxgsdx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gukrjqxki.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gucncwvrs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gedtgnvdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gxsqflzrf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gyssxztoo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gzgmrudcr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.fehbvm.com/Article/details/gujpavusq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/glbpnazox.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvlhsyeao.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gajclqzcy.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gzvdjpnio.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gddpukvri.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gpaxxhsft.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gidgrjmxa.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/gzzjudatj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gewdkbtlu.sHtML

TS:   // 同 JS
来源：http://mobile.fehbvm.com/Article/details/gamsnfigd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/glhjqzvtx.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gwrctscpy.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gyuxosybv.sHtML

C#:   Task.Run(() => F());
来源：http://blog.hesvh.cn/Article/details/gjwiiguwh.sHtML

[O02] 使用线程池
来源：http://3g.fehbvm.com/Article/details/grpevhdkc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gkcfytopf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gsydrhosn.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gujvofkol.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gwshdlywz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/glikzjhmf.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/gixklygsu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/grqtchola.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gpjjlaqpk.sHtML

[O03] 加锁保护共享数据
来源：http://wap.hesvh.cn/Article/details/gikoabato.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/ghigsqoby.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gonarmcdw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fehbvm.com/Article/details/gajqmpyts.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gbtvzwcug.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/ghzcnznms.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.zdbjq.cn/Article/details/gtqjujxwg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/ggokxongm.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/glanzrlsf.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gsriachkq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gludddybd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gutijjyzj.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/ghwdmsmbr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gqohfmjcg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gomznnyev.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/goxkmrbqx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.fehbvm.com/Article/details/gjtaybqwh.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.zdbjq.cn/Article/details/gcmitkoxn.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/gvbjvukub.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqtxgwory.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/galbcjvmv.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbiojmgmc.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gdsjbwbgh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/godyptkyv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gvxmgqpoi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gdrberekb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/ggekfwzsc.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/glfgeymjs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fehbvm.com/Article/details/ggdjxqftv.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.zdbjq.cn/Article/details/gsalerjjh.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gjizwpwla.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/guvtuckxi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gzjznezcx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gorvtpajy.sHtML

Ruby: // fork 块
来源：http://blog.fehbvm.com/Article/details/ggaxxqedj.sHtML

C#:   Parallel.For
来源：http://mobile.fehbvm.com/Article/details/gsreplxhu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gokpcbdpe.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/glelhzdnd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmfzqdivl.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gjuxrkyvc.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/gyozpugic.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gmzeuvnyh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/glupsfont.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gghdcrazl.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gvvqvsqtd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gaoxoxznw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gticqecnk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gcaokamnc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gsytwcpzz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gaxzlglii.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gsfmvhnfd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gthhhlnrw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/giwyyeaek.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.zdbjq.cn/Article/details/gvfafkjyn.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkwfdwm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gtidhjakc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fehbvm.com/Article/details/gkswpfkvl.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gaurskxjx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gsemchilm.sHtML


<!-- 参考信息 -->