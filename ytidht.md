代发 wailian999

L. 网络请求
来源：http://hz.gaohongyu789.top/gtnrklxfpk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtoyivtmyc.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtwznlbtdo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtsbfgdfmk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtuflukjvy.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtscdymfey.html

TS:   await fetch(url)
来源：http://hz.xylfe.cn/gtydnjjpkx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtiwvmnpsh.html

Go:   resp, err := http.Get(url)
来源：http://hz.jinghuilouyu.cn/gtxsmxyxhm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtoyfbljlq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gttieofdqn.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gtgpamydho.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtwyomtxfq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtvffsycip.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtssczjykp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtwhhdrvjx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pycfn.com/gtorkvkeak.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtmgblytac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtiaqbubsz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtrnpijpaw.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtxqxybxup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtxqvyepte.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gotoacloud.top/gtgtogwzgq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtfoeodsve.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shzxlz.cn/gtozbjgsak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shangyingyoupin.top/gtggkyjhza.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtcoqkyqhz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtmzgtwimh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cdnleiting.top/gttycxrtod.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtczpzykdd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dianchejie.cn/gtgxmvyfts.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.birdmap.top/gtegnovear.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangtech.top/gtvriuffwz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtrjrgirad.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtimarbswg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gttfzzrtdu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtjsfomhcs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.c1oappe.top/gtipjbdlmg.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258.top/gthzzalrxk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtgjfhxvjp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gtxkcyebxz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gthbvrdqih.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtmeaceqgt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtmchnpzge.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtgskghqhi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aibaodan.cn/gtnegwdhvw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtgmeixaiy.html

[L06] 解析响应为 JSON
来源：http://hz.yanxiufei.cn/gtotevbort.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtclofnpkv.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtaufdppow.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gthcsuitwe.html

TS:   await resp.json()
来源：http://hz.chenzaomai.com/gtmdrhehgp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxuanxn.top/gtmwbojiuc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtqdkdreou.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtkkldnrgz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinqigufen.top/gtvbehauhu.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtrclqgkdf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhiwuduotai.top/gtllrohfrd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sweek.top/gtcoshclbi.html

JS:   resp.ok;  resp.status
来源：http://hz.316326.xyz/gtcjdxkhoh.html

TS:   resp.ok;  resp.status
来源：http://hz.yangfankeji.com/gtptbdrbzc.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtlznxlpld.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtajdpntrs.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtljrphnwm.html

C#:   (int)resp.StatusCode
来源：http://hz.shuidangran.top/gtlwsczqqz.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtrzbwjadh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tanke756.top/gtbkvziofg.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxinkj.top/gtjygqgmut.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtftateyce.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtveqezyrs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtzfzazfjv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.316326.xyz/gtmpenpeio.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gtpiqopnzx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtrpymkjnf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtsdwhcrla.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtivstzred.html

================================================================================
来源：http://hz.yj20258888.top/gtpzojrcvg.html

[M01] 读取命令行参数
来源：http://hz.ydzc1.top/gtwqjdmqqe.html

Py:   sys.argv[1:]
来源：http://hz.haohaochexian.top/gtlypimnbv.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtdoynloqu.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtlgirxhgi.html

TS:   process.argv.slice(2)
来源：http://hz.jianghu66.top/gtxkvlisob.html

Java: args 数组（main 方法参数）
来源：http://hz.andypj.xyz/gtgibbprxq.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtfzjyehse.html

Ruby: ARGV
来源：http://hz.daria6918.cn/gtwtqmygok.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtldauisdv.html

[M02] 读取环境变量
来源：http://hz.c1oappe.top/gtuzcgoxum.html

Py:   os.environ.get("HOME")
来源：http://hz.pycfn.com/gtyljmbxfk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xinyue.icu/gtvsoqkcne.html

JS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtjvltqjjy.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gthizbwess.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtwkfkenus.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhiwuduotai.top/gtmuzificf.html

Ruby: ENV["HOME"]
来源：http://hz.hammf.cn/gtwyhveziq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hongshengwenyu.top/gtlkgdpxeu.html

[M03] 执行外部命令
来源：http://hz.ivvv.top/gtseumwfxm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gtcrdrvrcc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangtech.top/gtsdimyptm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtwmelbixj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtddpgdibp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgufenzy.top/gtndryvzbc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hysaishi.cn/gtxeifxhfo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.9152youxi.cn/gtwxzrrfvj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydzc1.top/gtolhsffhw.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtcevcdyps.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gttdrmyoid.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtfsqfbwzj.html

JS:   process.cwd()
来源：http://hz.yanxiufei.cn/gtskrcsktk.html

TS:   process.cwd()
来源：http://hz.shangyingyoupin.top/gtrwcumphe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shuidangran.top/gtmfzyevcz.html

Go:   os.Getwd()
来源：http://hz.aibaodan.cn/gtkzgeyiwk.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtequjuxrj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.havefunace.top/gtkggxrwdm.html

[M05] 设置退出码
来源：http://hz.dashuyun.cn/gtmctvkwln.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtslbwdavy.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtshbxnhor.html

JS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtzbcgpbru.html

TS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtfsggbwcf.html

Java: System.exit(1)
来源：http://hz.redwolf501.top/gtnfvryqoe.html

Go:   os.Exit(1)
来源：http://hz.hnxiangtu.top/gtrfrhgyfc.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtwvpddddk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tianlin.xyz/gtbzkjaqsf.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtfrlcgaco.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtlwiovmym.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtxxfggxat.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtznidojjt.html

TS:   console.error("err")
来源：http://hz.jyoumei.cn/gteypnwnla.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtvrnnpzxd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtggtcmezm.html

Ruby: warn "err"
来源：http://hz.bjfxy.top/gtyjglyvce.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtirhdfkyp.html

[M07] 判断是否为主入口
来源：http://hz.cashguo.top/gtsnjlscja.html

Py:   if __name__ == "__main__":
来源：http://hz.tian-w.cn/gtmoyivfhz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhijiandao.cn/gtccmuwxsg.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gttomjmjba.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtzyqzjspb.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtkvhembta.html

Go:   func main()
来源：http://hz.zhongyouzk.top/gtgajpkavh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yangfankeji.com/gtsylxistd.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtrpxstnmu.html

[M08] 获取系统与运行时信息
来源：http://hz.zhoulong.xyz/gtltgkcbxr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dashuyun.cn/gtvewbqrhu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtaopydpuy.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtpxewmcfs.html

TS:   process.platform;  process.version
来源：http://hz.tanke756.top/gtjpobcvou.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hnqzz.top/gtczhovork.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.vqdsnc.cn/gtuugwmbdy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtaiupdrxc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.fengsongda.top/gtufbhvpgv.html

================================================================================
来源：http://hz.kuanghao11.cn/gtslnrtvvd.html

N. 数据结构与算法
来源：http://hz.jqgufenzy.top/gtaqlaslhm.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtbblxjtsd.html

[N01] 二分查找（有序数组）
来源：http://hz.haohaochexian.top/gthgelokpd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtsrtvomgf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dashuyun.cn/gtdchqknab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtpqvoxcmq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258.top/gtxsxuvvws.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtrzajhlvv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtunksqkur.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtcrjlvbtg.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.daria6918.cn/gtnueujuiu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cashguo.top/gtxnhoitya.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gtwhsacace.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinghuilouyu.cn/gtmujtxdtf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtxvuqbcck.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtcttiylwf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtfcocwfab.html

Go:   slices.Sort(arr)
来源：http://hz.xuanzx.com/gtezpszofw.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtvjqkfcvo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.pengpengdd.cyou/gttbsrpghg.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtbfiacviw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.haohaochexian.top/gttjnumbya.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtqewqamph.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gotoacloud.top/gtozomdbuw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtaaxpdblw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtuutnggji.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gteytrkozd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.9152youxi.cn/gteugormhj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.quarkkingdee.top/gtzuwmewgw.html

[N04] 斐波那契数列
来源：http://hz.chenjidiqi.icu/gtefagfwof.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jinyuanbaomall.cn/gtqnfeheli.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtgdnwedqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daria6918.cn/gtmegtzkfm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtjuwidfwm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtzyllfohx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhiwuduotai.top/gtvkcwbhds.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtoiqwfgcv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.guannengcc.top/gtzjemdvli.html

[N05] 最大公约数
来源：http://hz.yueranfly.top/gtxwuhhxif.html

Py:   math.gcd(a, b)
来源：http://hz.quarkkingdee.top/gtfutahjps.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.ydzc1.top/gtjdvneubb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtgunmysxp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtczxnoilo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.9152youxi.cn/gtvvruqbxl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yanxiufei.cn/gtpsoueyzy.html

Ruby: a.gcd(b)
来源：http://hz.tianlin.xyz/gtpylldqnt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.9152youxi.cn/gteksirfvt.html

[N06] 判断回文字符串
来源：http://hz.yanxiufei.cn/gtdlmohbxx.html

Py:   s == s[::-1]
来源：http://hz.cqqwz.cn/gtkqjdhocj.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtgusscjnu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangtech.top/gtxqibognb.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtixtiplsx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhengqikj.top/gtbkauskof.html

Go:   // 双指针从两端比较
来源：http://hz.shuidangran.top/gtqiufxzrm.html

Ruby: s == s.reverse
来源：http://hz.zhongyouzk.top/gtexcdxgjz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gteawznjcx.html

[N07] 两数之和（返回下标）
来源：http://hz.xingfuxueyuan.xyz/gtkhxsxrki.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.zycfv.cn/gteepysczu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.svipenyu.cn/gtjqohvbcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pycfn.com/gtzgzdtdgy.html

TS:   // 手写 Map<string, number>
来源：http://hz.daxiang520.top/gtzvduuhgb.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtchipnsmp.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gtqjyoymmz.html

Ruby: // 手写 Hash
来源：http://hz.ydjk.org.cn/gtqjxwucsd.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hfpthk.cn/gtjunlbgpr.html

[N08] 生成全排列
来源：http://hz.0kj1m.cn/gtceydrgxh.html

Py:   itertools.permutations(arr)
来源：http://hz.zhengqikj.top/gtggtphbzy.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtoztxxvdw.html

JS:   // 手写回溯递归
来源：http://hz.snrcjt.cn/gtzswpqkip.html

TS:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtcgrckran.html

Java: // 手写回溯递归
来源：http://hz.pycfn.com/gtjbhwfgmc.html

Go:   // 手写回溯递归
来源：http://hz.daxiang520.top/gttfycezwl.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtrqkxrkqu.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtkzxduofc.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtoirizijm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yuxming.cn/gthlhfnvky.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hysaishi.cn/gtnjztprji.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jqgfzy.top/gtjipbtxrj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yuanzhike.top/gttnnpcbmz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhengqikj.top/gtehplrwic.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.mhx1999.top/gttugrlzdo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zycfv.cn/gtbaeifmrs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zdqjudy.top/gtrngstowi.html

[N10] 链表节点定义
来源：http://hz.daxiang520.top/gtaiyetqdq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.9152youxi.cn/gtfloqcwfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.52xcode.cn/gtyduczfae.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.316326.xyz/gthgukltgf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fengsongda.top/gtcoqjjiml.html

Java: class Node { int v; Node next; }
来源：http://hz.ydzc1.top/gtlvmscids.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.smart0.xyz/gtaeqpkanr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yueranfly.top/gthyvcxglf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jiagoushi.top/gtyonrptyr.html

[N11] 二叉树中序遍历
来源：http://hz.birdmap.top/gtvamzzias.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtgaiezznh.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gtlhxaqnni.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.quarkkingdee.top/gtitbsbcia.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtiybrlqxv.html

Java: // 手写递归
来源：http://hz.ydzc1.top/gtjvelewwh.html

Go:   // 手写递归
来源：http://hz.zhengqikj.top/gthgpwhowb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnqzz.top/gtjxiurrba.html

C#:   // 手写递归
来源：http://hz.daxiang520.top/gtlzspngrx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.tanke756.top/gtfqurqrxp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ehwqpu.com/gthwypstdu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jyoumei.cn/gtiuphkfvz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yongpay.top/gtdhattrqb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtplhkxwbk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jiagoushi.top/gtriyawuzm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gtwyevaphj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.zhiwuduotai.top/gtmjdmfpjw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.hnxiangtu.top/gtmpfldjcz.html

================================================================================
来源：http://hz.daria6918.cn/gtmzytojzz.html

O. 并发与异步
来源：http://hz.shanyushiyangtech.top/gttxzseibo.html

================================================================================
来源：http://hz.bjfxy.top/gtebhcdbqc.html

[O01] 启动一个线程
来源：http://hz.daxiang520.top/gtnyhgeqtd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.tian-w.cn/gtdyzrwpiv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.dashuyun.cn/gtschoyyrs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jinqigufen.top/gtcokoozhq.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtbdaiwnvo.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigufen.top/gttesizxld.html

Go:   go f()
来源：http://hz.yj20258888.top/gtmtywredd.html

Ruby: Thread.new { f }
来源：http://hz.9152youxi.cn/gtlwgdjhot.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtvmznaync.html

[O02] 使用线程池
来源：http://hz.sysykeji.top/gtjoltxkgy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.iojbl.cn/gtfzsrefwx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tian-w.cn/gtkebysndm.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtvelxhufl.html

TS:   // worker_threads 线程池
来源：http://hz.0kj1m.cn/gttxmxoqvg.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.bjfxy.top/gtnmqglvit.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yj20258888.top/gtmixvhtqc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenzaomai.com/gtmyofmarf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinyuanbaomall.cn/gtvrchmwki.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gtfxnzyidq.html

Py:   with lock: shared += 1
来源：http://hz.ppjwa.cn/gtcxzhqaty.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnxiangtu.top/gtcnpynkof.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhijiandao.cn/gthtjwdbzz.html

TS:   // 同 JS
来源：http://hz.birdmap.top/gtgydffdzf.html

Java: synchronized (this) { shared++; }
来源：http://hz.ydzc1.top/gtakyxbczn.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daria6918.cn/gtvfdefprm.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jianghu66.top/gtkkqjnbft.html

C#:   lock (gate) { shared++; }
来源：http://hz.jinqigfzy.top/gtnqqgzzas.html

[O04] 定义异步函数并等待
来源：http://hz.mhx1999.top/gtighbccwg.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtoaffounk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gtyblyidze.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gtuolfckud.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.dianchejie.cn/gtnjjpfryf.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gzhubu.top/gtzcigrwig.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.jyoumei.cn/gttkeatcgs.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gthcagmqxs.html

C#:   async Task F() { await G(); }
来源：http://hz.havefunace.top/gtveznqwmu.html

[O05] 并发执行并等待全部完成
来源：http://hz.tianlin.xyz/gtacwajkxg.html


<!-- 参考信息 -->