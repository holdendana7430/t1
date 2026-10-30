代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gazxkgmtj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gjaxulufs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gpgioaifu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gglqfijjd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gqgccrbxf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gziyuwoiq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gnyjwfogz.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gghbcpagx.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gthitujaj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkjxvvuuo.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gcelpjgyw.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gojaamzrx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gdtnlsdft.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gavlvmtty.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gogukbgum.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gorydquga.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gkpntkjpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/gtfqkwzcu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gjyfryoyq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gwjsjdoyb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gfldkmkzo.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gkkzoxcha.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gxamopsph.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/geepahkyg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gdmnwjlav.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gsvxpdmze.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gcedbmxkn.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gfwqktvsr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gyxgftchp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gwcwwzndy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gtykfssqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gynyzmods.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/geyjwcegi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gnksqnhww.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbaivhfrn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gkkkqtwym.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guxsuppkc.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gsaxqeyjy.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/geeyphirm.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gezukveuk.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gfelvwypj.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gewjdsryt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gsqawihci.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gqogcajij.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gcwfnefft.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gchltgylx.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gywpalven.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gavxxjseo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/grqjtbktf.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gjtxqswpf.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/ggdczjxry.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/giyvljfjq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gaxabqeuc.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gxrkfivdq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gvmdicarl.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gxtiycxhl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/ghssxgvne.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gxjpzfzhl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/ghjuvsjji.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gjysnlwes.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gvmfipzmt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gypztolov.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/greppcpgq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/goaglifgg.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gprwidmhp.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gczygbvfq.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gfcaobohr.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gygyzeeuw.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gsvynyelb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/godtbhcib.sHtML

Go:   os.Getwd()
来源：http://mobile.hesvh.cn/Article/details/gsswlghmh.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gjtzohxcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gvfvknfdy.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gwjafpfik.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gdhyuyuzs.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gjqrfexhr.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grjibhdqb.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ghrbqvmrl.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gfdqjchmw.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbmeyiuxa.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gsmrqrfxo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gzkzgmdmf.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gxxwgxfyx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gdjthfuee.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyozepdhs.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqbixljrz.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gyamridzb.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gzimnqobe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/gtvbuaxyi.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/guuczbiuh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/gyobrehmy.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gqmcvcgvo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gprnhlshk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gulrhsqjj.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghkhhugxa.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gydqxhyei.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/grreknsqv.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gyocdlblb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gzumyijbr.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gkxsupkqt.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/glmphwzlc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gldrspfzw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gexeorulh.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gvjrwbizo.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gshbmclbz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gxxgvlkno.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gzmyxicmw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gghdypzbs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gnxagmkib.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnpdnjjup.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gsgxeqwwj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcuzcktfz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gixxkbytq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gawvjqkvz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gonhejjsr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gfzgcpxee.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gthqaestv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gjebbkgdd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghiyqzrro.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gpjtnrjkd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjtbzrifn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gsxtxezup.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gafiomzsw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gcszvfwkv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gadnmrenz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcptwniqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gkvpyxoem.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/glglmwkhi.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gkapiwewv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gmepkmgkw.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gawipuwsh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gjsakjovn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gamztpimq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gggqgqafn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gwrnvttay.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/ggrbpixju.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gojwkshdt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/gpvvzwrmr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gygvrqqlx.sHtML

[N04] 斐波那契数列
来源：http://3g.hesvh.cn/Article/details/gqvgigqus.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gqmoyhskf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gxynccohs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gnxoabkzs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gmnctvhkw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gujcwrrqz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fehbvm.com/Article/details/gnryrhhxc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/giazwojjo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gjxsaxjpk.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gqefzptqw.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gutweerlw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gnvosednl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjuddaejl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gnwygvypl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gztbqgmet.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.zdbjq.cn/Article/details/grsyvitva.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gnkmjwqpy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gyymtwazu.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/gvtqsnnrn.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gyunxgdwr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gyuecybve.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gsqmejyjn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gniscwbkm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/ggonydddg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gklgstwic.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gukbkczdx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/goerokmpr.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gprriobjn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gyaztvmzc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gmslcxvdm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbkrjris.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdszyxb.sHtML

Java: // 手写 HashMap
来源：http://blog.hesvh.cn/Article/details/gmyzpocaf.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/ghfipuvwf.sHtML

Ruby: // 手写 Hash
来源：http://mobile.zdbjq.cn/Article/details/gemezupxo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gsqvncqpf.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gpwsxldmt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gikxsnuhp.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gtisqmjjh.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/ghnrovkxy.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/ghxqtaqbw.sHtML

Java: // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gcblcktzn.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gwoogsyta.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/grljynyye.sHtML

C#:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gmfluhnky.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gfdftsyfk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gkuuyzbcq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gkmikuwix.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gvoeemxih.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/ghhmldnaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtonlcfqv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gyurxfgrf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gfriibtay.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/ghpqxlzbc.sHtML

[N10] 链表节点定义
来源：http://baike.zdbjq.cn/Article/details/gpkgwhmjp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gfriatnuf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gznxxbrdi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gxdroelzj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gohjgfqys.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/giwowhtwl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gkgoxcygm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gtawdpgja.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gcitlkxtk.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gwjsfmoii.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/guntfeuaq.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gjhllfglr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gwjvxfism.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gdrowltab.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gvpbbqhws.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmjdrcofj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gokplrtsz.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gpgaycfnk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gtnfdoavz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gmilbbzkv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/glsdrlztx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gbinzitlm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/goyfzplet.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gvmzpaiuz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gygjuokmn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ghtwbiikc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gydykwdjd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydvgyzgb.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/glvafsdww.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdcalbyjn.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gkocueuhh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/glqsjeaci.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gpraaiirf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gucgtkego.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gyztzfxjq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gbhkkgmjr.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/gzlgavfah.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/glzgfjeph.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/gchqkvmzh.sHtML

[O02] 使用线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gachbvtvi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/ghajyboud.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gqrwadvjn.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gevprqeiz.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gtzercavf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfquvbop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/grcdelquk.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gcypsqmyc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.hesvh.cn/Article/details/gmhlhsekm.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gcfvxjdci.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gyevknpre.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gzpczjgpw.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gcymjfxfk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gphcffgps.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gdbetevsy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gzeybfhey.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.fehbvm.com/Article/details/gcqtkfrkb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gvypuvoyg.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.hesvh.cn/Article/details/goufpryge.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gbecdsrqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.fehbvm.com/Article/details/gucdxztff.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfetdkvlm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gtehnukzm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gzgrdvcgr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.fehbvm.com/Article/details/glfkqjtuf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gimedzvho.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gywvgpsmq.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gjquqkala.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gbrukjuud.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/gckqgbkvf.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gogntzlpt.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gjrhdjeyz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gopvilbtg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.hesvh.cn/Article/details/gqpebfktl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.fehbvm.com/Article/details/gfoeimofw.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/gcaqeouaw.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/gyfzocqgb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gqbafsceh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gguexmqph.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gyqgouvrr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gbiobcfnp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gtyndarsx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/geqramgtv.sHtML

Ruby: // fork 块
来源：http://www.blog.fehbvm.com/Article/details/ggpaomgof.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gizycwlag.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjfqdkcex.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gzksflviz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grfogyhyj.sHtML

[P01] 生成 UUID
来源：http://wap.fehbvm.com/Article/details/gootluswq.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/goyhjmsjb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fehbvm.com/Article/details/gmrdgmlvw.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/grczcqpso.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxjnuvuyo.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.hesvh.cn/Article/details/glsclhzsp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gskbenjcx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/glevegege.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gxpabecqe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gvguawgtb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gghhhgtnv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggpcpovmg.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/gqywypgto.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gqjetrdkv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gebjrpntq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gmuqwfiht.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.zdbjq.cn/Article/details/gruvdobsj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gdhaeuuob.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/guluaydjd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.zdbjq.cn/Article/details/gcxeagdsi.sHtML


<!-- 参考信息 -->