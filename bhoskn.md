代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtukvncttx.html

JS:   await fetch(url)
来源：http://hz.yueranfly.top/gtcmfuiyhb.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtwseobjxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.havefunace.top/gtutsfsufy.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydzc1.top/gtavlopqkf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gtpafkrsok.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtocqxxiwp.html

[L02] 发送 POST JSON
来源：http://hz.0kj1m.cn/gtffdyswxf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtohefvkru.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtbwazpzou.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtdjqbdayf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gthvlszrmc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ehwqpu.com/gtatenbwyl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydzc1.top/gtpdqvupcj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtvnfzgcdd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gtgapfvbxg.html

[L03] 设置自定义请求头
来源：http://hz.jinqigfzy.top/gthtsxgvur.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtvqnaiycy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtaafrvnaq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ywan-chungtsiang.top/gtnxtjvxha.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtzpkwhtgq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xinyue.icu/gthnqxdoro.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gthyestttz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtsmabpdmk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtpprjlunw.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtopurgizl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tanke756.top/gtiowhubai.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtfziklzpt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fengsongda.top/gtiveyyhec.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtfkoewhrl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yongpay.top/gtvbmvgoxi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtkocfogun.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtqxgdksxo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtgiufjchp.html

[L05] 上传文件（multipart）
来源：http://hz.gzhubu.top/gtieddxqcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gticikrgre.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.iojbl.cn/gtatxubwdi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtyeyemcxz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtpcmqvmxz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gtxnlmaprv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtdkwjcnnx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtiekvcwso.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtfvvwclgg.html

[L06] 解析响应为 JSON
来源：http://hz.jqgufenzy.top/gtxfwtkvhu.html

Py:   resp.json()
来源：http://hz.cashguo.top/gtnrnvcafi.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtfbvxtuay.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtftmoyuzn.html

TS:   await resp.json()
来源：http://hz.sxryk.cn/gtsczlufce.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangtech.top/gtkhettwai.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yangfankeji.com/gtmnzopaap.html

Ruby: JSON.parse(resp.body)
来源：http://hz.0kj1m.cn/gtglzokcaf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shangyingyoupin.top/gtouzsnwcd.html

[L07] 处理 HTTP 状态码
来源：http://hz.chenzaomai.com/gtjxgllwhe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtjhohmepi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtarqdpqrc.html

JS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gtlvgpkvor.html

TS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtscboetig.html

Java: resp.statusCode()
来源：http://hz.hywenlv.cn/gtyqcsklps.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtmorevvmx.html

Ruby: resp.code.to_i
来源：http://hz.jiagoushi.top/gtdrlfxdgs.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtpnwfgndg.html

[L08] 并发请求多个地址
来源：http://hz.0kj1m.cn/gtwgtnxfev.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aizwys.cn/gtfvslkawk.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtxvylqwcg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.smart0.xyz/gtlgvylrhj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgfzy.top/gtivtkekcm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cucudq.cn/gtdlaefcxx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtamonegxu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtwxustvhk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuetiantiany.cn/gtufiwrtpr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtnwkendly.html

M. 命令行 / 进程 / 环境
来源：http://hz.hywenlv.cn/gtwzntpogt.html

================================================================================
来源：http://hz.shuidangran.top/gtrqoisrte.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtipdpgqsu.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtknfjjooq.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gtszizlpvh.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtrwnzpqvr.html

TS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtdqlmohpm.html

Java: args 数组（main 方法参数）
来源：http://hz.hywenlv.cn/gtblnkfekb.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtkmkolvqj.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtmbxllldg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yuxming.cn/gtapdztkiu.html

[M02] 读取环境变量
来源：http://hz.xinyue.icu/gtnxuuasqq.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtwfsytheq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtldgsscxb.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtdupooneg.html

TS:   process.env.HOME
来源：http://hz.sweek.top/gtgfwcbryj.html

Java: System.getenv("HOME")
来源：http://hz.quarkkingdee.top/gtfsokcvwo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jiagoushi.top/gtyhnzvwlk.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtfmvwwkzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtkuoxscqw.html

[M03] 执行外部命令
来源：http://hz.yj20258.top/gtredecyng.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtckeahjvj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.haohaochexian.top/gtainizgtx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtobamyztg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtvakjbsah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtuekkhqkm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenlongwang.top/gtgwyccswk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.meibo888.top/gtnbxvaiah.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gttgdldksk.html

[M04] 获取当前工作目录
来源：http://hz.jinqigfzy.top/gttytxmyjr.html

Py:   os.getcwd()
来源：http://hz.chenjidiqi.icu/gtifnengqo.html

PHP:  getcwd();
来源：http://hz.hongshengwenyu.top/gtpgcpuyyi.html

JS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtdmgnoxdo.html

TS:   process.cwd()
来源：http://hz.daxiang520.top/gtxxuzikan.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtlnrmaria.html

Go:   os.Getwd()
来源：http://hz.hammf.cn/gtximuwlfd.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtpnftqykc.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangtech.top/gtfgkizzlp.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gtsdpoyujp.html

Py:   sys.exit(1)
来源：http://hz.smart0.xyz/gtfhsmrrqe.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtkkrqkpif.html

JS:   process.exit(1)
来源：http://hz.havefunace.top/gtcpqmhgyl.html

TS:   process.exit(1)
来源：http://hz.redwolf501.top/gtrndhuhad.html

Java: System.exit(1)
来源：http://hz.ppjwa.cn/gtrjnkpynt.html

Go:   os.Exit(1)
来源：http://hz.yj20258888.top/gtuvasrcif.html

Ruby: exit 1
来源：http://hz.jinghuilouyu.cn/gtryvokveb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.meibo888.top/gtytmmlxln.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtlxzyaqkb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtxxfehfsj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtiknozsgs.html

JS:   console.error("err")
来源：http://hz.iojbl.cn/gtduqsvres.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gttmfwoexj.html

Java: System.err.println("err")
来源：http://hz.chenjidiqi.icu/gtwxjtdsjq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gtddihnuuz.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtucxlqluh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.0kj1m.cn/gtjnbykydn.html

[M07] 判断是否为主入口
来源：http://hz.quarkkingdee.top/gtiaaklxjj.html

Py:   if __name__ == "__main__":
来源：http://hz.jyoumei.cn/gtcktojfeb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtxtxluozp.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtjhqvhbmq.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gtzxkoynfx.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtpgpjffll.html

Go:   func main()
来源：http://hz.cqqwz.cn/gtwmlbyppw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ppjwa.cn/gtwvyqszeu.html

C#:   static void Main(string[] args)
来源：http://hz.316326.xyz/gtqtsgbiro.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtkhyhdulw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtsxsuvvpk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtkbcjmpki.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtrisbnkbm.html

TS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtnukainut.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhijiandao.cn/gtvqutlqcp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jlsjyb.cn/gtyhdlowoo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cashguo.top/gtqguvtkdy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtbcwlxwat.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqybfujib.html

N. 数据结构与算法
来源：http://hz.aizwys.cn/gtqsowrqju.html

================================================================================
来源：http://hz.0kj1m.cn/gtppdlvwvj.html

[N01] 二分查找（有序数组）
来源：http://hz.guannengcc.top/gtsxysikhd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yongpay.top/gtybbqzphu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ydjk.org.cn/gtxhyqmwoy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cqqwz.cn/gtbxbalhpu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtdzkdpipb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtkcjiuetf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aibaodan.cn/gtahhtazfl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtpjggezix.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtglqgmjqv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cucudq.cn/gtzjwdkdcc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtravkatwz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.bjfxy.top/gtymmfgjgh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtrbrxbuna.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtmkvndmjh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtfauuohjr.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gtnwmtsrii.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gthqnieifw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ppjwa.cn/gtbmsuimqn.html

[N03] 快速排序（分治示例）
来源：http://hz.aibaodan.cn/gtkwveulmt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gtwkeamykk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shangyingyoupin.top/gtmdbnkkkm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinyuanbaomall.cn/gthiumkqey.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtxnmxoqic.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtrvwzlwqo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dianchejie.cn/gtlhwfrbab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yuxming.cn/gtbfwbbyni.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtuhfxdlbf.html

[N04] 斐波那契数列
来源：http://hz.mhx1999.top/gtbjnbfnrk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nwbrower.top/gtdyjuclgg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gtgubpdsha.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.0kj1m.cn/gtcxuspnrk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tian-w.cn/gtzhbwswlg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yueranfly.top/gtoeexhuta.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.9152youxi.cn/gtinocipru.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinqigfzy.top/gtuhhlmara.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.mhx1999.top/gtpzzprufo.html

[N05] 最大公约数
来源：http://hz.hnqzz.top/gtnzounyax.html

Py:   math.gcd(a, b)
来源：http://hz.guowangkeji.top/gtdxfuzjwo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gteggkzzyb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.smart0.xyz/gtyfikfptr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtlkgdvngt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tian-w.cn/gtlzyxvkhm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nwbrower.top/gtitqgedrw.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtuobqquej.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.cheryme.top/gtqstzjhjd.html

[N06] 判断回文字符串
来源：http://hz.jinghuilouyu.cn/gtngyxbxqv.html

Py:   s == s[::-1]
来源：http://hz.xziqi.cn/gtfmzlogli.html

PHP:  $s === strrev($s);
来源：http://hz.shanyushiyangkeji.top/gtmewaxpva.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtpfxgysue.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fengsongda.top/gtqzaepsqu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhijiandao.cn/gtpmdhpqtl.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangkeji.top/gtwpplztar.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gtxtkdmqds.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gttstvzhdo.html

[N07] 两数之和（返回下标）
来源：http://hz.pengpengdd.cyou/gtulimjxno.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ydjk.org.cn/gtzdrhopzz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtjnnuksib.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yueranfly.top/gtabvwcgbk.html

TS:   // 手写 Map<string, number>
来源：http://hz.meibo888.top/gtcennqmbr.html

Java: // 手写 HashMap
来源：http://hz.daxiang520.top/gtluhxzxjk.html

Go:   // 手写 map[int]int
来源：http://hz.vqdsnc.cn/gtfvpnlfji.html

Ruby: // 手写 Hash
来源：http://hz.xuetiantiany.cn/gtlxdyxziw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.dianchejie.cn/gtvytyswdu.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gtxbjjpswm.html

Py:   itertools.permutations(arr)
来源：http://hz.yj202588.top/gtkoktwwzh.html

PHP:  // 手写递归交换
来源：http://hz.cheryme.top/gtoqknbtyo.html

JS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtxklholfi.html

TS:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtkvpgjlab.html

Java: // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtaujbuior.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gthxbutduc.html

Ruby: arr.permutation.to_a
来源：http://hz.sufxvd.cn/gtipnxaugq.html

C#:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtnfyikens.html

[N09] 栈与队列
来源：http://hz.nanxinkj.top/gterppzyfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.kuanghao11.cn/gtivvxgggb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jqgufenzy.top/gtlgoqxxbz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.shzxlz.cn/gtdyakafbv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.xinyue.icu/gtdjmokpqf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.jinqigufen.top/gtgaatfcqn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.yj202588.top/gtgzdqmmdj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtuogphhov.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtzaecuxct.html

[N10] 链表节点定义
来源：http://hz.gogol.net.cn/gtidwkxifx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xziqi.cn/gtatgdhifp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gthhlzkbmo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xinyue.icu/gtpwcdpkkz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gotoacloud.top/gtjbpewsqw.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtizuvrxzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.redwolf501.top/gtqlmqjktw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cheryme.top/gtsdooesop.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.birdmap.top/gtkvlqhgdn.html

[N11] 二叉树中序遍历
来源：http://hz.jinghuilouyu.cn/gtufyzxplb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtgcwyqbwx.html

PHP:  // 手写递归函数
来源：http://hz.meibo888.top/gtcmzzbete.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtbbikgxjx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinqigufen.top/gttosxoeqk.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gtkyrbrxca.html

Go:   // 手写递归
来源：http://hz.sweek.top/gtbfiijzwh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sysykeji.top/gtxbuhxqpd.html

C#:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtffpqjesj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ybcxt.top/gtzaigmrka.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.fengsongda.top/gtnavezstw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yangfankeji.com/gtwaowlcve.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.sxryk.cn/gtefgjkrpg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtgbkrgvbf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtxoxktxta.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtdxolipcx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.redwolf501.top/gtpkmwxvik.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shzxlz.cn/gtzhuxrwvg.html

================================================================================
来源：http://hz.fengsongda.top/gtewnuquyu.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gtmxspoccm.html

================================================================================
来源：http://hz.dashuyun.cn/gtcxydtnew.html

[O01] 启动一个线程
来源：http://hz.haohaochexian.top/gtqrrzdntn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.zhaomingkeji.xyz/gtccnqshgm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhijiandao.cn/gthbngevgx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fengsongda.top/gtrcfwtjpo.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtnegkcvcl.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinyuanbaomall.cn/gtdrmntcnl.html

Go:   go f()
来源：http://hz.yueranfly.top/gtlgxcqznh.html

Ruby: Thread.new { f }
来源：http://hz.smart0.xyz/gtueirbonv.html

C#:   Task.Run(() => F());
来源：http://hz.cheryme.top/gtsczuvynw.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtzugfqgku.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cqqwz.cn/gtinmyrwou.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.chenjidiqi.icu/gtzkzfcuel.html

JS:   // worker_threads 线程池
来源：http://hz.jyoumei.cn/gttyainnci.html

TS:   // worker_threads 线程池
来源：http://hz.jianghu66.top/gticojvitq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zdqjudy.top/gtmbtketas.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xinyue.icu/gthhpmfvgz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtejbjajdl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.feifeiyinyue.top/gtjyuhjans.html

[O03] 加锁保护共享数据
来源：http://hz.jinyuanbaomall.cn/gtyrbgikwg.html

Py:   with lock: shared += 1
来源：http://hz.hnxiangtu.top/gtpalkdozf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.haohaochexian.top/gtygozgcmg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aibaodan.cn/gtloyauqyj.html

TS:   // 同 JS
来源：http://hz.wangshuangyany.cn/gtxdnqbuiz.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydjk.org.cn/gtjsiotcxk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.tian-w.cn/gtacaxpnhm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenzaomai.com/gtuseronuf.html

C#:   lock (gate) { shared++; }
来源：http://hz.yueranfly.top/gtfqovorvr.html

[O04] 定义异步函数并等待
来源：http://hz.aibaodan.cn/gtgxgkliru.html

Py:   async def f():⏎    await g()
来源：http://hz.quarkkingdee.top/gttucxxilr.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.sysykeji.top/gtgfvhaqni.html

JS:   async function f() { await g(); }
来源：http://hz.ywan-chungtsiang.top/gtpyxwvngc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cheryme.top/gthhvbjrca.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.ybcxt.top/gtmbejnnhr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.shanyushiyangtech.top/gtljtutlfw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.daria6918.cn/gttawfktwu.html

C#:   async Task F() { await G(); }
来源：http://hz.tianlin.xyz/gtagvbkfyq.html

[O05] 并发执行并等待全部完成
来源：http://hz.fzhhl.top/gttxlvebry.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhoulong.xyz/gtfjohhntd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.andypj.xyz/gtkbmvvrjx.html

JS:   await Promise.all(tasks)
来源：http://hz.fzhhl.top/gtsjexfwpd.html

TS:   await Promise.all(tasks)
来源：http://hz.ybcxt.top/gtfywujyqr.html


<!-- 参考信息 -->