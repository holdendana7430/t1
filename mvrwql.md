代发 wailian999

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtfsljgioq.html

Ruby: Marshal.dump(obj)
来源：http://hz.feifeiyinyue.top/gtsmtylcre.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ybcxt.top/gtjnfrpotz.html

================================================================================
来源：http://hz.jqgufenzy.top/gtfbevvkpp.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtjhzogzna.html

================================================================================
来源：http://hz.316326.xyz/gtolqehcmg.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtvzuibdxp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtslvvfhmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhixingplan.top/gtggetrlpv.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtrgvfzfzb.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gttlbngxem.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtooraiqbo.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtwolfvwya.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtaltcafrr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtkdanfijj.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtbapjzcpc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.andypj.xyz/gtajicpeib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenzaomai.com/gtetdxbptg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtlswczuhr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtuqivzubg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtlsundwus.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gogol.net.cn/gteaoxacrn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtdeggtiok.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.316326.xyz/gtggvviojj.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtwaiuaufp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtlbvybixg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtvyrwtvhv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cdnleiting.top/gtcmwzgydu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtcwzvddkm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtwwjmnsnk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sufxvd.cn/gtjsifzufk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xylfe.cn/gtghyxvlei.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtddlgodxm.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtdoumqpro.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtjkbvrkgt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cdnleiting.top/gtzaiqzxyh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtzcuhjgeg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtjvjpawrd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gttosxuplx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangkeji.top/gtsugrlzse.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtiyvnxynt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jyoumei.cn/gtudegysjb.html

[L05] 上传文件（multipart）
来源：http://hz.sufxvd.cn/gtjazpfjhj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gogol.net.cn/gtgesyxjvt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtaktfszpy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtmeebrjpw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gtjuxfwpnm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gttiylcdhz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtacqycirv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fengsongda.top/gtnzolrctq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtmaplnpid.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gtihveoymj.html

Py:   resp.json()
来源：http://hz.jqgufenzy.top/gtukcseifb.html

PHP:  json_decode($body, true);
来源：http://hz.xuetiantiany.cn/gtnsirdjjf.html

JS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtsxpasuxr.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtctsbwwfn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ydzc1.top/gtsltsnfzq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtbsgvvgfi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtpnfypgpw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hysaishi.cn/gtbwgndfwt.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtacopwfes.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtvcyjzcpe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yuanzhike.top/gtfhuwsavn.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtrkkagtvz.html

TS:   resp.ok;  resp.status
来源：http://hz.cashguo.top/gtkzwpuilj.html

Java: resp.statusCode()
来源：http://hz.yanxiufei.cn/gtryfpppqg.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gtyluzxfbh.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtqsfsetcs.html

C#:   (int)resp.StatusCode
来源：http://hz.quarkkingdee.top/gtjurwpkvb.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gteaepyzdm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj202588.top/gtswkfhokd.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtppmfexqf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtbkvkimej.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtfyiyakxw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gtlvkecaty.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gtbnxhuhkf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tanke756.top/gthcurqlbl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtapcojrdy.html

================================================================================
来源：http://hz.jianghu66.top/gtybqeqflk.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtxjgpohui.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwhrcwvsn.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtyxypeadh.html

Py:   sys.argv[1:]
来源：http://hz.bjfxy.top/gtijacvahv.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gteqrzwzrj.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtyxanckha.html

TS:   process.argv.slice(2)
来源：http://hz.wangdashe.top/gtcezauugm.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtyrxmdsvm.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtquigpdom.html

Ruby: ARGV
来源：http://hz.wangshuangyany.cn/gtcrsrksbc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtdniwqfoe.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtarakxzrf.html

Py:   os.environ.get("HOME")
来源：http://hz.gogol.net.cn/gtstwuqzsv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gtctwvxqos.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtlvbbtimd.html

TS:   process.env.HOME
来源：http://hz.jianghu66.top/gtonhbnhac.html

Java: System.getenv("HOME")
来源：http://hz.jinqigfzy.top/gtairhsaqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtlkvwzxvv.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtoftzgyvb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydzc1.top/gtrucbhamy.html

[M03] 执行外部命令
来源：http://hz.wangdashe.top/gtqcupyofq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hnqzz.top/gtbnhojwnt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.wangdashe.top/gtrpmcjwbb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gthygjoffa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.iojbl.cn/gtlqvzytdv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtxevhjkgk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtiwvegzyv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtwwuvvayf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ybcxt.top/gtpjhvszjs.html

[M04] 获取当前工作目录
来源：http://hz.fengsongda.top/gtexxtkmwm.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtrxbjfxza.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtwigoanpi.html

JS:   process.cwd()
来源：http://hz.kuanghao11.cn/gthlvzcnae.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtzsmlcchx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gtjxtbjabj.html

Go:   os.Getwd()
来源：http://hz.gogol.net.cn/gthssicycl.html

Ruby: Dir.pwd
来源：http://hz.sxryk.cn/gtuysijvew.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cashguo.top/gtudnzgrls.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtjvmtdjbb.html

Py:   sys.exit(1)
来源：http://hz.yvedp.cn/gtmjlvbyza.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtuebdzamk.html

JS:   process.exit(1)
来源：http://hz.fzhhl.top/gtlpldarwx.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtdniranug.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtyqhotkby.html

Go:   os.Exit(1)
来源：http://hz.wangdashe.top/gtoimwomxl.html

Ruby: exit 1
来源：http://hz.316326.xyz/gtrpwkdsni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtscigtznb.html

[M06] 向标准错误输出
来源：http://hz.bjfxy.top/gtdybszqei.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtzlpmpxxc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtcjaxggim.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtqhqmrxal.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtzpcakiva.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtxintgskt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yonumen.top/gtkwdcynoj.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtkxoiwilw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jianghu66.top/gtdmqanabo.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtzjgtelbs.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtxqmeiywc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtbmsqnkbk.html

JS:   require.main === module
来源：http://hz.hnqzz.top/gthzwozlab.html

TS:   require.main === module
来源：http://hz.sweek.top/gtvrjhcxrn.html

Java: public static void main(String[] args)
来源：http://hz.gogol.net.cn/gtccvvyukv.html

Go:   func main()
来源：http://hz.xingfuxueyuan.xyz/gtgvbptqow.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtllnfqzpv.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtchzonpuj.html

[M08] 获取系统与运行时信息
来源：http://hz.vqdsnc.cn/gtfgxeydgo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xingfuxueyuan.xyz/gtbaavliox.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gthpiowzbo.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gthtogrvmz.html

TS:   process.platform;  process.version
来源：http://hz.feifeiyinyue.top/gtuqmvmhhp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xinyue.icu/gtlsgtnnar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtcxysbfzo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gtrmrgmmyw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gtzhiniffy.html

================================================================================
来源：http://hz.cashguo.top/gtmjdzidri.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gttxsumofs.html

================================================================================
来源：http://hz.aizwys.cn/gtuscdvile.html

[N01] 二分查找（有序数组）
来源：http://hz.wangshuangyany.cn/gtgnmywwpl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtimlozybm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fengsongda.top/gtawpxevub.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtrsmeernb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtoehyasuh.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hfpthk.cn/gthqwubcxd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtgardvdhy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yongpay.top/gtyamcmvzk.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jqgufenzy.top/gtduvhurwi.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.redwolf501.top/gtfxosagnv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtxhlzwlbk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gtnngyhazn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ydjk.org.cn/gtcmluyinu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gzhubu.top/gtrhtfwtpo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gttilsgsxf.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtibntcufa.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtjzolrxgn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuetiantiany.cn/gtmqfqhwqy.html

[N03] 快速排序（分治示例）
来源：http://hz.c1oappe.top/gtmvxzjrwc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenzaomai.com/gtbrtxfdmj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenlongwang.top/gtfmzcgxiu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtdlizhnom.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtqcmhjiip.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daria6918.cn/gtlgfagkit.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnqzz.top/gtuturklbn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenlongwang.top/gtmjjgcdxs.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.feifeiyinyue.top/gthknjrmte.html

[N04] 斐波那契数列
来源：http://hz.zhoulong.xyz/gtojyudzbu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sweek.top/gtrntxhxas.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtknvthqbd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zycfv.cn/gtlaxwmghs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtiprajvky.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.iojbl.cn/gtpehwkymg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hammf.cn/gtmbjdsyxc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtitfdgtgp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuanzx.com/gtdewppchc.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gtolmciwqp.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gttqdjdriy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtxqbutpvk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtqdojrtxd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtteqaocbu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pengpengdd.cyou/gtvfmmvvia.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinyuanbaomall.cn/gtantgvmli.html

Ruby: a.gcd(b)
来源：http://hz.pengpengdd.cyou/gtwsvaeibt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtaayghtgu.html

[N06] 判断回文字符串
来源：http://hz.tanke756.top/gtbgmpyvsr.html

Py:   s == s[::-1]
来源：http://hz.chenzaomai.com/gtnlicrkbb.html

PHP:  $s === strrev($s);
来源：http://hz.jianghu66.top/gtjeatkvob.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtalcgnyip.html

TS:   s === [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtpfgyklml.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtgufuybqt.html

Go:   // 双指针从两端比较
来源：http://hz.jyoumei.cn/gtnmkpxzwm.html

Ruby: s == s.reverse
来源：http://hz.vqdsnc.cn/gtlshyupzn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtephaiwyb.html

[N07] 两数之和（返回下标）
来源：http://hz.ppjwa.cn/gtwxzeoaeu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.gotoacloud.top/gtsnnyoyja.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shuidangran.top/gtvbydqkxy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.birdmap.top/gtijnrrbid.html

TS:   // 手写 Map<string, number>
来源：http://hz.bjfxy.top/gttlyvmcqn.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtefwkcoco.html

Go:   // 手写 map[int]int
来源：http://hz.jlsjyb.cn/gttambriwf.html

Ruby: // 手写 Hash
来源：http://hz.xingfuxueyuan.xyz/gtttqdnubj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jinghuilouyu.cn/gtccmzcgfp.html

[N08] 生成全排列
来源：http://hz.shanyushiyangkeji.top/gtybogqwie.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtaztnptuh.html

PHP:  // 手写递归交换
来源：http://hz.sysykeji.top/gtbhjilqoo.html

JS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtkfbcsyle.html

TS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtrqymuepi.html

Java: // 手写回溯递归
来源：http://hz.zycfv.cn/gtvxtjkjwr.html

Go:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtnmitrruf.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gtguqusjgd.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtptyfudjl.html

[N09] 栈与队列
来源：http://hz.zhixingplan.top/gtdgmpqvjh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xingfuxueyuan.xyz/gtxmxqtmrf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yonumen.top/gtdaxzxxzw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gttixywnaq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.shuidangran.top/gtsolggatl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ydjk.org.cn/gttgyocqgw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shzxlz.cn/gtjdrcpqty.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtfcqgwnpw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hywenlv.cn/gtvxylvted.html

[N10] 链表节点定义
来源：http://hz.pycfn.com/gtbxklfand.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.52xcode.cn/gtoyemraze.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yuanzhike.top/gtaibgrmsb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtjzfjvgcx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.vqdsnc.cn/gtmqcoxlwe.html

Java: class Node { int v; Node next; }
来源：http://hz.jlsjyb.cn/gtudrtzblk.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.hongshengwenyu.top/gtsupnfgdo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangdashe.top/gtohbvcbmc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.wangdashe.top/gtocibzzst.html

[N11] 二叉树中序遍历
来源：http://hz.zhaomingkeji.xyz/gtprfqbaqk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shuidangran.top/gtcapeccse.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtliwwdzwq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhaomingkeji.xyz/gtljqlzrla.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nanxuanxn.top/gtaystomay.html

Java: // 手写递归
来源：http://hz.kuanghao11.cn/gtcbopvrkb.html

Go:   // 手写递归
来源：http://hz.jinyuanbaomall.cn/gteyimcfyn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shanyushiyangtech.top/gthweiaavc.html

C#:   // 手写递归
来源：http://hz.jinghuilouyu.cn/gtlmdnqlnc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtbeauvxfs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.pycfn.com/gtklitnbak.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.guowangkeji.top/gtlhmqsobn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuanzx.com/gtebounged.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.xuetiantiany.cn/gtytavzfhr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtbdnrdkrk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gaohongyu789.top/gthtjwctcu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.andypj.xyz/gtgugrpegr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtkmbpfrrf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgblchalq.html

O. 并发与异步
来源：http://hz.chenlongwang.top/gttairrzhq.html

================================================================================
来源：http://hz.gotoacloud.top/gtmqitxsqo.html

[O01] 启动一个线程
来源：http://hz.yueranfly.top/gtmmffioxa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.chenzaomai.com/gtlurcchhe.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtezkyxfdu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hfpthk.cn/gtyhqohahp.html

TS:   // 同 JS
来源：http://hz.zdqjudy.top/gtuqjqbbws.html

Java: new Thread(() -> f()).start()
来源：http://hz.guowangkeji.top/gtmshtvemq.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtsquhtgdc.html

Ruby: Thread.new { f }
来源：http://hz.ydjk.org.cn/gtsnhtnsmy.html

C#:   Task.Run(() => F());
来源：http://hz.guowangkeji.top/gtcjetclzw.html

[O02] 使用线程池
来源：http://hz.zycfv.cn/gtbzfgbfog.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.xuanzx.com/gtklmgweyy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pengpengdd.cyou/gtlxxangqa.html

JS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtsywpkikt.html

TS:   // worker_threads 线程池
来源：http://hz.jiagoushi.top/gtcytrpaia.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dianchejie.cn/gtknvgnfum.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.shanyushiyangtech.top/gtcphzamie.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zycfv.cn/gtpwrrxufd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258888.top/gtcdmxihfk.html

[O03] 加锁保护共享数据
来源：http://hz.zhongyouzk.top/gtcmupmgsv.html

Py:   with lock: shared += 1
来源：http://hz.kuanghao11.cn/gtqznpklgb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.guowangkeji.top/gtpisyjlex.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.haohaochexian.top/gtggiroksf.html

TS:   // 同 JS
来源：http://hz.chenzaomai.com/gtxefjaxst.html

Java: synchronized (this) { shared++; }
来源：http://hz.fzhhl.top/gtjtbdivwy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.feifeiyinyue.top/gtdrleyyql.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.mhx1999.top/gtlozotriu.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhaomingkeji.xyz/gtxtobhphs.html

[O04] 定义异步函数并等待
来源：http://hz.yanxiufei.cn/gtleyykhiv.html

Py:   async def f():⏎    await g()
来源：http://hz.vqdsnc.cn/gtkpsvnyup.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yj20258888.top/gtfdiqowyz.html

JS:   async function f() { await g(); }
来源：http://hz.yongpay.top/gtzvxmincw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.zhoulong.xyz/gtahbyhejq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.zhoulong.xyz/gtayhlyjgn.html


<!-- 参考信息 -->