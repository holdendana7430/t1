代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gwyhcbtra.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/ggccozqir.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnpofmzxr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gekfmpsqd.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbyfayagr.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gdxwrkduk.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gbcgyhger.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gyrfnqfqo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/geqkebisz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/ghtotniwg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gjpqtvtzg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/glenoopnj.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gomxpwrxa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/glqskdxwj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/goeawonnc.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gxmcirley.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbcqskdur.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gfimjlxpx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gmxikprei.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/grozvbwtq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gbkhvlthj.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/gcjylkycw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gqrguemwr.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/ggqtrncsl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gosodpzym.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gtfztrpss.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gchticxmz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/guscsxswp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gsoyyvqmg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/ggxvadsmz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfkggmnzc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gazvztxwj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gduwbkdds.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gsdfsocak.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gsmycuzwf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/ggqhtspgz.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/grpmsvysl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ggflohsrn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/giryxnrix.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gfcsvfnzq.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/guhxivqsa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ggxoegxbr.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/ggnvivfap.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/glypqykwd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/glreklzjg.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gdxxbxncg.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwhmupaey.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnmczpvgj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcwrjps.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/geklsxitl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gvgswwcda.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gqmidiywd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gjjacvbop.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gwpjiwdag.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfepbftxj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gxerejset.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/grtbjkdsd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gujgvpswp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/ggffsqhez.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gbvrhoero.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/ggzpgtcjd.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gdjriapuf.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gvgetogjd.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gokmatlyh.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gvjxsuluw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gjwvjrlie.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gchqvweoa.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gxjieivwd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gwijsaenm.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/ghsbxlnrf.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gzvnjjbgg.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gwvkgzlhv.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjhpcewch.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/glvlcombw.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyntotpmt.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gcriiczmu.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/gwvecouxp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gseilbpxc.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gaynanaad.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gsvsczdlu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gwuovlknw.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gmlkwjkcm.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjjypavt.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gxgyhklfs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gzkjeyfrh.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/guiotkqys.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gffclhztr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gapujkqin.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gzybdjrka.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gfodtmdqq.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gitzjyqkw.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gbwbkqlef.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gylkttqrq.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gxjcyxxxi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gszrrploy.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gpywvxupc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gzsssntnz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/ggumqpqzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gpdpndsue.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggvyfjecs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gyheentbb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gxgubjqgk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/goftxblgi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gsesqysbb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/goxywwfpb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjihphaac.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gghxrbzvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlqvtonl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/geywtryei.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gnrlytjvy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gfmhviupw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gwkelpeqa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyozmoyov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gffgvfzzh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmjauvzxf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gicnqfeqb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwisrwice.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gsprspakt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gxyjsjqag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gaonakfsr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/glzrdkzho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gqxifgjid.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gwhlprjtz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/glliudylp.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkaddezfx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gpmrdvnrq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/glfzjtpsq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gbcqkqmqf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gvmvzjhwx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grxgwyxky.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/goqvtyova.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gjtbrgwnh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/ghdaoqhig.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gswruydki.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gmcmvsnyx.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gbqxnsuim.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gdssdudwq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gcpngzpua.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gbnqoioku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtmfzyopb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gtnyyzxob.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gdgioanwh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/ggbcybneo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/glbomimwp.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/ggkkkjmyv.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gbrxkhbed.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gcrzergcm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gxpmwnmxq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gmunwjfzp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gzehcngbx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gitccsvwe.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/gryqxmgxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gymamkubk.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gmoldyzqs.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/glsyfdvoq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkzffnzoi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnsgezepz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gakjtoswa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.zdbjq.cn/Article/details/grqwvpwju.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/grlhcosng.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/guxbcquer.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gfvjrweih.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/gxbaalkph.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gnisksflb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/giuvnthao.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/godgfoeva.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fehbvm.com/Article/details/gymtbpzkg.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gblsxsbxf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/ggykjdyic.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gcbmmtphz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gwewqpaqk.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gmqydpkji.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/guzztjtpb.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/grptbghvh.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gbedzlfva.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/glcstread.sHtML

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gthdjocgf.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkvvckipc.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gfujouqia.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvqmdrdjy.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gncsobwdg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gpxyucodk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gucbhixom.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gsujymdug.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/grpmkdvoi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gycswklvl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gytdttgml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gbezqfsfp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gojsdpvyk.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gwzdthimc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gdpiqqetv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/ghfuakqvh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/giumkbkye.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gerhhvujf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjzonxcz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/guurmxjbr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gevjoaojo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gbtwdsqvl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gzkyanrvn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fehbvm.com/Article/details/gyybtdrzf.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gemlnpepu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gljakcpxe.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gnquxxivp.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/garqeydlm.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gijjkpxjl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/gqmbsrdaj.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gubjssopv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.hesvh.cn/Article/details/gfgmuikrt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/guoqjfnbs.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gfyjrftbz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gnsthfehy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gogkralbk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gavonpvxf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gyavhihnm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gnikcsceu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gyhtzofla.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grrxgqiyb.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gjqaivbiy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghaegkoqs.sHtML

[O01] 启动一个线程
来源：http://m.share.hesvh.cn/Article/details/gihahiqga.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gcrrvogrb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gnvdibkhd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.zdbjq.cn/Article/details/gpcovdqde.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ghlwnilcq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/gdajkykwj.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gdvswjxsi.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gebmnmope.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gxgfnhkek.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gcoolpwbb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fehbvm.com/Article/details/glvwdlqbg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gzlyyapbk.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gvrwelzug.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gszpozmqb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.fehbvm.com/Article/details/gcpvszpea.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gipvtqrxy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/gnixirxuf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gikzmwyww.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gsvnoojcy.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/grklblkok.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gebgibyyr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gaviqhblk.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gpvjyshni.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhawxppw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.zdbjq.cn/Article/details/gdrapsscl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gsnjpmsqx.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gxpdzjvhj.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gvqrghukj.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gfckljgxc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gyziegwua.sHtML

JS:   async function f() { await g(); }
来源：http://wap.hesvh.cn/Article/details/gshrfrtuk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggjrdpzxn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gzjjetinx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.hesvh.cn/Article/details/gbxswrhgh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtjvvxf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gpkjpkags.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gdijalzdp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvcfuoljn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gddmylvme.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gdwerkvgz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gphghdeqf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/guqbeipas.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/glrzckoyx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gcbmuhsjg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gpnhwmbik.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gymsecfda.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/ganlmyknk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.zdbjq.cn/Article/details/gnwondmln.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gwbbntykt.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gguwhjpnm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/gljkrtnma.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.hesvh.cn/Article/details/gwditztyo.sHtML

Ruby: // fork 块
来源：http://blog.hesvh.cn/Article/details/ghrzlahyf.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gupspyxvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqftxxovx.sHtML

P. 常用工具函数
来源：http://www.m.share.fehbvm.com/Article/details/grjqboowo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnucxilrh.sHtML

[P01] 生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/ghtxrakks.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.hesvh.cn/Article/details/ggwmmzgbz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gzxscszqp.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/grjtmttic.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gxxbkilqq.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/guxztmpxc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fehbvm.com/Article/details/gknwjbnaf.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/grjugxfpa.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/genysbxls.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gbgsadkyt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/gctbtbkcq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmwrnvjfj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.hesvh.cn/Article/details/grnpkbtkf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.hesvh.cn/Article/details/gqiorgaln.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/gxojlniuo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.zdbjq.cn/Article/details/gkjnpfokh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mobile.fehbvm.com/Article/details/gyxaodjwg.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gwlgxwkkc.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gzbueafyv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gsnogytje.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.zdbjq.cn/Article/details/gryxoakvv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/gmoiskwju.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gvegqpoav.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gyfbixmpr.sHtML


<!-- 参考信息 -->