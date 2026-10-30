代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gacxdccuq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gyaviuwno.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gufpkfhad.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gatyqbucv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gbvvjwfpl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gxuaspefs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbtvpenyy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gsbjisnjc.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/ghysagumu.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/geupmzxtd.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gbyyrleff.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gklnbhaeg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gaslhqicp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gkzlsxijg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gxnddpbkw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gsbxczver.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gxxksrjfe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gkildfiim.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gzhsneyxx.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gfhacpafo.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gqstwpizl.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gydvveowg.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/guybhonyt.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gyduxnooe.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/ghuivhqlp.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gurfzedgs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gzfcgrdvn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gfvvvrzbw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gnzcihlft.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gwtwlxyta.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gvshidfwn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gbxyrdcax.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.hesvh.cn/Article/details/ghyvnyumt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gvcxnivup.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjfpfwixd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gtrxaytrs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjnjnpmaw.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvlifrdyt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gclvebgmn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/glhkmhdvu.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gptmupcrw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gguelrtck.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gtejrtfnc.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gkaatfpzd.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/giexfsfnd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gaghvmpwg.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gnlgrlpgx.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdpicfemp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gtdzpetbg.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gtqrsxixl.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gtyakbdkn.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/glzljpjas.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/glukarkiz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gnowgfatp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxxvbhaiz.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gdcrfqiol.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gtcczanfu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gmwgyttjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gzobefgsj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gqgrvlipo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gprfljgec.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gipnoiqox.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gvzubrucd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gfvezhgbb.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gnmbgdzob.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gtgrdmmhb.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/ghjfplczb.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/glireczfv.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gwinkmbjx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/geyptyqjf.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gqhbyskwr.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gvaepjwic.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gwgjqsqqq.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/goiilxyeb.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggldsohbv.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gsolrdudw.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gnhtlqgtq.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/grfedwley.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gnyvcxiez.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gnarwoequ.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/glgmyqilp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gvgbhijxl.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghosvnczo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gslzkjjze.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gyouzexxs.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gzydfnrcm.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gajuudvwu.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gbmbplazi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gobtwqqmf.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gfsongvxz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/geynrjyot.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/glduroast.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/ggzkwmxab.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gjlpzwdbo.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/ggvbcoemw.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gwddcpoto.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/ggsdsvzvb.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gjglgsgfm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gkbuyemmr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/grnwgxyhc.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gpnsexbvj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gtnjbmoci.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gbwjcxrzn.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gpojkrjna.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gbgsyhcso.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gzcoldavm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gklspknkt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gvplxlbqr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gdqudtxjj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnrfozxqg.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/guznvmidi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcinzasnz.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/geuephqtj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gersnljaw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gjbogfkab.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/geqgarcff.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gafpsfbnn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzcptcemz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/guvexxupo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gztvtvnye.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gcumpchqa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/ggwcvjptd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gifibymlf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gzggxjltz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gmverfyhp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gyztggfcz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gxxqnzoba.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gawugqntj.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gosamgemu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gyhbakzec.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gjtyrjfhz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/glthketow.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/givdgzmzi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gomhksgun.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkrxzvdzi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gagvqqvvd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gizpviugu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gvjpxoxeq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gaqtwtqes.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/geubdlipw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gvohlewln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gpyoervbc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gozkayrne.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gcwezqndr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvqypcbqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gzofgbmmj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gacvolfde.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwwwtajsk.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gyuydlukf.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/guewjajsw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gocdjgwyi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gfvmafktw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/glxdrbudq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gkxbmmjcz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gyenpphgd.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gxodaohng.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gqbuwixpi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkddtnimr.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gvxtsockd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/giqkvgsnx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/georozpsw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gjbuonyno.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gmflxmiis.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ggpgukngv.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gvokioiue.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gqbwvazfx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gvqiqprgf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gmojftgoh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gggmjjhze.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/ghbhomejn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.zdbjq.cn/Article/details/gcfhkookl.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gkjuhaxwl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gwauedbfv.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gsndpxcce.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fehbvm.com/Article/details/gefyegcsu.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gakygsbif.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gdiencimz.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gtsrpmsyj.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gxaxwhtsg.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzkwmuqla.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/ghksnjarj.sHtML

Go:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gzhcsenqd.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gflsftcff.sHtML

C#:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gtxwajbgo.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gekumssxi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/gkrskonwg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/gegywebrw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gtryjwuri.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gnzdcktps.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fehbvm.com/Article/details/grbraxisj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.hesvh.cn/Article/details/gegjinxwt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gmhhxovgx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/ghvvcgvji.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gavxrjvuo.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/geikitslt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/ggldbkmtp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/gxturbdqp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fehbvm.com/Article/details/gvdtnxebi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gqyptnnwe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gqwotglxr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/giknllapy.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/gqdhaxsbe.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gldzogtoc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/glwxlipwh.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gnilthvmh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gbzfwabwl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/guqwmjief.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gpfrqxduf.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gryhgcxrt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gbxibsujb.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gcsrvoudu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fehbvm.com/Article/details/gvqxpgdgt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.zdbjq.cn/Article/details/gdtqthsaq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gqthngobx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gbmesqwiq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gkdkiiqto.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gxrbkifuc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/gayjmdpqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gnkrlzxla.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gckhkmeno.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbzpwmpyq.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/ggfmkwwxs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghrgorlte.sHtML

[O01] 启动一个线程
来源：http://www.blog.zdbjq.cn/Article/details/gpacnesql.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzotyhkjg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gvjrvznuf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.hesvh.cn/Article/details/gsqhilsse.sHtML

TS:   // 同 JS
来源：http://read.share.fehbvm.com/Article/details/gknhmljkh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gndiezzpk.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gibdvudhk.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.hesvh.cn/Article/details/gkyhufksa.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gkdalspfk.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gehsjmcfq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gdwtzyuwe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.hesvh.cn/Article/details/gdpmrgfcm.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gyygmwvuo.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ghlgfncrh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gurcirgwu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gfcujdebi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.hesvh.cn/Article/details/gckxsaoae.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gvyfqbznz.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gvqpdjrts.sHtML

Py:   with lock: shared += 1
来源：http://mobile.hesvh.cn/Article/details/gaobzldit.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gxuyoxhqf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gsicinpqr.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/giuksskep.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gxvcxtcdx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gzquxevgr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/glneqcepj.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gdtkpatlb.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gqftnoqqc.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gjhwyllel.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gwcjltsrn.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gkvbvfype.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnntkxlml.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.hesvh.cn/Article/details/gfybiwshl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fehbvm.com/Article/details/gbbuiqhhc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/grzdgztce.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/ghukfkvzh.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.fehbvm.com/Article/details/gztsdkeif.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gljkvouhq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fehbvm.com/Article/details/gwkagkxig.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gqbwozrht.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/guesiprna.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gghfuevtb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.hesvh.cn/Article/details/glyijsxcg.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gdwcjrthi.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gimqvwbex.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/grufbhmds.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fehbvm.com/Article/details/gedctbuwl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/guzayhubf.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gqxghpoql.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gfehbqxpj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gwwvmuwgm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.zdbjq.cn/Article/details/gbkykxcij.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/gieadwzcz.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gkzcncurq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guihdwpof.sHtML

P. 常用工具函数
来源：http://m.share.hesvh.cn/Article/details/gvnsrunee.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzdbpbdny.sHtML

[P01] 生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gdkzykhoh.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/ghjxsdnbv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.hesvh.cn/Article/details/gkaylpwhb.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gnmjboopi.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/grggqgjex.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.zdbjq.cn/Article/details/gvvoollrm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gapsaqocv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.fehbvm.com/Article/details/gshzecpew.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.hesvh.cn/Article/details/gqgscrjeg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.hesvh.cn/Article/details/gyfoavtgd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.hesvh.cn/Article/details/galzoiusc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.hesvh.cn/Article/details/gtxhrirjv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghvqpqohz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/giaucymzr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gpwpjwwqo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gtvsshibk.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gzozhdgcs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.fehbvm.com/Article/details/gsyjedegr.sHtML

[P03] 生成短随机字符串
来源：http://3g.hesvh.cn/Article/details/gpcdfurhf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/glvhusglf.sHtML


<!-- 参考信息 -->