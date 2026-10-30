代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gettsmnqc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gaikyzfjj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gztzccffi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gsvduylgw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gapdpkmzb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gyrtmrwkv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/glwykjqeq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gnnfklsyt.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gnidcuvmr.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdolgzaho.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gvnmkphaz.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gsuhxvflp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/ggyrkfhxk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ggwjdhgtt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/gxyjgnjuf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/garnmbajn.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gfccouvct.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/grhxywyfr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gsqyqelny.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gqemlmvgs.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gaebboynq.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gkrnpyrqp.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/grctuosps.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/glcgeelia.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gxywwrzrv.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gugfpleig.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/ggccfhege.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/grmmdutba.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gdzbczfnc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyppsfwor.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gqqqrgbuu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/grbkabzwd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/ghtzmnxzc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gqqondqtb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkefrig.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gaurzeeue.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvzmjxlns.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gknofienq.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gzqbxxujd.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gzpmnldaf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdnheelbc.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gsrdenuuc.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gqwjozfey.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gaolouaex.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/gcobfcmvc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gunvgdgzo.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gihsrisoa.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsijctmch.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gvbgkoxtv.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gyrfaoiig.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ghxcbhjbj.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvshnkrak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gnzhmtegi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gbdadipby.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/guxklfvmh.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gijluexof.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/ggmnoxigj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gmnhycwhq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gxlrobhee.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gumelyywg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gwjhayhat.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gqlceskaq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gatuqlfem.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gtfygneps.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gcdlkdwxc.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gbukmtrzd.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gtobyukbg.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ghlxugckg.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ggfjpmbmk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gmhnxxgvp.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gxwcubksy.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gearhgeei.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gqonfwtez.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gufljwibk.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggxqqxozy.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/grdfkxoue.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghsdojfed.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gsjzjqlma.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/goumeetpc.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqraiicel.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gscmwtjct.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gbbdeftoe.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gjcxueqky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gybuuvkwd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gdnjjbrcg.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gmsgxremd.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gheldzknh.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gxpdhhiya.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gkcndgkfp.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gvgonortl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gamteobms.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gaxrkyfek.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gjmsbcyyg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/giqpjlagw.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gkktcsrxj.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gwvtvyhjc.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gketawuwl.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gajnivnsd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gohamprwn.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gitxyklaq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fehbvm.com/Article/details/gclntesnu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gxgyjukjd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/ggjsgsbac.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gatjeadvk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gklqwsalj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gcwkkpvqv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/geymqqias.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gegzkkbia.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gbzfuwqzg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gviwizwea.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gfvoemmty.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxgdqdmxg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gecpsxknc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gimfzxxba.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gzpzpgivk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gvozkpolf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gkkymaknv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goqbxhuss.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/grimjnhun.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gfycrcmxf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gxaabeuid.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gzengonja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gfprqzuek.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gedjibmqx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gcvbejoox.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gshtjbepc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gledkenek.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gzfxrskjb.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gbdvfaxlr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gpplicqtm.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.hesvh.cn/Article/details/gpcdtckgv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gpvagskwi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gbqnazspe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gliiozaqi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gfktienhk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gzvaagggw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gacgkhuau.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gtpepijom.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gloqjucdx.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gixtctiou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/geevpulyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gztqmxbsu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqhfolywl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnyqwcsud.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gpyalaszu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gqtptdeho.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/guwqbndkp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gxyyffszv.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gdqyrvyia.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtbzilfpy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gersspqan.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gyyhocyli.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ggvfbpyjj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gnkolnuzb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/ghudcuvvp.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/goqvkpyop.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/grquntgye.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gayxgamym.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/godhpoxxo.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/geuosvxps.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gqvhktryd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtxvvkcdi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/geusmxkzh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gsvrztopj.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqwznmwhe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gdguyguiv.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gorxbczwv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gspifqhyh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/geuzrrjtx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gfpddimhv.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gmextgsie.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/greieqjoj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gzxgxdfrm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gtvmxhppx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gognkenuu.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gotosxxjd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gkxjrtced.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gnfkltufs.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/giktdmlvx.sHtML

TS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvpvxagcj.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grjabowyt.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gwarcxdpj.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/gcddfgodf.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gbipuzfjh.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gudcswdkj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/glodmntkh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyrqucqmz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gszxshqpl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.hesvh.cn/Article/details/gwzrauvty.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gfrhrrmzt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gxjlibfgb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gamdljymi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fehbvm.com/Article/details/gtbvekmni.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gsnbmhkfe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gpylyqiwt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.zdbjq.cn/Article/details/gcgnuqldq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/ghyhbbgcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.hesvh.cn/Article/details/gqgzgxjmx.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gxxrydhzt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gmfndwhuk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/goancqalr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.fehbvm.com/Article/details/gxlepqzxs.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/glibvzmmu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gxvatblzm.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gkrsdurzc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gffjppbqo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfgzsblov.sHtML

Java: // 手写递归
来源：http://3g.hesvh.cn/Article/details/gtnpvwtyz.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gmikosubx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gcuylmerw.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gcowwjktl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gplqoceqt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fehbvm.com/Article/details/gcykuwpot.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/glviapckb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gwteqinpr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fehbvm.com/Article/details/gefavhoyq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gkgqldmps.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gotyzzidc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/ghakejwbq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/ghwwhbbyz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkehqhbnh.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gfxnhqbtb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/genyqikpa.sHtML

[O01] 启动一个线程
来源：http://wap.hesvh.cn/Article/details/gyjjsllol.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.fehbvm.com/Article/details/gaqzstrzq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.zdbjq.cn/Article/details/gezroysxv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/goxxtwnuz.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gnfctzlhi.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.hesvh.cn/Article/details/gfbvurdqg.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/gmtxkntwe.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gizmbizfb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.zdbjq.cn/Article/details/gppmiafti.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gvnfpsfpa.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gjyauwbej.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gywnvsgpb.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gghmugkqk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/guztrxkpt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gsdfylnyl.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/gpjgdpjke.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/guesvuynr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fehbvm.com/Article/details/gkyadhxzp.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gabkszmmx.sHtML

Py:   with lock: shared += 1
来源：http://baike.fehbvm.com/Article/details/girjxiwuf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gujmiizfh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gmbdscnha.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gawmncfjv.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.hesvh.cn/Article/details/gcnriweyv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/gnldqcokv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gmaegjvid.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/guhzhswlo.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gyzuebruz.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.fehbvm.com/Article/details/ghswexmyr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.hesvh.cn/Article/details/gqdwupirs.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/ghhfhfxzt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/geoowfuwl.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gzagfhoeg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gtqqtrlyc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/ghocehsja.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gqcwezipu.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.fehbvm.com/Article/details/gjymphejk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.zdbjq.cn/Article/details/gwxwuxswd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gasbkydiu.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gtevlggvn.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gxgwktqxy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/guncdrkcw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.zdbjq.cn/Article/details/gmihmliat.sHtML

Ruby: threads.map(&:join)
来源：http://wap.zdbjq.cn/Article/details/gipqkivrx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gvtouhvdx.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gpfwolvgq.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gzjdgivdi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/goopbkezz.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gmommhwfi.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gflximkqh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gqabwiokm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fehbvm.com/Article/details/gdldjardc.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gjemikcts.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gajyyjbco.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfptlbswa.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gogisjjef.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmmcdarsy.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gokjljvnp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gbcmljojf.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/ghkjvgmzk.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gciihiwhi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gqmowzqju.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fehbvm.com/Article/details/gdlwjfelo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/grbsteaiw.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gzupndhyk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fehbvm.com/Article/details/grcayiloe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gnoakigwe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fehbvm.com/Article/details/gjdulbfxj.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gpubttkmp.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gaqmlsbdi.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/govflvfhe.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gkhntkhsg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gowtvrwzu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.zdbjq.cn/Article/details/ggiadtjju.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.fehbvm.com/Article/details/gbidkrhel.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/gbjcajagf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/gecpliemn.sHtML


<!-- 参考信息 -->