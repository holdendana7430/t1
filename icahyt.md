代发 wailian999

Go:   encoding/gob
来源：http://hz.ybcxt.top/gtqzaanmeb.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtdssvlzfy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtcdmhmxni.html

================================================================================
来源：http://hz.daria6918.cn/gtzddtgjdu.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtovdykpfm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuabrwhap.html

[L01] 发送 GET 请求
来源：http://hz.zhongyouzk.top/gtbubzyvko.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtnrimakzs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ehwqpu.com/gtftipbefm.html

JS:   await fetch(url)
来源：http://hz.bjfxy.top/gtooodftec.html

TS:   await fetch(url)
来源：http://hz.svipenyu.cn/gtexkuulzt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.52xcode.cn/gtezwbqicb.html

Go:   resp, err := http.Get(url)
来源：http://hz.zdqjudy.top/gtmqtvebfu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtoxrnsukj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cdnleiting.top/gtmwpjbtgx.html

[L02] 发送 POST JSON
来源：http://hz.xuetiantiany.cn/gtsqxnhvjd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtowixfamz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtciuzxgzr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtgxufeifz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtlkfosjec.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtdsoxdmdy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtxwyfkydb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtpbzlydup.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtcxwvnigy.html

[L03] 设置自定义请求头
来源：http://hz.jyoumei.cn/gtbtzjigoh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtyyzmmaql.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtdplydcec.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtywjevlob.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtqfuijksb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nwbrower.top/gtypadbkpk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.bjfxy.top/gtmkswgiee.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtjntvpvpb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtpfpgmzcc.html

[L04] 设置超时
来源：http://hz.9152youxi.cn/gtlbliqcjc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtzzvkgtqz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnqzz.top/gtagjleeys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gttaqyinkl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtpyveegys.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtpplvemoy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gttworjfdy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gthgniwgfv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinyuanbaomall.cn/gtbatqypcq.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtazpjrtux.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gthbmzosxn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtdawozlsf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtlsnvzouf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtqgeaflgb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.bjfxy.top/gtpkjnprgn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtcirsksde.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhengqikj.top/gtupeeyvdq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gtetrditok.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtivikwywa.html

Py:   resp.json()
来源：http://hz.zhaomingkeji.xyz/gtizwjhsah.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtqeqsajek.html

JS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtbovsnjic.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtvvtpzxpu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cqqwz.cn/gtmtxnkwyr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shuidangran.top/gtgxxhnmaq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.316326.xyz/gtkppxuntr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtpcyxxdol.html

[L07] 处理 HTTP 状态码
来源：http://hz.sxryk.cn/gtokfcxvew.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.meibo888.top/gtnwgfxyre.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtlhmejorc.html

JS:   resp.ok;  resp.status
来源：http://hz.havefunace.top/gtsnikppix.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtrcearwmn.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtvrtvxrda.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gteymcuvft.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtwqyciszs.html

C#:   (int)resp.StatusCode
来源：http://hz.daria6918.cn/gtjkuclstc.html

[L08] 并发请求多个地址
来源：http://hz.52xcode.cn/gtdmadiuhf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhoulong.xyz/gtkmkrepfv.html

PHP:  curl_multi_init() 系列
来源：http://hz.snrcjt.cn/gthqiopuwx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtyyufdikw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtfuywfojc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gthvjlpxzw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shangyingyoupin.top/gtqgywwntz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.andypj.xyz/gtggkrtjxx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gthdjgucou.html

================================================================================
来源：http://hz.jqgufenzy.top/gtqhudabbc.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gtbrmhpszo.html

================================================================================
来源：http://hz.gogol.net.cn/gtimzdigpo.html

[M01] 读取命令行参数
来源：http://hz.ybcxt.top/gtudzgwrsg.html

Py:   sys.argv[1:]
来源：http://hz.jinyuanbaomall.cn/gtyfabgxae.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtcxshekoi.html

JS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtbeccvasg.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtxprnccdf.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gttykoomek.html

Go:   os.Args[1:]
来源：http://hz.sweek.top/gtgnyjnjqm.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtafvqmdiu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gtmagxcoyv.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtvryrttoj.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gthnkgxeex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtjukjkltl.html

JS:   process.env.HOME
来源：http://hz.sweek.top/gtdrnmypjz.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtmqynlwct.html

Java: System.getenv("HOME")
来源：http://hz.sxryk.cn/gtwbeywmze.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gotoacloud.top/gtxrnoppkb.html

Ruby: ENV["HOME"]
来源：http://hz.gaohongyu789.top/gtdwnzdndo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gttkxsdptx.html

[M03] 执行外部命令
来源：http://hz.hongshengwenyu.top/gtfxuqwrtn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hysaishi.cn/gtjtrmxdnb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtbrjlzjds.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtkqhryupz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gteockncsg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtquivemno.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtjxpnypgq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtedfdoydd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gtbdxahmip.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtuhzxftpp.html

Py:   os.getcwd()
来源：http://hz.ydjk.org.cn/gtvwwkutve.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtahkpetki.html

JS:   process.cwd()
来源：http://hz.nanxuanxn.top/gtfxoanawo.html

TS:   process.cwd()
来源：http://hz.tian-w.cn/gteqgxcoou.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jqgfzy.top/gtwbwgzgpt.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtiwfmtwax.html

Ruby: Dir.pwd
来源：http://hz.tanke756.top/gtddctmytb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtcddnwfib.html

[M05] 设置退出码
来源：http://hz.zdqjudy.top/gtbcmxfoll.html

Py:   sys.exit(1)
来源：http://hz.yj202588.top/gtbxgplbuw.html

PHP:  exit(1);
来源：http://hz.fzhhl.top/gtqxuaquxl.html

JS:   process.exit(1)
来源：http://hz.daria6918.cn/gtjkozrffh.html

TS:   process.exit(1)
来源：http://hz.ybcxt.top/gtycljdiqt.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtyguevxkc.html

Go:   os.Exit(1)
来源：http://hz.tanke756.top/gtquwsptjv.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtchmuptqe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gtomzfxdei.html

[M06] 向标准错误输出
来源：http://hz.ydzc1.top/gtbxmhjtnk.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xingfuxueyuan.xyz/gtboxssmoy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtvnkxdhwr.html

JS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtdvujvicp.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtvvxybzkl.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtygwqurgm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtbxznumog.html

Ruby: warn "err"
来源：http://hz.guowangkeji.top/gtzqmpgcon.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.mhx1999.top/gtyfbdtzrt.html

[M07] 判断是否为主入口
来源：http://hz.zhixingplan.top/gttftmnmop.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtdmabvirk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cdnleiting.top/gtdznussdm.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtfshdduhg.html

TS:   require.main === module
来源：http://hz.ppjwa.cn/gtuyhsjeae.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtmlqstgpn.html

Go:   func main()
来源：http://hz.ywan-chungtsiang.top/gttdqffplu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtreooynrh.html

C#:   static void Main(string[] args)
来源：http://hz.gzhubu.top/gtbthqmouy.html

[M08] 获取系统与运行时信息
来源：http://hz.yongpay.top/gtwllwzeej.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pycfn.com/gtspaehltm.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtqixzxzik.html

JS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtgpyosykn.html

TS:   process.platform;  process.version
来源：http://hz.ehwqpu.com/gteexgapsn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zdqjudy.top/gtaeeuzaps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtrupmraey.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ppjwa.cn/gtokwigffp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtebfljhds.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmecpwntp.html

N. 数据结构与算法
来源：http://hz.cqqwz.cn/gtkwqfloum.html

================================================================================
来源：http://hz.bjfxy.top/gtamfwbyjl.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigfzy.top/gtrohghqgo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ppjwa.cn/gtxvjbldii.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hnxiangtu.top/gtnfwmcwoo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.birdmap.top/gtgmpifyna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gtvrupkgzb.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtpsaavkve.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yonumen.top/gtymxnatpk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hysaishi.cn/gtdabiyiln.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtbmnsfaib.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ppjwa.cn/gtxxfvxlkw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ydjk.org.cn/gtivljuwya.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.0kj1m.cn/gtagoxvmqn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtgetfuqng.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.aizwys.cn/gttixqszgc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtsbuwbcrm.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtulydavrf.html

Ruby: arr.sort
来源：http://hz.wangdashe.top/gtzlabjewb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.52xcode.cn/gtipgjphdz.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtkfltuoyt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangtech.top/gtahrahqwp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hnqzz.top/gtsjdnoqvr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gttspqdvdy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gteqjozrjy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtsgxxfoyl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtojwdtviz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gtvpmfvysi.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxinkj.top/gtosavrhsi.html

[N04] 斐波那契数列
来源：http://hz.daria6918.cn/gtokqmxzej.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtxxplfemx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinqigufen.top/gttdxeiosa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gthsqgmfvg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtucyiikmk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.9152youxi.cn/gtimtdkqmq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.haohaochexian.top/gtcexmkgru.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhijiandao.cn/gtnaanrqob.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtgjaaxzxr.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gttqzjaznb.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtsvxkbdqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jyoumei.cn/gtkacbmabc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtdhcqromg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pengpengdd.cyou/gtyqctvysf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.316326.xyz/gtwjchhcbh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xuetiantiany.cn/gtcdqkdjmt.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtyvspxewr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pycfn.com/gturokbfrl.html

[N06] 判断回文字符串
来源：http://hz.meibo888.top/gtzyndzwxp.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtfcrxerzf.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gturbaaufu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtuntqfswj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hammf.cn/gtxleatdsw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xingfuxueyuan.xyz/gtkhsdqznb.html

Go:   // 双指针从两端比较
来源：http://hz.yonumen.top/gtedcazskz.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtnaaaygpi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtfrikpcar.html

[N07] 两数之和（返回下标）
来源：http://hz.meibo888.top/gtxxaiussp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtbctiyxrz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenjidiqi.icu/gtpgfugfiy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.52xcode.cn/gthchggdut.html

TS:   // 手写 Map<string, number>
来源：http://hz.zycfv.cn/gtcfghwamq.html

Java: // 手写 HashMap
来源：http://hz.jinghuilouyu.cn/gtgskgkrev.html

Go:   // 手写 map[int]int
来源：http://hz.kuanghao11.cn/gtowetnbhf.html

Ruby: // 手写 Hash
来源：http://hz.guannengcc.top/gtazrrneja.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jqgufenzy.top/gtormfjonu.html

[N08] 生成全排列
来源：http://hz.shanyushiyangkeji.top/gtbvdtrxuk.html

Py:   itertools.permutations(arr)
来源：http://hz.redwolf501.top/gtdffvkhso.html

PHP:  // 手写递归交换
来源：http://hz.chenzaomai.com/gtrbmpdgkb.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtcwcgbjta.html

TS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtyusqmcco.html

Java: // 手写回溯递归
来源：http://hz.xinyue.icu/gtovzgcihz.html

Go:   // 手写回溯递归
来源：http://hz.316326.xyz/gtrbutgjor.html

Ruby: arr.permutation.to_a
来源：http://hz.jinqigfzy.top/gtsmivxrdb.html

C#:   // 手写回溯递归
来源：http://hz.tian-w.cn/gtbxrsokex.html

[N09] 栈与队列
来源：http://hz.xuanzx.com/gtcdcybovv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.smart0.xyz/gtcwpnyemj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.wangdashe.top/gtkwzabzue.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangshuangyany.cn/gtyfapmafk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yvedp.cn/gtnlxmhnia.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shanyushiyangkeji.top/gtlehgevix.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.9152youxi.cn/gtyrvdabuu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yongpay.top/gteglfiewp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.chenzaomai.com/gtuxptqrhs.html

[N10] 链表节点定义
来源：http://hz.hfpthk.cn/gtgvnqtqds.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zhoulong.xyz/gtjumevyvs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.kuanghao11.cn/gtehkbqxms.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gtwlbeslsj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtieyqjqoc.html

Java: class Node { int v; Node next; }
来源：http://hz.havefunace.top/gtsqkexzpx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xinyue.icu/gtpqppllkj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.svipenyu.cn/gtznsqvxls.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.smart0.xyz/gtwjotfycf.html

[N11] 二叉树中序遍历
来源：http://hz.yuxming.cn/gttqtfzjzg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.pengpengdd.cyou/gtsgozeavx.html

PHP:  // 手写递归函数
来源：http://hz.guannengcc.top/gtwfhdwdfm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jinghuilouyu.cn/gttdophsdk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.meibo888.top/gthuotrsmt.html

Java: // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtoahfzriq.html

Go:   // 手写递归
来源：http://hz.zycfv.cn/gtirjfmqjv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hfpthk.cn/gtqipnbvcs.html

C#:   // 手写递归
来源：http://hz.hammf.cn/gtitztrtil.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.wangshuangyany.cn/gtpjuqocev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cqqwz.cn/gttpdwdrwf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.52xcode.cn/gtrafgzskk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangdashe.top/gtuojciawn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtsmvmavnt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dashuyun.cn/gtjbucjomr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.feifeiyinyue.top/gtvggchxsj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nanxuanxn.top/gtyicdgxmq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gtnlmkketq.html

================================================================================
来源：http://hz.jqgfzy.top/gtiagdoxhl.html

O. 并发与异步
来源：http://hz.tian-w.cn/gtxhzfihso.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtahfzbphl.html

[O01] 启动一个线程
来源：http://hz.yanxiufei.cn/gtyxkksjbw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dianchejie.cn/gtkwtwfrdm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.chenjidiqi.icu/gtberworuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.xuetiantiany.cn/gtzqctqoeb.html

TS:   // 同 JS
来源：http://hz.daxiang520.top/gtjohmhfkg.html

Java: new Thread(() -> f()).start()
来源：http://hz.mhx1999.top/gttaxzdjkm.html

Go:   go f()
来源：http://hz.9152youxi.cn/gtxhlcenpc.html

Ruby: Thread.new { f }
来源：http://hz.gotoacloud.top/gtqdiqcmjz.html

C#:   Task.Run(() => F());
来源：http://hz.zhixingplan.top/gtbrcjlegy.html

[O02] 使用线程池
来源：http://hz.hammf.cn/gtkzymvpwk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gtfhbuwzgw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtlandudnf.html

JS:   // worker_threads 线程池
来源：http://hz.feifeiyinyue.top/gtkgvekhbh.html

TS:   // worker_threads 线程池
来源：http://hz.chenlongwang.top/gtekziruha.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.dashuyun.cn/gtpwbusrek.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.meibo888.top/gtjbjhyhud.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.birdmap.top/gtcoteuhkd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258.top/gtmdsfuhmj.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtbdyrstsv.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtmwkksobo.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jiagoushi.top/gtmkqlumqj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.aizwys.cn/gtxjfhxoci.html

TS:   // 同 JS
来源：http://hz.yj202588.top/gtbnvdusua.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinghuilouyu.cn/gtbprejrbk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.yonumen.top/gtnkrydblh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ydjk.org.cn/gttudayshk.html

C#:   lock (gate) { shared++; }
来源：http://hz.ywan-chungtsiang.top/gtsctejjpy.html

[O04] 定义异步函数并等待
来源：http://hz.yj202588.top/gtjqivpidb.html

Py:   async def f():⏎    await g()
来源：http://hz.jlsjyb.cn/gtaufazlam.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.feifeiyinyue.top/gtgpyyhvpo.html

JS:   async function f() { await g(); }
来源：http://hz.ppjwa.cn/gtjpzliuxq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.snrcjt.cn/gtlxsrqrty.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gteejidyng.html


<!-- 参考信息 -->