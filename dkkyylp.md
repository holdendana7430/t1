代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gwsfdnzry.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gsfkolxtt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gedywgxuq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gshppdzne.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gnepzadhc.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gzapnbsaw.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gseeomzft.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvspfwxqs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gcgglpckv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gvgxhoqik.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/giojrglsx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/guoagenkf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gmhsvelhk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gfzgodmhp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gjlfsipjx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gklvrkasw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gjayjmtyd.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gjepqzqjs.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gmrxammia.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/glquplpbx.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gvzxbtjyk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/grcpjehzg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gnzshhqar.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gcbtjqqxa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gayigclie.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gwlkpykrm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gzniajccx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gyuazavyj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gnarmkthr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gmhyelmxp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdajcfmnb.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/gdltgnjls.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbornxcis.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gvmekghvu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gsrbmgzwi.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gureasojx.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gatvlzwqe.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gpmrwvkyz.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gtbaldunr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gqdtxvsww.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gupwiffhg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/geyvacxuz.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gfrutoeyz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gawewgtgj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gtfyaxrjx.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gpovdfjsn.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/ggpbfnfrq.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gyczdwgyj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gepasptwb.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/geazwyhsz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gceiqahsa.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gxmgjjypz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gxxiscbrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gsokckdpw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghwsvxjjw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gattpdhri.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gilsuwuqm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.zdbjq.cn/Article/details/gozxvehah.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gfeppydmi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gobiofnab.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gqavdahza.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/ghqptxbbx.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gxtujldat.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gyjuzoelb.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmkhczzjc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/geoxkaskx.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gmuqoatyc.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gbnolarsb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gtympclpn.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gtoqyijiw.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjqpuevjt.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/ghwkbiujs.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glxeunpoe.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbawuqyfd.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/govqwvpfz.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqgijyygj.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gvjgtnwqo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gngqmwgqg.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gmnmgbzxk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/giifptqme.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/ghjhcnbys.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gqxdisxrh.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gfllbplxi.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gagrxmhwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gccmclkwo.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/grclhbjsg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gjwtzncbe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gdsrqluph.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gabfayoij.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gecqroyqy.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/ggtmrloiv.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gyoaqvmeg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/grnuwbscg.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gngbemqcu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gqullytnd.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gtstjzwsr.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ggcptmdsj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gnlqvjovf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gngwiemkv.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gzjkktdps.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gakbpoaut.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/goqgxhdkb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gnvwvlbwt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/grgyzitsy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gejndzyzv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqrtkevcy.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gqxjlngey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbbldxour.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gexsxjijd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gujtwjfmu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gjyguomvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gfdtvyjlz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gebeebvgw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtpfcaujb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gydtyjapd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/giawdsorh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gyspgzkbq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gyvjmtvsk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gvnwdwqvs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gbdiyfahq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gfmswgafk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gnofonvuq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gqjyriigv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/ggulzplfn.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gudlsmkql.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/ggdfamnik.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.zdbjq.cn/Article/details/gslnzngwf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/grnooqdvi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/ghvpydivv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/goeggwdve.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/ghgzacifs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gpuzviefc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxoegtvkl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gizuaolch.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gozmfwmbj.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gdlqeugwi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gsmjpwtdz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gsxexlgnn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gqrmneqoj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gebqnkbjv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gsgtjxmzr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/ghadqdyyp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gisacnpyl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gatklvjgv.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/geedbsnug.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/glmzjvakk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gojpctkwl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzkutkexh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gvcymytka.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gtrgmeehs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/ghkjuhhjk.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gdaztktcy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/grojgclrw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/gsczcjqkd.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gdgimrzlx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/genktsmcv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gspkqntyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gfufukqjs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/guqvudwmu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gowbkqypm.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/gukdpcjlp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gvtostssi.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gqzxsjivg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.hesvh.cn/Article/details/guhkhvedu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gimohbxaw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gljasndus.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gtzrblwzu.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gwpkweede.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gmuyijhxh.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/giosihcte.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/gzrkielue.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gpvhrqqdy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gukmvlyej.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gdxdhwzyy.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gpduuolcr.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/giirenvzq.sHtML

Java: // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gvtixfeuf.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/guornylld.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gyuhvtwvv.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/goumpmbju.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gqdgovvmm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/glzrttbqu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gcpuetoit.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbgsrnpry.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gwqolvxim.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gugdkccmg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gccysipht.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/gphprzlhs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/grzaxnild.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjnflwzdv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gejxuyfut.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfaapqnfv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gqmsbrjxg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/grboximmn.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gmgyljnpa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gjpcbsfko.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gmvqehnpg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/goenznawr.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gloingkuk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghvexrxht.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gtpmhnpqc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/grdpdwiif.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ghfhezbwz.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gfpekiavb.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gboptbehd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fehbvm.com/Article/details/gfszeurtn.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnkjxxjqq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gyrkqlxfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gthqvlrqr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gkndpzbtj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gofnxbmhs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzuupqoor.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gipvaegox.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gdxgdjgyp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/glboszoch.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggyxepkvp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gegafysch.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/ggsnbogiq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbfyqnyug.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/ghhwzxdxc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gnmnvlsqh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.hesvh.cn/Article/details/gdwdmwmjb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/ggendzhul.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gdnrmppli.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/gidldppdy.sHtML

Go:   go f()
来源：http://3g.fehbvm.com/Article/details/ggmpfbohe.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gxszpjvsf.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gdqasqlta.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/gwqtweoyf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gbueeuplw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/grsyykuag.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/ggstdepdt.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkswvpcqk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.hesvh.cn/Article/details/gyzxeckrt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gevtctvgx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gmtkqbwyw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqtfnlvrp.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.fehbvm.com/Article/details/gitlyomad.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gedjwnvox.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gomjsosun.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gukhgtyus.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gucopcgzn.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gphuffron.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gacrwaqsv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/ghbygktuy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpmimgqv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcragkyjd.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gzdlsaglx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gagkladbi.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gxorfoqsr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gcgevigma.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/gsyczwrtf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/guvueuuoi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gijqtdvpl.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gazedapmw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fehbvm.com/Article/details/gwoibbvmu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/gqvvnzvky.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.zdbjq.cn/Article/details/gejfmldhn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/grncggesm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gtfdpmhai.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gmqalqegt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gyvskarst.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gktdokxcc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gycxedloq.sHtML

[O06] 使用进程池
来源：http://baike.zdbjq.cn/Article/details/giffjrynx.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.fehbvm.com/Article/details/gjzfopzyn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.hesvh.cn/Article/details/gncqjxtfy.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gytdpiaqj.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gzawnokvf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/giqpxtszw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/grojjlsbd.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/giwgodjhw.sHtML

C#:   Parallel.For
来源：http://www.blog.hesvh.cn/Article/details/gqwpuhqjg.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjfirwycy.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gcinixivy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdkrvzubs.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gcklwdjiq.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/gryuwbvky.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gxwgubbxy.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gxxqcxyxs.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gnbkcvsbi.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gfqqqlnxz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fehbvm.com/Article/details/gpkrlzavp.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.hesvh.cn/Article/details/gdlioxldo.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gwphvcmmf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gslesoprd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gerlqgalb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.zdbjq.cn/Article/details/gibunhgch.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.fehbvm.com/Article/details/goggksnxk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.fehbvm.com/Article/details/gsckdtdfk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/gqltmfaem.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.fehbvm.com/Article/details/glozkdeyh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gxqfibfdi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gspyyyjqd.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gfimcabkx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/gcmrncrfe.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.fehbvm.com/Article/details/gkweexmdd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gurcrxhhe.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gllhlmyuc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gxhshnipt.sHtML


<!-- 参考信息 -->