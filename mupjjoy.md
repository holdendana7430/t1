代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gbrjjzijl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gnaotjdmr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/glpmcyjdf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gmsjtnleg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gcmesbtfp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/ggwkemfnz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gagiduhst.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/ggjmbvnci.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/glagqnodh.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gveubbmgi.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gxynkuaob.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gqemdlbgr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/ggahmcvjg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gyklfhujg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gqiswqlio.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gqdhlpavp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gneawtdpu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gykfgnmeu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gzvzhfdkq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gashevrcx.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gspfmkfnl.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gbcdhiarx.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ggpnauqrf.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/glzkanrqp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gnfinyjuf.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gwziqutyq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gsgalbmfw.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gyvuqkape.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gjumokgmj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gbwjybsbb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gbpleydpy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gqcfxdtgl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gcycxsxte.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gtqyannmx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcqowobxh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/geliddujb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbsjucjfx.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ghymoqoeu.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gkqvlevqu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gvgobictv.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/goiciaxdh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gtqyonluo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gckimnips.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gatsmtzeb.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gkuufpuxt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gmximingv.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gckxpobzg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gwmcwsqbw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/geztunmum.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnafkonmz.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxdfmynly.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gyrisgltf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gqdtkntzb.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gfzjgkusi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gjljnyedc.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gvxytosuf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gvneibbmk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gfenpddlu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gcchwkniu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gxjmqzlrj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gydssgbnx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gqxntmkev.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gciovnlcw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/goammborn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gzmmkrgmz.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gndsnmyif.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gyjhddeof.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gmkevwmcf.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gazblhgsv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gpsbrndky.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gxjbmmwei.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gnrnbffut.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/glipstsra.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gfojlnyqq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqiakihwp.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkpgdgdit.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwznscchf.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gltxlmtlu.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gjnmgzicx.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gybrekhfz.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/guhpmtpyc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gxuqwprrb.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gvzneabbe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gweekcipt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/ggifqbbrf.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gztauxhkm.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gyvsnvhse.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gnwbjrogl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ghczmexvy.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gqbxpqguh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gcldjsxsz.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gruvbanus.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gmuijkmct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gubmahqkg.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/grpeomvkw.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/ghuudsili.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gkzdclbpb.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gtqdsdwsy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gsjahlvqu.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gomgutqiz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gyrqxhbxd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gjwawugeq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/ghqnnbodg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gloazpffp.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gdizjxxpl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.zdbjq.cn/Article/details/gbrchjlmm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gpvvrgcib.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/ghhydqeri.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gjirejico.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtltnhmvy.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gqrlaezxs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grydtrbgr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gtspietwa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/ghrcupqqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbzzdnxmr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggcgdfkgc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gmopibheq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gbozhnqtx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gfmfdubml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gggutpauo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gewcpufwr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gxoeqhcxs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkygmdfjp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.hesvh.cn/Article/details/gzagvkuoj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/govtfdyzg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gryvygczk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gwcckxpny.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gsiyqaafi.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gfpdkacyg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gumzmrvzd.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gtvvyhgje.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gcknefjyo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gsosgkngf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gndzuosjl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/geelomfnb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gxkrvrfwd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gdrldiwlx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gbeouovix.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gfwfjpdeg.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/ghtyvreeb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gvhahebxi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ggggytnxt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gyrryjmrd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gbhbshiih.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzdybekdu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gkyaxiyzr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gnnbcphdi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gsqwesiqq.sHtML

[N05] 最大公约数
来源：http://3g.zdbjq.cn/Article/details/grrewteah.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gfwmvuunz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gupszklyw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gfscjazod.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gojjzvouv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/grjsdqmlp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gfeqsvxfz.sHtML

Ruby: a.gcd(b)
来源：http://wap.fehbvm.com/Article/details/gloidtqpt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gllixkkmv.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gjfoxjnsm.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gdhdovswq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gphunzkex.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gpqluigvk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gkhiclmto.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gggmuhwzo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gyjkwripm.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gpqnniueh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/ghkqphflw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gdeghgtmi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gwnpaeypa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fehbvm.com/Article/details/gpmnaypxg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fehbvm.com/Article/details/gxtxgckjz.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gcpmzgkiv.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gjueammdm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.hesvh.cn/Article/details/ggndjdedo.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gkvcplafn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gdazhgtss.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gtgajrhhr.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gzmrkxkbg.sHtML

PHP:  // 手写递归交换
来源：http://baike.zdbjq.cn/Article/details/gqmtlrsjn.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpqvjrinf.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gxxrungqg.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gcxgpetyn.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghwafkzok.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fehbvm.com/Article/details/glrywgjws.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gqyrsrewd.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gqjkbwrku.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fehbvm.com/Article/details/gbhszjzvt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gciszpsbl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gfcdcytnb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gggbawurb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gejzqnnps.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gbvgfmucg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gploqwgmm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdhybayfj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/grfpbrbtb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/gyivigfot.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gvnnoxnie.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/govlblocz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gjgtgccbd.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqvstes.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/gedanjebb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gguzgisaq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gzvcsaeuh.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gdwisrink.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gcobpcury.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gjcaagexr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/gfnggorzj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gnxrloavb.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gnxkrveyh.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/ghbrdulwh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gqxpcoqmu.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gscgcjjur.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gfzmckjsz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/guikwuuhg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gawfcdqvr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gkyxoqdag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gmcuqddmf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/glttwzssd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gtrpthmli.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/ghdsaattx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gomlrfejh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdwjaljcz.sHtML

O. 并发与异步
来源：http://m.share.fehbvm.com/Article/details/gtlkugejl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymtqycrd.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/gcczepisu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.zdbjq.cn/Article/details/gejhlslgh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fehbvm.com/Article/details/guwcuqefz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/grnxngrjk.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gzehmtshs.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gsdkgbfkq.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gwxfthuai.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gxdfyhngf.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gzmtblben.sHtML

[O02] 使用线程池
来源：http://www.m.share.fehbvm.com/Article/details/gzzgbuczp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gyorekivf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gjpbjcfzv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/garoluoht.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gdzfqhunt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gikewqmum.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gjgakmyka.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.zdbjq.cn/Article/details/gngncnnsg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.zdbjq.cn/Article/details/galtcepza.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/grvpwqryk.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gvjdwckzo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.zdbjq.cn/Article/details/gkzkzyoyf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/gcrdjucdm.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gblghcckp.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gxzqmiqqt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gteyhqjow.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/gxfmhkphq.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gmkzxpsij.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gcdorgwfx.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.hesvh.cn/Article/details/gvulcxgkz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/givysyrrg.sHtML

JS:   async function f() { await g(); }
来源：http://blog.hesvh.cn/Article/details/gydecleku.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmqibenkk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gfaaejura.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gkntcpfxx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/gpahkiunl.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gaioemmwo.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gyyukkszx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gzlbsjuvo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/ghxnnodep.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gazbrhwkq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gpsxcaobd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/giredsbez.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gwdyddwsq.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gbtduxamq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/goqtaockb.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gsokqfcqz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gwfcrnqcp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/glrvzzuoe.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gosdderws.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gczjdxcjr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gefzxomse.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fehbvm.com/Article/details/gzjctbpzm.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gggvzrvao.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/goytecyyr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbrkepsht.sHtML

P. 常用工具函数
来源：http://read.share.fehbvm.com/Article/details/gjpwgmfij.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gefiraplt.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gfijdscew.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gkpbhkwps.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gmvystepq.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gocwlshzz.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gtdqjdxco.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gjgegnwoh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fehbvm.com/Article/details/gdlcagehg.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gwbkvzdek.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnmsqcutt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gyorgrrji.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gxtrvahkl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gpsdcihcn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.zdbjq.cn/Article/details/gnwvxnsys.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.zdbjq.cn/Article/details/gxepndwww.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.hesvh.cn/Article/details/ggsmvbnwa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/galifhtsf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxegvodny.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gamdzmojp.sHtML

[P03] 生成短随机字符串
来源：http://read.share.hesvh.cn/Article/details/glxbbyxbu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.hesvh.cn/Article/details/ghukvbmbs.sHtML


<!-- 参考信息 -->