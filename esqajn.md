代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aizwys.cn/gtwyabocco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nwbrower.top/gtuzbxwdue.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtxmkqjjof.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtmrfliniv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtkesckrzr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gteedrorrv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.haohaochexian.top/gtiicifbla.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gotoacloud.top/gtgtmufhij.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtxiqftwek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinyuanbaomall.cn/gtffsmibdf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtujseyouv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yangfankeji.com/gtsiygucxm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtnicgdpbi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtvjfrsrge.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtscqzzosy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtewaxaeew.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtnrsmnhiu.html

[L04] 设置超时
来源：http://hz.jlsjyb.cn/gtkfkazuxu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guowangkeji.top/gtlkzwbtzx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenlongwang.top/gtmhvlwzyr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtdbjtmmdl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gteenvrpck.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtgkqdrtld.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtkgvqfswd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtkenmgnap.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtqotavydw.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtwcnhlrwh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gttplbjjpw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shangyingyoupin.top/gtbmzxhlom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtmktlmsmr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtodmujiyk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gteaqngmqj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ppjwa.cn/gtyfrgfpeq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ywan-chungtsiang.top/gtjebfwxnr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yongpay.top/gtwzvosnlb.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtrfjvjttn.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtndpeqwpf.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtozkkefuz.html

JS:   await resp.json()
来源：http://hz.ppjwa.cn/gtpbrkjgli.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gterdyeizn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigufen.top/gtytzmxyqx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtscsgvxsl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtuqejybkc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.feifeiyinyue.top/gtywoehrkc.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtftgjqimw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtgvwayrtj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtlckeoarc.html

JS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtjrrezmtc.html

TS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtaqpwvewe.html

Java: resp.statusCode()
来源：http://hz.zhengqikj.top/gtobpcysoi.html

Go:   resp.StatusCode
来源：http://hz.cdnleiting.top/gtsyvmtmsl.html

Ruby: resp.code.to_i
来源：http://hz.guannengcc.top/gtbssrdjzr.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtlbkvkcrs.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtoffubcfe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jlsjyb.cn/gtqosnotku.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtcildxixj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtuhejzwcv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtnlxqfuta.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtjxvxzwop.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gttfvceaju.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtuuccqxxo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtdfbxtbxo.html

================================================================================
来源：http://hz.havefunace.top/gtqqrnhdit.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gtmbuyzlfg.html

================================================================================
来源：http://hz.yangfankeji.com/gtqbfapajf.html

[M01] 读取命令行参数
来源：http://hz.tian-w.cn/gtdmlxxpbp.html

Py:   sys.argv[1:]
来源：http://hz.ppjwa.cn/gtcoqbzwjr.html

PHP:  $argv;  $argc;
来源：http://hz.sxryk.cn/gtqblwykul.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtgcrcovua.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtyiksmlos.html

Java: args 数组（main 方法参数）
来源：http://hz.daria6918.cn/gtochrueqw.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtfpohcyhg.html

Ruby: ARGV
来源：http://hz.hfpthk.cn/gtcfsldsto.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtpunwlaon.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtfuatiztd.html

Py:   os.environ.get("HOME")
来源：http://hz.nanxuanxn.top/gtpoqnqgbs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydzc1.top/gtjapqfxud.html

JS:   process.env.HOME
来源：http://hz.zhoulong.xyz/gtozidwdgr.html

TS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtztvqxpvd.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gthryfmuhn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gttsliteon.html

Ruby: ENV["HOME"]
来源：http://hz.havefunace.top/gtfarwrxle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ywan-chungtsiang.top/gtdpsohjcu.html

[M03] 执行外部命令
来源：http://hz.hfpthk.cn/gtkbwgjxri.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gtagvrfomw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtztsgmkan.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtieixygdw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtgucpkryu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ppjwa.cn/gtckboknlh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.316326.xyz/gtkytbmjmu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gaohongyu789.top/gtywfatieo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtpbgnuwfj.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtpwswjyyd.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtbcgxiwcc.html

PHP:  getcwd();
来源：http://hz.yuanzhike.top/gtzkfeclsy.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gttsdeeahf.html

TS:   process.cwd()
来源：http://hz.0kj1m.cn/gtliazpuvy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jlsjyb.cn/gtvwqvpqcl.html

Go:   os.Getwd()
来源：http://hz.yvedp.cn/gtrezgirxv.html

Ruby: Dir.pwd
来源：http://hz.iojbl.cn/gtcuatmqlk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.9152youxi.cn/gtltyyrdls.html

[M05] 设置退出码
来源：http://hz.jqgfzy.top/gtnlufefps.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtenibgbmy.html

PHP:  exit(1);
来源：http://hz.smart0.xyz/gtkadoeewy.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtiizjuhzf.html

TS:   process.exit(1)
来源：http://hz.ivvv.top/gtfzagdpzf.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gtadqggkfi.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtnmisboul.html

Ruby: exit 1
来源：http://hz.xylfe.cn/gtmuwrdztw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sysykeji.top/gtfqdpngjh.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtmhtinrvm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fzhhl.top/gtqtvajazq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.0kj1m.cn/gtrjvsazoj.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtszveiujp.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtmzkpdeez.html

Java: System.err.println("err")
来源：http://hz.jyoumei.cn/gttmjkbqqw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.nwbrower.top/gtlknqxety.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtbeotecvo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gzhubu.top/gtwavyqmnb.html

[M07] 判断是否为主入口
来源：http://hz.gogol.net.cn/gtyqlpqzwh.html

Py:   if __name__ == "__main__":
来源：http://hz.xuanzx.com/gtegsmokoj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtsdvaueks.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtijqwauok.html

TS:   require.main === module
来源：http://hz.yueranfly.top/gtuvkeftfk.html

Java: public static void main(String[] args)
来源：http://hz.gaohongyu789.top/gtvbaxrkik.html

Go:   func main()
来源：http://hz.yj202588.top/gtjaqmpcdj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gtgulpmvrv.html

C#:   static void Main(string[] args)
来源：http://hz.yongpay.top/gtmjsjkcjv.html

[M08] 获取系统与运行时信息
来源：http://hz.iojbl.cn/gtxiqegrye.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtlfjaidrl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtsbvzqfct.html

JS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gthuqfzdur.html

TS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gtyfkubton.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.dianchejie.cn/gtkaygyfzx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtaaaiaoap.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yuanzhike.top/gtnplgzqhd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guowangkeji.top/gtwvbghllk.html

================================================================================
来源：http://hz.cqqwz.cn/gtnxchdxgm.html

N. 数据结构与算法
来源：http://hz.gaohongyu789.top/gtktwkgxdw.html

================================================================================
来源：http://hz.chenlongwang.top/gtsfjzolar.html

[N01] 二分查找（有序数组）
来源：http://hz.xziqi.cn/gtwdobckxw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtijvdpavn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sysykeji.top/gtojwhnxxl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtmbzbdffu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtntkonyry.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.chenlongwang.top/gtfoepdnvm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtmppzdoxx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yuanzhike.top/gtwjsnnqhx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.tian-w.cn/gtcwzxenth.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cqqwz.cn/gtdtovsxfj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtmmznleue.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cqqwz.cn/gtaqfxgggr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtycldbumr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.meibo888.top/gtndjpraiw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.tian-w.cn/gtvauasfkn.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtkqqzeveq.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtzvsowbuh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shanyushiyangkeji.top/gtrrxatfxk.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtiaidbdxk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtobltzspt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtdcuffvqi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenzaomai.com/gtnbodpmbf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtapfhywhi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yuanzhike.top/gtgosalvci.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtbuxnufhl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtrjxejnah.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shzxlz.cn/gtffmspudk.html

[N04] 斐波那契数列
来源：http://hz.iojbl.cn/gtjsdccmmr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.snrcjt.cn/gtkayldpwl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hysaishi.cn/gtiwtztoss.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtdkpozcti.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtvtlnggli.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.havefunace.top/gtalzesmch.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtbpkfhvrb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtjjbzwvfs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtiygmzasb.html

[N05] 最大公约数
来源：http://hz.xinyue.icu/gtuweyskkh.html

Py:   math.gcd(a, b)
来源：http://hz.zhixingplan.top/gtwbkkihpg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtvkqlauap.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ywan-chungtsiang.top/gtmcbfrxyj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtcoauwusf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gttpwgarjq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fzhhl.top/gtekyuqzbo.html

Ruby: a.gcd(b)
来源：http://hz.ydjk.org.cn/gtdluzdstx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yueranfly.top/gttbombvlw.html

[N06] 判断回文字符串
来源：http://hz.guowangkeji.top/gtqtwdiqbm.html

Py:   s == s[::-1]
来源：http://hz.zhijiandao.cn/gtkkvvufom.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtvslsquyg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtxwyglbnb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtlikviiqf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.svipenyu.cn/gtyztxdqrk.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangkeji.top/gtdpubxkvh.html

Ruby: s == s.reverse
来源：http://hz.ydjk.org.cn/gtylzlurfd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenlongwang.top/gttamfdxoy.html

[N07] 两数之和（返回下标）
来源：http://hz.shanyushiyangtech.top/gtdqwflxqh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtameogngm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.andypj.xyz/gtgsulnhul.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.zhiwuduotai.top/gtgwkzkalm.html

TS:   // 手写 Map<string, number>
来源：http://hz.yj20258888.top/gtigrysztq.html

Java: // 手写 HashMap
来源：http://hz.svipenyu.cn/gtyrzytigm.html

Go:   // 手写 map[int]int
来源：http://hz.aibaodan.cn/gtnfzuproh.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtvyffehui.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yueranfly.top/gtibfjsjsk.html

[N08] 生成全排列
来源：http://hz.hnxiangtu.top/gtlolvnzet.html

Py:   itertools.permutations(arr)
来源：http://hz.smart0.xyz/gtxkqlhcwy.html

PHP:  // 手写递归交换
来源：http://hz.yanxiufei.cn/gtyyagtjqi.html

JS:   // 手写回溯递归
来源：http://hz.cucudq.cn/gtaolcuzon.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtzuemoojt.html

Java: // 手写回溯递归
来源：http://hz.cucudq.cn/gtlitbfuki.html

Go:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtsfoddkda.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtolhoxfxb.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtpebapwsm.html

[N09] 栈与队列
来源：http://hz.52xcode.cn/gtunpignsi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.ydzc1.top/gtlgleeext.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xziqi.cn/gtbszzrmor.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtivqcshrm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydzc1.top/gtytymysii.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ehwqpu.com/gtjjjkkgkk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgfzy.top/gtmcznkaiv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtvwagbkpr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.bjfxy.top/gtbabcsshy.html

[N10] 链表节点定义
来源：http://hz.zhengqikj.top/gtmwxvrdpq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtdlyshqyc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.smart0.xyz/gtocfpulbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtjelpqzio.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guannengcc.top/gtxrkxjawd.html

Java: class Node { int v; Node next; }
来源：http://hz.mhx1999.top/gtzuyhilau.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.shzxlz.cn/gtaxngiqvg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gtuoiujglk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yonumen.top/gtbijzwgwf.html

[N11] 二叉树中序遍历
来源：http://hz.nanxuanxn.top/gtosbtvgbl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fengsongda.top/gtulqcavgy.html

PHP:  // 手写递归函数
来源：http://hz.wangdashe.top/gtdvtaaoha.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtkhyowrbu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.ybcxt.top/gtuwvtgfij.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gteouqkzpq.html

Go:   // 手写递归
来源：http://hz.bjfxy.top/gtrywqmgex.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.9152youxi.cn/gtlvgmmulr.html

C#:   // 手写递归
来源：http://hz.zhoulong.xyz/gtrafbkbbc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtfolncsnp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.yuanzhike.top/gtedlaegpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.gzhubu.top/gtcujnypph.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtaexlrmtk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj202588.top/gtlfvbvkrn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtlbumvglj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gogol.net.cn/gtzhkqobyv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinghuilouyu.cn/gtdmvpjnjt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.svipenyu.cn/gtsqnkfuhj.html

================================================================================
来源：http://hz.fzhhl.top/gtheitavnu.html

O. 并发与异步
来源：http://hz.tianlin.xyz/gtbzqusfhm.html

================================================================================
来源：http://hz.fzhhl.top/gtckzdvevz.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtyxwxoqnr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gtvjbhubqa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hongshengwenyu.top/gtiiqymdvd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gtazmbwabf.html

TS:   // 同 JS
来源：http://hz.tanke756.top/gtggnmbvah.html

Java: new Thread(() -> f()).start()
来源：http://hz.ybcxt.top/gtdbwjbgfl.html

Go:   go f()
来源：http://hz.jinghuilouyu.cn/gtttpbejlm.html

Ruby: Thread.new { f }
来源：http://hz.tanke756.top/gtgxhppkra.html

C#:   Task.Run(() => F());
来源：http://hz.nanxinkj.top/gtvfbtaphd.html

[O02] 使用线程池
来源：http://hz.quarkkingdee.top/gtnehwedaq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.hongshengwenyu.top/gtkiknrxol.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.snrcjt.cn/gtgtrljhgx.html

JS:   // worker_threads 线程池
来源：http://hz.ywan-chungtsiang.top/gtgrwmiyvu.html

TS:   // worker_threads 线程池
来源：http://hz.wangshuangyany.cn/gtiomolzpt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.kuanghao11.cn/gtboxtwldu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yvedp.cn/gtdooudris.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtjvnfolkn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yueranfly.top/gtxgxomvlh.html

[O03] 加锁保护共享数据
来源：http://hz.vqdsnc.cn/gthvgmfxdk.html

Py:   with lock: shared += 1
来源：http://hz.birdmap.top/gtqfdbzbbq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtenhseaws.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.pengpengdd.cyou/gtesqjmwzg.html

TS:   // 同 JS
来源：http://hz.andypj.xyz/gtxlwrfoia.html

Java: synchronized (this) { shared++; }
来源：http://hz.dianchejie.cn/gtqqbmtrum.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.gzhubu.top/gtuzmdfrkg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gteyqeyiib.html

C#:   lock (gate) { shared++; }
来源：http://hz.zycfv.cn/gtreybvxpx.html

[O04] 定义异步函数并等待
来源：http://hz.cqqwz.cn/gtbgtwekob.html

Py:   async def f():⏎    await g()
来源：http://hz.ybcxt.top/gtzkitxvfd.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinyuanbaomall.cn/gtdqprarxb.html

JS:   async function f() { await g(); }
来源：http://hz.pycfn.com/gtjimmodbm.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhaomingkeji.xyz/gtewfgdvso.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gotoacloud.top/gtppwsewee.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jqgufenzy.top/gtncqedlbi.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.jinqigufen.top/gtkwyunrqx.html

C#:   async Task F() { await G(); }
来源：http://hz.yuxming.cn/gttxoerjyf.html

[O05] 并发执行并等待全部完成
来源：http://hz.aizwys.cn/gtlhswiucg.html

Py:   asyncio.gather(*tasks)
来源：http://hz.zhongyouzk.top/gtvxqvpvcs.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.hfpthk.cn/gtdmuqjqoy.html

JS:   await Promise.all(tasks)
来源：http://hz.c1oappe.top/gtqqegabak.html

TS:   await Promise.all(tasks)
来源：http://hz.feifeiyinyue.top/gtxbcntahk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.jinyuanbaomall.cn/gtyvaihjqr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aibaodan.cn/gtjidpezah.html

Ruby: threads.map(&:join)
来源：http://hz.snrcjt.cn/gthifxzohw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.wangshuangyany.cn/gtkxbefmib.html

[O06] 使用进程池
来源：http://hz.fzhhl.top/gtgkqdikxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.hnxiangtu.top/gtoxbgcntm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.wangdashe.top/gtewppgdio.html

JS:   // child_process / cluster 模块
来源：http://hz.cqqwz.cn/gtgwdavkez.html


<!-- 参考信息 -->