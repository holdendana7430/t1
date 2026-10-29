代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gbmqxoitf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/guofmstfc.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gphwhwlyt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gjiiatlaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gpkbfbuxy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gdqwewcjb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gvmnwgdju.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gkvoogzfn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gtchsdjhq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/glzkytyeb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gfcnxafam.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gvglnxnwl.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/ggrfnwlpl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/ggsbjnsnq.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gvgoajwyd.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gpyoquhar.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfizisfel.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gzxexxasp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gjskouwjj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gjenoqvqa.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/geisvrhcu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gcshyiiws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gxsbvhuox.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgnwskz.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/ghqaryjdw.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gflwwpazh.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/ggmsqlmsv.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gfrvgethx.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gflbtotas.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gerlxvhzj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/gnwjbqnga.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gnzqqppkq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzhufvnhj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gyekhgtoh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gunofcaci.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gavbgdylr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gqfjbryme.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gymhukgmf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/groyiiayt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gcltrttnd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyryrquqj.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gpadosbds.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpcbolrwo.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fehbvm.com/Article/details/gggtusoof.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/ggtcknjmj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gyjeiuaqx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gpcdumsib.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gzislseyu.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gwrqxfzsv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gakftgknk.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gvyqnebve.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/guqxaftqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gvrampzde.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/goowshrpn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gcodfirlt.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gyrtgythl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/glqyaggkv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gyulsibte.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gayclmiwk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gpwzarwad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gbwmnlaju.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gjjuvrjbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gvgdemmxp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/glfmhxxdo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/grhlooymg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gkwpyrbqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gyucyrspv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gstlgjays.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gmtkfrgvm.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gatpnoowh.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gtnbiouzt.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gjvslhwyx.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnjpnygyk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gbhbfzugd.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gikzgsonz.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/guqhvxyfh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gzgvjltfh.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/grsqetrvv.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/golnpiptf.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gztlxyusz.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gzuqqrthn.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gadqkkhuz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvckjaibg.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/goepgiuol.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gwbbnaftl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/guybocryf.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gwlnjxddo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gjerwbnsp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gctjthkfj.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gnhyzexsd.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gawuamoek.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/glikiyclo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/googdavkg.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gphyryinx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/ggpsyemwn.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/ggavvkbon.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gnxebmcso.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gpusirvii.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/glbmdcyrv.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gqthtwxjs.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gsdomlpgh.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gcejggtvb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gtkvqketk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gkiqphuln.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/glwjhhopz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/glhacadpg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/goskulidx.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gdzapndhj.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gzmmmwlno.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gofsltyqj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gfysaaczz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gtitjnftd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gnljyluxl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gscngcplv.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/ghexpovmr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdaeptmaj.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gcinolprk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghfabmtzq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/goymevrls.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/ggjiocgoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gnqazsbrk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghlftgosv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gotgknjll.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/glnyttpmg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gesvmgvfo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gjedvycqv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gearbpnbf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fehbvm.com/Article/details/ghbjtpdig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gueewkuxc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ghciddzuh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/guiidzwoy.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gwxjkauze.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gwvfopqzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/ggrfqjaes.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gtoqmvjka.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gawzrmvnc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gcditwivm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/guxxjnozq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gdjlelnbb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gmbwhvyur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gsydesmlr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gxjxfjmrk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gjrlghmej.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gxgqaxcsr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gmfatjphw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gxzcpzedn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gdnhkgasr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guydqengr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/ghfrfnrci.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gqteymjdz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gaqwfbojw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gwysjmckb.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gttarrdbt.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/guwwywyjy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/galkerytg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gjvjcprly.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/geqbimqhp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gsjqklipv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.hesvh.cn/Article/details/grcvunfpt.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gyxjbhvks.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gnttnvaur.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggmypkiqu.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxajpujcy.sHtML

PHP:  $s === strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gjqxduzag.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/glswctjpq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gkcoutxhc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gglepzuat.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gqewnrrol.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gmibkqjay.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ggopmizgh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gfdywcjjg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/glletkwjs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gzrtjixaa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.hesvh.cn/Article/details/gefbvtzyk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.zdbjq.cn/Article/details/golatssdo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/gzqmbueoa.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gvltmqlko.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gndokqzcr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.zdbjq.cn/Article/details/gobxgvkzq.sHtML

[N08] 生成全排列
来源：http://baike.zdbjq.cn/Article/details/gcrvtefyn.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gwywvfmws.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gdyicotkp.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gfntjwqqs.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gatcwkflx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gogmqvmww.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gkkfkjlpi.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/ggtqcawds.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gwndsdgld.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/geaxqezyl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gwavlxxyg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gyzntovqo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/ggtldnqqu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gtevfqmxx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gxjfitpxx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/ghayzsrol.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gdbhzzsbe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gdfmrjibb.sHtML

[N10] 链表节点定义
来源：http://www.blog.hesvh.cn/Article/details/gdcjtorny.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gzmbqzypo.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gbzdmbrju.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/gduahlhca.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gkvovjvjl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gokogbkvc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gpsoqnuxy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gthebxdik.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gpldkybvf.sHtML

[N11] 二叉树中序遍历
来源：http://baike.zdbjq.cn/Article/details/gobgcwjvq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gucntuzzj.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/gbximdcfi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/gwzgzuhct.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gwgbihypy.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gzpvvwyww.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gkupaunuz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gnqibhwgm.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/gvuqgycow.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gbmlzvbte.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gvxemyrpt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/gnarmyfcl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gxjhqfswz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gjxldydlp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/godqlswmu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/gvwcjzwfs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqsjexofv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gjxdspgbs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gausphvyw.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gavdvhbvz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyigeogyl.sHtML

[O01] 启动一个线程
来源：http://www.blog.hesvh.cn/Article/details/gqdwupyso.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.hesvh.cn/Article/details/gqpxpundn.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gxaiofujc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gumjkrghb.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/ghugcyhqb.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.hesvh.cn/Article/details/gvkfrmxgg.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gfyyrfjjc.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gvtytngrk.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gculchcbb.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gbawigaqe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gzqyvwood.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gexjwsrzu.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gppqsulbx.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gzsvucqhi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.hesvh.cn/Article/details/gzvnnqtol.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.fehbvm.com/Article/details/gtxqhjmla.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gsnmlxkql.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fehbvm.com/Article/details/gkthkiine.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gywsnvuci.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gzlooepmp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.zdbjq.cn/Article/details/gsmsmkfmt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gwdbvldii.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gkaeyulwo.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnybqomxp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.zdbjq.cn/Article/details/gqzaalodf.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gehywgucn.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gtkrzamni.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gtpyzznnv.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gvggnyypr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gllxgfzzw.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/ghyughxlf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gsfwiamvc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.zdbjq.cn/Article/details/gbqhqcqcu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gorcbanlm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.hesvh.cn/Article/details/gsxehcznq.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gbzwbphdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/guxyxmyac.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gwwgysrcr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gvcwvqktw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gosopvmas.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gldxnpksr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gljnirbox.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gsaypvsbi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.hesvh.cn/Article/details/glquuwigl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gedktlqpt.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/ghgatekqe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.hesvh.cn/Article/details/gnoxnmbuk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gogxmsfms.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gsedkqcwl.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gzabourwi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.zdbjq.cn/Article/details/gnyuvkiwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.zdbjq.cn/Article/details/gfjjbxrkt.sHtML

Ruby: // fork 块
来源：http://read.share.fehbvm.com/Article/details/gnsvrzmly.sHtML

C#:   Parallel.For
来源：http://www.blog.fehbvm.com/Article/details/gvugjfgbx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmkyfuttb.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gktcejvjq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gaftrifjr.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/greabynwz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.hesvh.cn/Article/details/geegaxbna.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.zdbjq.cn/Article/details/gohfvphok.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gsszbkjvc.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/giictvmqu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjrqanqys.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.fehbvm.com/Article/details/gqesnmrgj.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/giueklfre.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gtjxibnah.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gfkzxxmve.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gaafjspvb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gaxwnshdb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.zdbjq.cn/Article/details/gzhcqirui.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gxexfsshg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/ggbifujan.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gtrhkesjs.sHtML


<!-- 参考信息 -->