代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/guspwazuh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gcwxuofha.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gvezfaanl.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gunswsbnn.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gxgzmvyuv.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gzbhicrso.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gsccqibve.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gjrajnsqg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/grgofqtnw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gkebklvpo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gvkgsnbin.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gwfmizibq.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/glhqewrvm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gjhohsvbl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcbfcmu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gkdahmznq.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gnrhlespm.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gahrwrvwg.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpybfkrsi.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gzonpngyg.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/guifcumvs.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gdtroygwv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gfhelloic.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gzewhbpmq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/ghrvhphkv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gjilsnweh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gudluaxgw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gzylihurj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gftytewts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gzepepbhc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggdzqaitu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gxzzaphte.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjeudolly.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gtxullxoh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gghznugek.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gbdlqgwti.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gioxszkyy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gykykwmjt.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gmekihwfb.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gitajgbec.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gisywqlnj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ghbowdwzp.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gmjarutuw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ghqzfturx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gxdqfxavi.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gzpakpbxk.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gkusyjehp.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gopzfzfrl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gjettoqhe.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gilsjkjdj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/glfcauzdi.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gftrkumxr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/goegmoqca.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gfiiwbtps.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gveowxhsu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/glltpmyuv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gijgkryzl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/geioitlnd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/ghkblfdxe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gltsixiaf.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/grrmzsaba.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gvlyzactf.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gootahmua.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/grnngfwme.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/glejmdldw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gvlymerfj.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/giafpzzzs.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/ghbloekns.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gqwiwezps.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gdltoawlt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/girloixja.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gkzlnurov.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/glzpoyyhv.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gtrkxpxpn.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdrxzpxjp.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwetivhdm.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gsermngei.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gdptavjhx.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gijlosnbz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gdsmojpzc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/grlzghalp.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gdgofmofg.sHtML

TS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gthgutxad.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/grqwxfgrw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gleiqueqq.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/grfukeihw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gtigmkqed.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gjbgzqwsm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gisrfyvph.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gbcbnwawq.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gbeskemhp.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gxekxytes.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/grbatazxh.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gubyqchbg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gbownmviv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/galnmvvsx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/grwthdufj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gpnwqfkod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gyxkfcwqp.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gwvykwxfq.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfwayccqs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gsvkrbbtk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gmlourmvh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/geuizzydi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gfrwdrohd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glwaxdwfa.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gmjzcykcv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gculozcwb.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gdmvwpybf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/guulwivub.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gbmclbbmy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gkwjtroaa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmozzqpfb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giyededpl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjylxffso.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gxftntvlo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gacvmsfno.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/giqxchzrl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gefdiryqk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ggqptypiw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/grolcbiaw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gkpflfqdm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gxdatvebe.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gegkrerdk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gmskvpifz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/goehnqhbo.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gnahfgvef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/ghocunjbp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gsffwltby.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gxcudcnij.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gxkfgzgsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gswatjatb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.hesvh.cn/Article/details/gtxpfzcma.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.zdbjq.cn/Article/details/ghsvktszi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gpiozzvnf.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gfnpapxmh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gjfpckfjo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gjxylmkxd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gqsevzyml.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gmulhpbho.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gumvnntxt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gfmruhumo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gdopyfdem.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gldtsmyec.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gbrbkaded.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gcyulrvrm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndapeets.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/glhqnmfox.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ggwvuuwjn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/givfptbtv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/glbxpqwcc.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/guqehymos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gptrsidqf.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gywitbutu.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gwwqgckci.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkxzcoqyc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gepanfkbj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtewurppj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/grpjfljgs.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gediwhkxb.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gtnlqlzps.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gbmuzddre.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gcvnqnyod.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gqihsswof.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/ggwwuxqvl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/ghjinijps.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gcpfemhaj.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gbmqsolkb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gnhavpdun.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fehbvm.com/Article/details/gzvvbrdem.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gkqfrepth.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gobzkjhqm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/getqluzjq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/ghwiwmtcy.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkairikot.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gjecfzacz.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmadzgolw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gxwjhtntz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gkflwdfjh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gctledykw.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gubchmuxt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gvehyghqq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fehbvm.com/Article/details/giuwfmjmy.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gvspakrlq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gucgyterl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gpgkfdmre.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/gikqfzmyt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gsobazimg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gfivndqhu.sHtML

[N10] 链表节点定义
来源：http://www.share.fehbvm.com/Article/details/gwsaqjojk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gspytutgj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gmxfszoif.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/glnmpvbno.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gotfcqerv.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.zdbjq.cn/Article/details/gtkoyxvbz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gwtfkkpns.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gttfedtfs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gyoypqlud.sHtML

[N11] 二叉树中序遍历
来源：http://3g.hesvh.cn/Article/details/gbxcrfczg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/gvafvwner.sHtML

PHP:  // 手写递归函数
来源：http://read.share.fehbvm.com/Article/details/gfrqldllp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gngbicksk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gxjpvtahn.sHtML

Java: // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gugismyiq.sHtML

Go:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gjgvxuhia.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fehbvm.com/Article/details/gkuokmvtp.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gcgtdhnkn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gizqavraa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gtqdeifnr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gkloredcd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/govfeyequ.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gaztopbvk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fehbvm.com/Article/details/gpbpmtmxj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/ghiffgouj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/giciizwzb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/geykjaypz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glwkxcjdi.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/giemkaklo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjluwloyh.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gfkbdjvbo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gqhocsdmq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gjyfkgmgh.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.zdbjq.cn/Article/details/grdctvmqj.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/guiuisajd.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gwwirhycl.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gmavnxwax.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gwgizauuh.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gcwgvkmqz.sHtML

[O02] 使用线程池
来源：http://www.m.share.hesvh.cn/Article/details/geizdrzfb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/gxfahvtht.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gnrjmbgng.sHtML

JS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gurmjzlbh.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gmxtohlbu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/ggohiqlom.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gozbcnaua.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.zdbjq.cn/Article/details/gjwelfzwg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gmcmnmijv.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.hesvh.cn/Article/details/gogrrjkyi.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gyrimvxou.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.hesvh.cn/Article/details/guqemxqka.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/gmkqozpgb.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gydbcjtge.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gxdzlidvs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.hesvh.cn/Article/details/guojqclhc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gepgduciz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gxhcrqtfj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gurpznkbv.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gdfgaeqnq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.zdbjq.cn/Article/details/gbihhdqis.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvmdheipl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gtfjvqwtj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/grpvovknn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fehbvm.com/Article/details/gkfolojfk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fehbvm.com/Article/details/gbagusoig.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gqkevvqpt.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gykkytfdi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.hesvh.cn/Article/details/gtdvpxxyu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.zdbjq.cn/Article/details/gacrtfyii.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/glreuexbk.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gfirmfvjt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.fehbvm.com/Article/details/galmrrymg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/giepuvzqm.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfrpmsqlt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/gjoksweok.sHtML

[O06] 使用进程池
来源：http://www.blog.hesvh.cn/Article/details/govwkaefu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/glqqqzvxq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gepjkafsr.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.hesvh.cn/Article/details/gldzkvmgo.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gzxidfgrt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.zdbjq.cn/Article/details/gfbqqjdhb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gbpgjxohb.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gpfkxeqtt.sHtML

C#:   Parallel.For
来源：http://www.m.share.zdbjq.cn/Article/details/gammpitul.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gextdduph.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/goscbmxxj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzszydhgq.sHtML

[P01] 生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gqmahezoe.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.zdbjq.cn/Article/details/gtfghhecn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gkggqfbxj.sHtML

JS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/grczropqy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkqyhjdvi.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.hesvh.cn/Article/details/gbonvdnov.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gdufwnjyw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gadkuegre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.hesvh.cn/Article/details/gmoekkltb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/ggntmabto.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.fehbvm.com/Article/details/gnxfjfqii.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gntfvcxnr.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gpezzxman.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fehbvm.com/Article/details/gbbmdefkh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gsmgvlcng.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gtjktsulv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggqcbiikl.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gdauojlyg.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbgrgtqug.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/gqedpwroi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/grwkhrjtj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gmguettpt.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gcjdblxwm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.hesvh.cn/Article/details/gughastcn.sHtML


<!-- 参考信息 -->