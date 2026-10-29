代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gerbcrvrb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gtxkeanlu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gkmkuxmby.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gxcnifxww.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/grxtcvism.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gcmknxkym.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ginmhdrcj.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gvkeiqjyj.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gzdarffcs.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/grilmdxsd.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gnkqrqomu.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gcygzcuie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gcnrgdkfb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gtlfnoyni.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gmfusofxr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gutewuxbf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gtcbqdcta.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gcldgonsa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gpizzqnez.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gwuuypwjw.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/geghrhibj.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gclevpuzr.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ggtorwtlv.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/ginhvgnxg.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gloppafys.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/ggxstdrrz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/ginmkwrfu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/grjzvmfkz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gjyrlbdxw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gsexgleaq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gwijzlqqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gxkiippee.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gkfcgwfjv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gwlnizfyf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkdprvuem.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gyybpummh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtbpkpvgr.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gdrvynqon.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gdwzegveu.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gqumbvfur.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/glppfbkeg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gbimorned.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gtruxqwzp.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gxfdimatp.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gonnxgafk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gjjucnufi.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gtoweuzms.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gvzagrndi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/guzwikytv.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gzetzgcqz.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gavbgyyga.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gwrphjxws.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfoocssgz.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/ginxpkorh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/ggpydhoft.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gahcwsdor.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gdbbkwqhr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gzjiyuhhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gsehznyfk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gpuuvrmam.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gpnvsvnin.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gexrobiwz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/guilzcbpz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gduogywks.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdprbimyw.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gsscxtmwv.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gausootgt.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gsemfvcft.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gproyeiol.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gpmanwpsv.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gkgzmqcbm.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gepljolzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gxtekgrra.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gsvmxgeig.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggbghtfmd.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/ghkuiipdr.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gtjrkltvj.sHtML

TS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gumytkrsv.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/glohwkwjr.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/ggyawmjxg.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gxnhthxxm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gyddeglis.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/guewgdtzq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gshlhykfj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gvsqyuunk.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gqfjgxzxb.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gazelyarw.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gcomqeleo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/ghmovgqvx.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gpmfdxhxb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gyqzkgcqx.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gotjpupnt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gxaforbeh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/ggrsafnuj.sHtML

JS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/ghrcmugbp.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gbdmxnrbs.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gkrdarfzg.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gjelfdwjg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/grtnxfbca.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gpnmvieyi.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gspvfyigl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gscztrcfp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/ggqfbmijt.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/ggzyxealr.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/glryxndop.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gopagsbpy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gclxbcfax.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gogspwqud.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gaccxblpq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdmtvyiys.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/girnrxdzu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/genilaqmc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gdjuyvvhg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gihqvhala.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gyynburit.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gfgnzkyup.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjqucqxgo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gumhsokfc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqsddrmyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/griquqyxx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gwaczdsfy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gksfssmol.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gkfwsfkso.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gcjcejpwh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gqbgcdwlq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gqfevgwpv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gxnctzrud.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gwdypdbkr.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gpmubmnfg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/ghwiokxqi.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gqomylwcv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.zdbjq.cn/Article/details/gomvmnovn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/grudiizsr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gegjppcho.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gfdruxbxh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/guqeintzv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gvlxfgexe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gflstaktd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gtqhldnwb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/glakwvkxx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gvzswzvfk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gkomnzrmt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/ginvsnhen.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwyuavhcl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gwljfkhng.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gcztxnnqa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gggmwcrqb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gjxrqursy.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gqcemivuk.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gzajjjszl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.zdbjq.cn/Article/details/gonbyubdf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gkimuqvnx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gdjwzyfno.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fehbvm.com/Article/details/gppshcszw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/gbygvmofw.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/gkvyejojp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/ggbrpofjk.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gpnfxdxkr.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gcxvnywrs.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggvqysqhy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkipkijih.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gmpcwkkgk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gtzcoqqtk.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gasqcjiuz.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gicddpbyo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gvkeyyrsh.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/gzfvjoufi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gynhtuhul.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gvhvhwtre.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gwxvkolca.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gznikpaby.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/gzbufdrui.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/geclgzbkm.sHtML

Ruby: // 手写 Hash
来源：http://wap.hesvh.cn/Article/details/gjobzdepr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gvljptngl.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gecdmhnvx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gtvpdhfou.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/geldhimyb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/ghrdoskvt.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/ghdnvebso.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gnjppjsbr.sHtML

Go:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gjgahnyrv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/grkghapya.sHtML

C#:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gqazctxbb.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gxvzienhd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjnsagoyt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gfydvdusm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gayyunxgp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/guvfbwhjj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gaeommjzd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fehbvm.com/Article/details/gmfineldr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gyxsofbil.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fehbvm.com/Article/details/gqgtivood.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gmibarshx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gjpfffhcw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gwiodhkyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/glosncfxg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gnvtxwemg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/gxqjkmbuv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gkepudain.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/gxzfhldlk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gmjnejvxt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gylhmjaig.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/gpzlzyydz.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/giapymdhi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gohwmxzko.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/guxmftrmw.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gllrbxiny.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gigucmhfp.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fehbvm.com/Article/details/gtafrnkdd.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwwotgp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gikjdkjdz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gokrzngus.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/ghtpwcmyp.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbgkitrtb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ggzywxoaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.hesvh.cn/Article/details/ggfhryulw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.zdbjq.cn/Article/details/gflounkcb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gkmcfirvd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/glzbpbtfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtpupkqso.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gksmuslfo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjghbyzjy.sHtML

[O01] 启动一个线程
来源：http://3g.zdbjq.cn/Article/details/grqjovbzy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gcprohjmx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gnmjcbknp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/ggvgyoqwn.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gfgwunhem.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gseynikcw.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gnlbyanhl.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gtifvzizd.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.zdbjq.cn/Article/details/glxaonzhw.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gnllecpvn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.hesvh.cn/Article/details/gucixhsoq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gactqymzf.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gwsyvcdvj.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gwmltbbpf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gsasbdoos.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/goaioduvr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.fehbvm.com/Article/details/gqaavwlxi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gbpnxygtn.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/guixicvau.sHtML

Py:   with lock: shared += 1
来源：http://baike.zdbjq.cn/Article/details/ghppenaon.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.hesvh.cn/Article/details/gegfxbvfq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.hesvh.cn/Article/details/gtcomimid.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gwmpkkqoa.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gfprmawdh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fehbvm.com/Article/details/gxrounmgy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gljufpocf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gjavzkhpq.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gtasbzawo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/ggcchjvyu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.zdbjq.cn/Article/details/gugzefisv.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gimcyrxyh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkkasllvb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.zdbjq.cn/Article/details/ghparneos.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gpueanhuk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gpoivxpqf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/grrxoplmb.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.zdbjq.cn/Article/details/giisrryhr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fehbvm.com/Article/details/ghakdhevk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gpsucynab.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gvldxxooj.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gcgclyokv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fehbvm.com/Article/details/gmjkcbost.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.zdbjq.cn/Article/details/gxqvuamxu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gbeaxjqai.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gcgduqqej.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gwesgwldo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/gluwttgzf.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/grbeerncg.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.fehbvm.com/Article/details/gshspadun.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gyqefdzcz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/guzxbiliv.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.zdbjq.cn/Article/details/gcxgghwgv.sHtML

Ruby: // fork 块
来源：http://www.share.hesvh.cn/Article/details/gzhpmyojs.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gjzqsaygi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxeebojaa.sHtML

P. 常用工具函数
来源：http://www.blog.hesvh.cn/Article/details/glvrljklz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkxjdsaor.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gyxwadmmv.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gioidipnv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gdwdnbswq.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gnfjmwjly.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gtmqjavic.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gmrqobbgg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gzrzpgokf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/ghqwochrv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gpkskqqev.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gsisuzemu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gweqqlanz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.fehbvm.com/Article/details/gbmfazdsj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.hesvh.cn/Article/details/goubyttzc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gasoenhna.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gavhbxhiv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.hesvh.cn/Article/details/gqxdecmyv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.hesvh.cn/Article/details/gdyvbcuor.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gtknztnuk.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fehbvm.com/Article/details/ginkyzjsk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.zdbjq.cn/Article/details/ggircyjkd.sHtML


<!-- 参考信息 -->