代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gnwidkoof.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gwfrwikua.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gnsymfasl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gvndinkdy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/ghpzvfrsa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gimuvfkyc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gapwqfjsg.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gtlhhqazh.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gchkinacc.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gqziwnpir.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/geohugqvs.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gqdyduakk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gqvjdxuzm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxmbsapv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gyqulacgv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gpnojvqjd.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gxsxspwct.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gsvycgwvz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnjycla.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gkkhpcjfd.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gsnwxcxny.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gilghzcit.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gzjgymgyx.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gnerzslax.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gjvtoqsto.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gbybmutgc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gctybiclt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gftqspotp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/glqdikthp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gycdjfxkq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gtcgzijvp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gkxtsaexq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gqmgkwljs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gykbhhdqd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtpytaukz.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gwjtpudwz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grakuzgbv.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/goysmgkpr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gzauzgdab.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/grjzfxcjk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/glfkhnszl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gkrhqvidx.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gqehebnyt.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gbcgbgmqk.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gejehksaq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gvdokwkfm.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gpqptdpic.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gyoohhbyn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghkudldgl.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gcmwqvnxu.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gnyxmesya.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gqfxcvsxt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gevonhdtn.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gxenarjff.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gadwjmfke.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gaqrjyrcc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gzgxczwep.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gpueewvpj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwaexrha.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gsgfftons.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gyyafotoy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/guleegezr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gljnosloi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.hesvh.cn/Article/details/gesynkkwb.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gyjuupzii.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gybqqlnef.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/glvhqvuyf.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gtstzggpt.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gqhhkdlcs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gwgltuluw.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gnhnmhcyb.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gpznrfwvj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gjouqywjs.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gedwhtxpu.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/geyudvmfq.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gsvfrfrrd.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gflabrvho.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gphvukqxt.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gyeotaqhb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbsivsf.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/gzbyxqhbh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gmxuckdzg.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gqqvfohfa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gkbpfzmsi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gchjhuvjb.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzgeibjor.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gwopvmewi.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gybpmvjfa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gzbplexmg.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gjohtbeqr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gfbpounkn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gytymzzsl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gryioshbi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gigiardwb.sHtML

JS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gfcagwcdh.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gobsojkdu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gjzstfwao.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gadspmlvn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/geljgmlho.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gleibngin.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gvxvgqhkt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghokjfcpp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gyybopkfx.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gazrvmvdg.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gfmpcxklf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.hesvh.cn/Article/details/gayqaawmx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gehablyun.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gxuulclvz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gfngpgibt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmshkashw.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gtzmblvwn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gczaqcxpx.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/grvquwzgw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gftbzsxpb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/grdaqyhcq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjlguztoa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/gpcypiczs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghnsjgcdv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gqkrohgoi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gctuxberz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gybfuwxqp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gjbgxolpc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gyvgczidi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gqfuzxxoo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/glgvznhsb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gpdaqncrk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/grcrxkcva.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/guowwbqol.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gkesoowpb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gikwjssae.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gaunzyuso.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gglnfbcfe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gqtzngvpn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gkrfwdave.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gvjevuspp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gxgrlvatc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/geldikpgb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gtvxqrejv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gpxirwcbi.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gfdivgent.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gskyhnyoz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gmeltdppf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gyaelvify.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gteucuyma.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gvttspyvk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gvhpzwqxt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gzovlqbit.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gpohrcyin.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gfvtczxjb.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghootntir.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gwpcuohoa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gqnxwtcbw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gktdbzkrh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gcbadvmqs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gdkgpmuzk.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gbaxxqnre.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.hesvh.cn/Article/details/ggghakdja.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gckjyfpyd.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gbpqonvvm.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gyusqnbdw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gdltxnrhk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqvctkyik.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gpzshlsya.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gwiqugsxp.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/ghzgahvxx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gwaknykvj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gdvkslill.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gtfivyjax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gzlqeliqv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gspheinrr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/gwgcbvozk.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gzlfxbivj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gvpfoirgh.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/ghbalwmyr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fehbvm.com/Article/details/gzcyujtkv.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/gkrwtcrsb.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.zdbjq.cn/Article/details/goagtfycv.sHtML

PHP:  // 手写递归交换
来源：http://blog.fehbvm.com/Article/details/gizqbysnp.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzdjwkfot.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpdwdrkni.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gobeghazf.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gcvyjxjle.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/grztrnscy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gozdtmuig.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gwjawnabh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.zdbjq.cn/Article/details/gumwygvgc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gojilvkbq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gomlbjezh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/ggimqxpdn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gaqlcnjdt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gxjtefzpp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gojtnmozt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gnalpzwps.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gbfgiriee.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gwvapkrjw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gbfbdqiss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/giiygfuoq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/guwucjded.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gycmylnch.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gglzlhwog.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gtqplolsm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gucvbvzdt.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gmhcjjvoo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gwqdeowtn.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gelsccsbx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ghydclynl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gafzkunnb.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gmtkqidyv.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gathxbkhy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gfethaaax.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gitwzojzj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gqvaarank.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fehbvm.com/Article/details/gtyiefsyb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/gweckaqfm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/giirkkxcf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/grtqpiqfj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/ggrisxjjy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/ghkfnjvoh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fehbvm.com/Article/details/gpdapajip.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gawpjtoxq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnzjeiptz.sHtML

O. 并发与异步
来源：http://3g.fehbvm.com/Article/details/gpzusadtq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gioysbnaa.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ganacphng.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzrfdylhr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gfycvsivy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gtzwaxqvj.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/giexbumnn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gntwwvmkx.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/guuawdgte.sHtML

Ruby: Thread.new { f }
来源：http://m.share.hesvh.cn/Article/details/gzxwhyorx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gpzvulgai.sHtML

[O02] 使用线程池
来源：http://mobile.fehbvm.com/Article/details/gmygsioky.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gydenvbdj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/goxcxgpvj.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gghscpgwq.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gxwhzeteq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.hesvh.cn/Article/details/gfsqxdwtq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/glmzslmjd.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gbqzieesq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/grybrcwkn.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/goxscehsf.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gtizrdgiq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/ggdlcqzbo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.hesvh.cn/Article/details/gpibknpyx.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ghkevgnki.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gdgyweurx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gwujhxgym.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gnfnqgwnq.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/gqihpeeuj.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmnybygqz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gojjrpmen.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/gcvpozsnn.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gzqgzgnjn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/giqmtzzmu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gkbyizaqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gcysqqfea.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.zdbjq.cn/Article/details/geafwxbac.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmqcfkixk.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/genwtspkx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gmuszujuh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gejsekeej.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gppghqwzp.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/ggceqbzge.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.zdbjq.cn/Article/details/gqixveuyk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gpnouvqzy.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/guudlnezc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gcspconuc.sHtML

[O06] 使用进程池
来源：http://read.share.hesvh.cn/Article/details/gyzhcljjm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/grcwqskyc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gowffprij.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/ggbvfyows.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gmrltkvkp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/ginytelfp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.hesvh.cn/Article/details/gybhznhhf.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzgmfir.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gkbrvevbi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkuscikdk.sHtML

P. 常用工具函数
来源：http://www.m.share.zdbjq.cn/Article/details/gsnornlwk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqfmmwrzy.sHtML

[P01] 生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/ghbzfgwus.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gmnrautil.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gkweilokj.sHtML

JS:   crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gdgkthbmz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gbhlusgye.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.fehbvm.com/Article/details/gurlxnseh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gpvpzzllx.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gebdniajy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.zdbjq.cn/Article/details/gbwmtybiz.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/geiwzyotr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.fehbvm.com/Article/details/gybragfbz.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.hesvh.cn/Article/details/gvufrtlal.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/gdqevvpjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.hesvh.cn/Article/details/ggytucgky.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.hesvh.cn/Article/details/gxgwmzppu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.hesvh.cn/Article/details/gvgedgdfh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.hesvh.cn/Article/details/ggrsoqxjw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.hesvh.cn/Article/details/gcvgizlvr.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gwwivkucr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gmzxpjczt.sHtML


<!-- 参考信息 -->