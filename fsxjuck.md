代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gmlksmyxz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/guqqkupnh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqnhebafn.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gsgfcrlzm.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzmntmhtd.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gvsmfiomn.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/ggsxiugaf.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gglvjikae.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/grdqjkupi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gprkiqhca.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gzzggtrus.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gzppabmyo.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gzrscayae.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbaxtiwas.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gdikxaeuo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gfuxsrhby.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/guspjkfyf.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gldhxuhda.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gnhmdntyl.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gussnpfyx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gnfqtaubr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gzfkqwkxr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gfdypaojp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gevvuihwt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gryxfjqle.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/giqfbfwhd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gvtayodzb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gplizuqys.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/glsbqyqvd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gqvbwnpuw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grmaxlmkr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gawsogsoe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcgbwryny.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gkpndqfrk.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gtgrifycy.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gvxcbwwnl.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjvjwtuaf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/ggtpgljjt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gsdphbkvw.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gltvfogdl.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gojyvorki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gzaqbphce.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gqjrvanzy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/grbcqhvoz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gesmhouig.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gmidnqcqq.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gpregicsc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/goflqnscr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/glasmzegu.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gxyzfjhfd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqtwecesd.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gflidtzht.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/ggmnlnnvh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gvfkkwsbg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gpprijkkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/glbdnmxsz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/goornhjww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gdpoyukiv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gyakginek.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gadcptnka.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gjtfdraab.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/ggdifotvq.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gaseuunqq.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gwpzjefpc.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/goqmrtvgv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gujrcvvzd.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/glcunjkea.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gsvwddcwx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gtvotisfo.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gwswgkfdx.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ghlaqknia.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gwnswbfwo.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gykfskbjv.sHtML

TS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gctltmnft.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/genoqdomu.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gtiecnnul.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gbzqtookx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/guddufdjo.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gjszfgzqh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gsiscudtf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gjhpcujhb.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gfjbltior.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gahwibewm.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/grijyfjgu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ggarqcnpj.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gycllzfxx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gdlnsdgdq.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/goybglnne.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gknghfnrt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/ghpieeulq.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gdvnlbcex.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gtyfxnwim.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gpudlmhrs.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gewazxnvd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gdfmgvbdh.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gkumfmdef.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gasqyxgwh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gyrgmsmwo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gwlimbqze.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkdkgwyhe.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gsycetvzu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gmhnmqbjq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gmzpyvohg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/ghglrqmxk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gizipsojm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goohgloau.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gyldebtdv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glxrwzszg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gjwyipzme.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ghctrfdkm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gjszaewvi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gemfykgug.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/goffnslvj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gwcojgrgy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrwescv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gdvjbqkxd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gyaxrwoyu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gxtaikrco.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gptnyqjur.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gclfnyool.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/geedtgpob.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gmhyasdgi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gloalftsw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gsgmkghfn.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gxoyzbgsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/gvkpjfunj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gmxacebgn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gorxjlnhl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gffadoelp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfcflmloq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/guadmtjqt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gqodprrui.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gxguhmalv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/glhiykovs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjawnwrrs.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gozciurbp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gkfqlrfhs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/grorglfov.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gnnxjxbjk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gadinudrk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gxwmsvxli.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/ggeohsebq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gxdkylyju.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gdlihfajo.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gycyxtfqp.sHtML

Py:   math.gcd(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtoxxmagt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gootvuaim.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gzmnhljhw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gsnelmqjf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ghgqxptve.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gblvdvapf.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/grmvenjls.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gvvnznvce.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/grewmfjog.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gwacuwqie.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gydzedtfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gusgzpmsa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gycgknxxz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.zdbjq.cn/Article/details/gbilwztso.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gofpntqpb.sHtML

Ruby: s == s.reverse
来源：http://read.share.hesvh.cn/Article/details/gfwvcmsns.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gejsoenjc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gwncaousy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/ggyzwkoad.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gvslmyllr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fehbvm.com/Article/details/gpwhjqwsd.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/goimonybc.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gyewkcbra.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/goyicomjh.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gmdnztyob.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gecdezihn.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gabruzaff.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gelnirjtj.sHtML

PHP:  // 手写递归交换
来源：http://m.share.hesvh.cn/Article/details/gjmgegayu.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gpwartttm.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/guwtzfxja.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gvywgpjiy.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmngqccbf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.zdbjq.cn/Article/details/gjdlyjgsd.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/guoryykkz.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gguxgdvdi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/ghordfirp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fehbvm.com/Article/details/gpgpnwyjn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/grugvwdqo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gevpwyveu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtkrronyv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gwtoyjjml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gteaxjdsa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gdifkjqjf.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/glgwemdor.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gaxmonvjl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gqnnsjoss.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.hesvh.cn/Article/details/gkphhnlwe.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gnzdoshlo.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gjvglqwmq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fehbvm.com/Article/details/gbrzostwu.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.zdbjq.cn/Article/details/gfsogiqjg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.hesvh.cn/Article/details/gugqztrqp.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/gquyzeifd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/gahdyqqyl.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gyzbmqhow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gnzswtetl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/guqqmukdf.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gmkxnnvsn.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdpbznxuo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gnptkjlku.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/giiwbzykp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/gdblcbkfd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.hesvh.cn/Article/details/gtmrtlunk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gdkifnwmk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gvjlyqhyu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gnhujjzxc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/guxdjwvyb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gdajrwzpi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fehbvm.com/Article/details/gyxvxxvog.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/ggainwsod.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbhswrzcf.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gvtrwudgi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gccezxvbb.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gcsgkvjir.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gntoqfckq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.hesvh.cn/Article/details/gcjauudqd.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/giccxilbn.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwrcayqrf.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gwqcfcxew.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/godyeljzd.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/glqoktenw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.zdbjq.cn/Article/details/gykioexwp.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gxkvmkwkx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gjwivzojk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gokohulxz.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gzlvrlskk.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gmicdnvzt.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.zdbjq.cn/Article/details/gzagpepqb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.hesvh.cn/Article/details/gtxkxgfzt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gpmpgvfim.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.zdbjq.cn/Article/details/gyzeukimw.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gpfwexvms.sHtML

Py:   with lock: shared += 1
来源：http://m.share.fehbvm.com/Article/details/gyjljrnvr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gnirrwoul.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/gjmlzmgjg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gdsucqsaw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.hesvh.cn/Article/details/giipqjzac.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gufnxsqgv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.hesvh.cn/Article/details/gvhcfevai.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gyevddfqu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gbvkpxila.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.zdbjq.cn/Article/details/gphbxiovf.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gxjprgbws.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gevczilgb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gspwngwkb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gvojwjvzh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gnewbstrh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gwgnjkfbf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.fehbvm.com/Article/details/gxcrwkhxe.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/ghbvejjjz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/guuedgvtm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.fehbvm.com/Article/details/gbxdsoosm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gjtbmqiip.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gombjdesf.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.hesvh.cn/Article/details/gkquyvvzu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.zdbjq.cn/Article/details/giwpfoduq.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/gqfvybpll.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.fehbvm.com/Article/details/glcbhutcs.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/gcuxsvxhm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gvgzvioon.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/geadlzmop.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gtqregpqz.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gpvsadjoj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.fehbvm.com/Article/details/gtfrvrmtb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gxawrtqgn.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gmmapmaga.sHtML

C#:   Parallel.For
来源：http://wap.fehbvm.com/Article/details/gqffphnvi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwxrrypdq.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gcuezaqvq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glgxdprjl.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/gqelvvqor.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.fehbvm.com/Article/details/gqazbjkpp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gpvbrffou.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/ghgojbmen.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gnxrkrdgi.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gengsopoy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gvqxggeje.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gpknlcagb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/gzbiuxhuk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gsnuzomig.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gduhrffwq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.zdbjq.cn/Article/details/gfkvainwf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/gcyocyicy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gvfjimhkz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfrksoq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gkanxqftw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.fehbvm.com/Article/details/gdynkhfsh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gskiyeoag.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/gsmxeinma.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gtufvtsfp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/gilqimsvp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/grbzfjcfi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gxplcxwsg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.hesvh.cn/Article/details/gqjozforc.sHtML


<!-- 参考信息 -->