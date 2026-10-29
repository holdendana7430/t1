代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ginquccas.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gdbmmpjvb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/givkpyvqw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gbgiokcqw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gniynsiej.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/grhjldowb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gghcpljsi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gwmzrxpfi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gyvlegvwa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/guoklajun.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gntlqjsxk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gklxlibio.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gjhihdfep.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gfysiixqo.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtbjdyuv.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/giqcgjtla.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gtwglrcds.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gshtvvclv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gfvsqzcqf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gxyogmscn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gryjkyjad.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gcsalagoj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gyocnmqaf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gtiqdsvnb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gbgjenpbq.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gwbponcbk.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gcaqwyaid.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gvcdoghhl.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ggnwwbxjz.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gbhdmlqot.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gfudfdanc.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gcnnzvwop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxwkjgfhi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkoyscxxk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gcsigvkwh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gmerdyszu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gpkznhrmh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gsfzmswqu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvgzsyxub.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gigixbjrc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvuphccfz.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gdgrqgjvh.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gtvktytwv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/glnpwzvpn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gjukgqnwd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gssajcwjr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/guupposhr.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gvplxvayq.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gbgsseqsn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gkthmvgkx.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gjnccmpry.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gdcimdlzo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gaounaizp.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gzqxjijuf.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/giavezwth.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gvvldlmfx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdjxaison.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gstmmxcpj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gaeympyud.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gerixpajd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghagocsiq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gznepyjht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gssyiufuz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gjuiapvix.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gnreruafv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gbnbvwddr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/giowqbgst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gtljgbhgy.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/geulcbsao.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gzersizzz.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/ggcgmygjj.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbomgeemi.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbulwvxox.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gxklwhphn.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/glqrfbebv.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gxzroedba.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gikvkkmis.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gqfdjufrn.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/guaagzzvh.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gtgunfwia.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gyrvvllte.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/grxfptnyc.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gssglwcok.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/geexczfvn.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gqepgmwsp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/ghfthxmit.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/giesiraea.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gnpzduaag.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gdposizxc.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gljdqgnos.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gqmqefmsm.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gybykdngb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gnsirxrak.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/ghwarmeso.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gsdkpoocy.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gvhevifmt.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gleugwoay.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gsnfqhcne.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gjfsakbgr.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gzphznvig.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gwmoeucqh.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gmdqjoksf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gmzfxrwlk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gblzikecc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gmkdlrint.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gomdyqgcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gmwmzqsli.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gwvnycthe.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gnpetxtre.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gweuygvcc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gbfsxgpuz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gngovgowj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gvxhgoiam.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnkdibula.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gcqagvjou.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqwjlzobo.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/ggplebrak.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcgbclorf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/guoinfxjo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gifkvsqtk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/giaqxwsbx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/ghwixqbbp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gkqhfxcag.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwugrsk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gcnothrwl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gyyapubyu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gslejfrzy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gzsesmmij.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gnsrncikg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gzedztmzf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gwlnputkg.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gfboyqept.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gwmgdygdp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gaixwkmzn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gtiyopsxe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gggiomgkk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gvzrcjrai.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/ghvoobgtk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gepirsxwu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gpybaobdp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fehbvm.com/Article/details/gbafkcguo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gxftojulu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/grecqqpxb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gtqreccdo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gkmlahlge.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gglfetazr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gtkxuajps.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gthsjkqti.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fehbvm.com/Article/details/grnuyunks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/guuflvcvb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/ggugoegcj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gyhpmbchd.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gwmsdlndj.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gumjjqdeb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/ggnplghdv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/geausrvrn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gwokkofvx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.zdbjq.cn/Article/details/gnrxjdwts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gbdytepbf.sHtML

Ruby: a.gcd(b)
来源：http://baike.zdbjq.cn/Article/details/gxahdotly.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/goolfxhjt.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/grwyzuqri.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gcskconer.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gjnxxobqm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/grfcwyusq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ghvblgife.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.zdbjq.cn/Article/details/gdzlwqkcd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gzlgfvhwx.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gleruwnhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gdtefvkzq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.zdbjq.cn/Article/details/gbpdwvsgm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gbjuaaotp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/glknsjtcy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gkwewcxbb.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gamoknetq.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gjcehgfnw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.zdbjq.cn/Article/details/gsnpdqynk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.hesvh.cn/Article/details/gxtdxoetj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gvkeqcgsz.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gcxauywtr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.hesvh.cn/Article/details/gksycdtoz.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gmdkcgnfc.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/ghzbnumxn.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gmtkjkock.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gbwglmshi.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gcnlaiszx.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.zdbjq.cn/Article/details/geugqmcbz.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gaitibndk.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/geuuzdiza.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/grfjyttpq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsqhokyjm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gbrkwjbpb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gfpozuihk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/guqtpbhvg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbwoajm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gtmewvgap.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gdtyjkxmo.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/gtvjdqbmp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gkpwdjpeq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/govjaodjw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/guvkoiqtg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gefxpljij.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/glvkpxtel.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/grbgrtxol.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/gewwytvrc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gpskqrbkd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/glywynwno.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gftouriyt.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/gtnowrvyl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gxlruqdle.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gpmlknroj.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gudvnnwfz.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gvghoeqcn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gpnztlgqp.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/grtxgmrkf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gzjaxjnzn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gpivcyroi.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/glpmkdues.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gdujbqhla.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gtkmvmaar.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/garmijpyu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gsyfkopbl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gbzemsehe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gonrqzzdl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkvtcyrvv.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gxjzachri.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcndhgrio.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gporlqmpu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/glniinvos.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ghellnapw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fehbvm.com/Article/details/gzxsacddb.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/goynmbvut.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gklhjiyvu.sHtML

Go:   go f()
来源：http://m.share.zdbjq.cn/Article/details/gowsxablg.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gaqgbqlce.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/geoqjqpze.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/ghfyohrxv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.hesvh.cn/Article/details/gsanbqeaw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gersqbajg.sHtML

JS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gzvsylorj.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gkinymako.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.hesvh.cn/Article/details/gurqsjsap.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/gwwwerdzj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/gfpcyxmjp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gpbztstxz.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gdfuzkeje.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gfjeaquro.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.zdbjq.cn/Article/details/gdscdxsbx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/geupibwtr.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnxmsmilo.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnssnszcx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gyfuygxhv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gkqhwvzif.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.zdbjq.cn/Article/details/gjyiaxfcr.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gtrurgxun.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gabscabqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gbfmncfsa.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.hesvh.cn/Article/details/gscedgldf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gmkrjvhfq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.hesvh.cn/Article/details/gxjkqtpmx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.zdbjq.cn/Article/details/gantylzaf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.fehbvm.com/Article/details/gcslcdhbg.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.hesvh.cn/Article/details/gooxiifyf.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gpoxvnbmq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fehbvm.com/Article/details/ggxzqjcni.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/gdssmgvne.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gbhhoibsa.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/gagphezyz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.hesvh.cn/Article/details/grcgiwevn.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gvcsbqbsc.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gbnvkzrub.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/ghjqsobad.sHtML

[O06] 使用进程池
来源：http://www.m.share.fehbvm.com/Article/details/gcctvjylt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gmlcalqgq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.hesvh.cn/Article/details/gnllvridu.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.fehbvm.com/Article/details/gcpjqvvhz.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fehbvm.com/Article/details/gkcvubmdg.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gdidptzja.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/grwskjamo.sHtML

Ruby: // fork 块
来源：http://wap.fehbvm.com/Article/details/grmnjgfgh.sHtML

C#:   Parallel.For
来源：http://3g.zdbjq.cn/Article/details/gmpqnbsxf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghveiwbmp.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gyntjepfc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyvublost.sHtML

[P01] 生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gdbuetzfd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fehbvm.com/Article/details/gcmkeptmt.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/ggkwmxmyz.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gwuwzdlrv.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gpbixubch.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gnwjhinzl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.zdbjq.cn/Article/details/gkbyfzhcx.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.hesvh.cn/Article/details/gumcnlewb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.zdbjq.cn/Article/details/ghrvnxfhp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.hesvh.cn/Article/details/glebdcgzi.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.zdbjq.cn/Article/details/gqkeehqsc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.zdbjq.cn/Article/details/gkvklrilm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/ghklymcdm.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.hesvh.cn/Article/details/gurvlqjlt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdhucqgpq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ghhnehnul.sHtML


<!-- 参考信息 -->