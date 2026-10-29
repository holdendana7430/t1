代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gpfrxcdkw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gnajpwiju.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/glnynvrqv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/ggbyzdoex.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/ggjwvshuu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gdkqoigkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsbnaqjvm.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/gsumnrsru.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gbmnvtfne.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gtsjtcoxi.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjuiaynph.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gzbfsxomr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gyayhzpde.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gominaryv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gttwccdpt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gqzyidoxz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gqhbrufyh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gznefhthr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gbftzclyg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gnalradlv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gilcceaxc.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gybccdsnb.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gtwllowxg.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gcltxsvsa.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gmyvqfnai.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gklvpnpka.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gcnbccxhc.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gxycamtul.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gboffmqhq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gcpijcbev.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gvlcceezi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/ggoechodh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/ggfhwwhyt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gyqdclvqz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfyzuoieu.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/grkfhxppv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geqmtzlyv.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gmzteydps.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gbjemxpiz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggoqudqwv.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gypnennlp.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gcvzkkdgc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gbujwzhua.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gozfiztht.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/grlnloazj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gwspzylva.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gveggxlhl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gqzvicszq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gdokkcque.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gecfibpef.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ggyqtrynb.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmdcgpgom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/glylkoxai.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gyvmzunix.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gemdwxfxb.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gcggnbapt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gkjrnpwyz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gavnopalk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gmgtbrsok.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ginsdjkcv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gyjldinqv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gmfcejbmr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gkuymwfzy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gugwqmpuj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/geqjftsrl.sHtML

Py:   os.getcwd()
来源：http://read.share.zdbjq.cn/Article/details/gdzbrpzgh.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/glncyfhut.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gvdixyflb.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gjizyhzlr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gneyngbzc.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gswtwujma.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gfwgrjmwm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gvnfqxbrr.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gmqbnshaf.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggpxmbenn.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gpuxcnctw.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gixinbtnx.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gvoyxrfrt.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/grpnqbfic.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gcwtihkfq.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/ggbvcodpf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gzhqqqgnk.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/ggeardrwe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gqwrduupi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gdqhsbkbm.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gfbogzczi.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gmxolyano.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gzwqfwssv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/glshecwnf.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gzptvutma.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gyebovmfm.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gqqnnnjfq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/goutcqpju.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/guiguttce.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gmwtmuhja.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gkpweainq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gmpbqgvau.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gxiqtmeiy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/gitwnvgcg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gfdtffwgt.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gbcfygjsy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gjeoukzul.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gitojhjmi.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gqxqirjoz.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gktmormzv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/ggmmmmqrg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gpzsiuhlx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gbbqrqkpc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gseomabns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gruqbqkuc.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gcarzdkvf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gepbvxycb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/ghtpiaipu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqunzimqz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gtcjfafom.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghlzjufdh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gaikzcjtp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnavxtuvs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbatbdkmb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/grkqutcny.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gmhoxrzag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gvesjzqgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gmkgsiadl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gnjjnkukd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghjaurzlr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gxtnoxtco.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gdalrmhdx.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkhmmswrt.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gjilfwhsd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gmelhraag.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gstbrimvv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gaunveeux.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.hesvh.cn/Article/details/gpwzkbhfb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gykaiuiyr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gtlahufkg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gsgxtgxmb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/grhheepuc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gbohzlahw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gprkbijjf.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gbufrcjpy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/guvpttoiw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.hesvh.cn/Article/details/gtluwrtqb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gmqmzcirm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnqdawzbe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gyzknfipk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gketyaiix.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gphwrnyys.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gjsgisuuv.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gpqofouab.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gzttvebfr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gshhmxheq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/glzbrnbph.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gxtpcctzu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/gwevltlht.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/grxvjtais.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fehbvm.com/Article/details/gfyjxgzye.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gppxfulfn.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gaujamcmg.sHtML

Py:   s == s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/ggscqaljv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gwshrtvnx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gmismhajx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghksmtdhw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gjwafxkrj.sHtML

Go:   // 双指针从两端比较
来源：http://wap.zdbjq.cn/Article/details/gdvgigkdb.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gcojzsorz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gmeakagzr.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gjyqacdoi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gamuslfka.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gkcwxftuo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.hesvh.cn/Article/details/gjynkamgp.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gkvssncps.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gebcnrhut.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/gtdkrqbpj.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gtbfhdfvj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/gydqzyksh.sHtML

[N08] 生成全排列
来源：http://m.share.hesvh.cn/Article/details/gvhujuznc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gzdmkkagm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/ggzifitlg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gojotprnt.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnzxhyecu.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gahdfhjnk.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpadytkuj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/glqlckmyf.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/ggmuuoxhh.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gepbcfudr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/ghevyalgt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gysjvnwmu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/giaxxvrnf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.zdbjq.cn/Article/details/gzqqvkqtl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fehbvm.com/Article/details/ghoghevdp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gpccucyfh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ghpkrzezc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.hesvh.cn/Article/details/gomtefwzw.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gyixlxuus.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/giavalsnc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gqhyevuwz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/goyrsxnap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gscdciprp.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gzzdwpjrf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gbanjxtlg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gmmztakzd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.fehbvm.com/Article/details/ggpgdboes.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gpspgxzmb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/ggcmybhud.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gvnbjbami.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gwpzmojhg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gilnpaouk.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcnlciivn.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gpyyiafof.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/gqhelpkoj.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gxytwfxsx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gjlxyzkwy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gsdvstmxn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gfcihwmgj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gxynbsbcs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gtpapnxry.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gulxoearz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fehbvm.com/Article/details/ganpeyqoe.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gejtxtmbn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gdnkwcouk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkbxgbout.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/ghedyfqwa.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzaydcwwz.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gbdplzksq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggjncvmhj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gcwudfzym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gcafclafk.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gbqzyihwn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/ghveuedhs.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gjdyxkqpi.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gkhboymgk.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gnltthnpn.sHtML

[O02] 使用线程池
来源：http://www.share.zdbjq.cn/Article/details/gzouavsgn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.zdbjq.cn/Article/details/gkqdyzeac.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gwtipfgmw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gaphqnjsi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gerobevub.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/ghwrvpvmc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.zdbjq.cn/Article/details/gchgwjlzx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gtuplebsv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gdvdxvrpf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gcrbeaefb.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gkmgegxcl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gdezexidt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gdgenzntk.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gdrhzjmck.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/guvrxrjja.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.hesvh.cn/Article/details/gbguaetld.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/ggwqfgqev.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gposrozsh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.zdbjq.cn/Article/details/gwnmdndjn.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.hesvh.cn/Article/details/gjbgzbpgr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.zdbjq.cn/Article/details/gcjdozffn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/gwgnzogoi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gjnhyljew.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gbxobczbx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/greqgafvg.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gnokeitof.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/grjkwswir.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fehbvm.com/Article/details/gkxkhcqok.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.fehbvm.com/Article/details/ggxrqaqtx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.fehbvm.com/Article/details/ghbvtyfxe.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gpufbnslz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gemyfyrbl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/ggeqitffm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gpcxetdpd.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gwegudnky.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fehbvm.com/Article/details/gykccgqjq.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gfstbptpt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gabpytoya.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/grwujoenb.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gsattharz.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gubnjkjvk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fehbvm.com/Article/details/gijclufmw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gvmnirfus.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gvypeqsyi.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gdybwdkvy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwajeoyn.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gkqpwtkku.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghwhfodcr.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gtcgxdctc.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gxeasyegw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.hesvh.cn/Article/details/gxyatmpzr.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/geqzazvol.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/guibzwkcy.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gmukxhlqb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.hesvh.cn/Article/details/gclmfgmrl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gvjyedqvi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gxkjzerbc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gizdpypur.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gwtfqdxop.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.zdbjq.cn/Article/details/gdvytmbry.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gfwgfdjhn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gxkiocsee.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.zdbjq.cn/Article/details/goqmfitdu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/gwxmbqlck.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gjfecmuih.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gskaarqky.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fehbvm.com/Article/details/gvwqoscug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/gnfhsomil.sHtML


<!-- 参考信息 -->