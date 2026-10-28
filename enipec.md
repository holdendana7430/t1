代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtdbyitqzh.html

JS:   await fetch(url)
来源：http://hz.shuidangran.top/gtguxahunt.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtchdrlwas.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhongyouzk.top/gtdiucqwqu.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtlmuksmes.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtisrnoxka.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangshuangyany.cn/gtvawxcgru.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtbmkqxilv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtbauahmew.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtqlibmnic.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gttbmrcuht.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtsahbmkzb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtzhfwyeno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gtozypqfpf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtajtxzbjm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258.top/gtceztucul.html

[L03] 设置自定义请求头
来源：http://hz.nanxinkj.top/gtvbjtsapp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtibdynzhf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtqrgwdxif.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhaomingkeji.xyz/gtxnygitdr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtzzfrriqx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtedjsldnc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtpijolppg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtwzxablqr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtayjxybrb.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtbjpfqwbv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhoulong.xyz/gtfhijzyfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtmecbzwfy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gogol.net.cn/gtrcecwaae.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gttvnbtqta.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgufenzy.top/gtnyglrqzs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtfdwndans.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cdnleiting.top/gtraxwrrzz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gttavrdrzs.html

[L05] 上传文件（multipart）
来源：http://hz.hnxiangtu.top/gtokgmmvln.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cucudq.cn/gtmcjoqmmb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtzzrtbnns.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtgdyrfpwl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtiblmkffq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.0kj1m.cn/gtsiftrvxe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtvlshfpbh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.daria6918.cn/gtflylkwth.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtvndvwxef.html

[L06] 解析响应为 JSON
来源：http://hz.zhixingplan.top/gtuvloztku.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtfzkertqk.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtreucmgkc.html

JS:   await resp.json()
来源：http://hz.birdmap.top/gthuglahwr.html

TS:   await resp.json()
来源：http://hz.dianchejie.cn/gtbwyzlcna.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtxjyibrcd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.feifeiyinyue.top/gtqseuqtnq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtnijwsnfi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.smart0.xyz/gttiousinm.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtmsnemqyf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydjk.org.cn/gtwauktqpt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.feifeiyinyue.top/gtfhoerdov.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtyxadktej.html

TS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtqyvaoddt.html

Java: resp.statusCode()
来源：http://hz.ivvv.top/gtlxrejlmh.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtprnolbnp.html

Ruby: resp.code.to_i
来源：http://hz.cdnleiting.top/gtjueabpbm.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtdxxavmcs.html

[L08] 并发请求多个地址
来源：http://hz.guannengcc.top/gtenehwhsg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtubyvvggq.html

PHP:  curl_multi_init() 系列
来源：http://hz.cashguo.top/gtczjpmylz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtdzepzgts.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigufen.top/gtsffgrdnh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xingfuxueyuan.xyz/gtlovxwvnu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtjhzuxmtd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hysaishi.cn/gtnjspadne.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.redwolf501.top/gtwsdszjhi.html

================================================================================
来源：http://hz.yueranfly.top/gtwxxouavg.html

M. 命令行 / 进程 / 环境
来源：http://hz.cheryme.top/gtiyuvttue.html

================================================================================
来源：http://hz.cqqwz.cn/gtuhmjqjyj.html

[M01] 读取命令行参数
来源：http://hz.dashuyun.cn/gtqroutdew.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtzoblopjj.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtejbjzkly.html

JS:   process.argv.slice(2)
来源：http://hz.yuanzhike.top/gtltnpvqft.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtswufzilf.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtrzbrhcfz.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtvjbllrll.html

Ruby: ARGV
来源：http://hz.jinghuilouyu.cn/gtgesrvqlh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtjhlyzcxg.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtwzwxxftk.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtpgncpgsi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gtoygwxfye.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtwmwgrtkn.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtcottphaf.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtfvsdydde.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtbagxqdet.html

Ruby: ENV["HOME"]
来源：http://hz.kuanghao11.cn/gtneeddpab.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtoewseubo.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtefkufjwu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtmvglvaqf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtnsnnwbfh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gttmtbnspa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtcmbmkwgh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hywenlv.cn/gtdhiaozea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhongyouzk.top/gtjyklrfkl.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnxiangtu.top/gthhkdartl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258888.top/gtjqixcmdc.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtwuafmnif.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtqfyvdhgk.html

PHP:  getcwd();
来源：http://hz.daria6918.cn/gtfotydhcm.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtcewqzaqi.html

TS:   process.cwd()
来源：http://hz.zycfv.cn/gtttwfbnxt.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtbnzduaxw.html

Go:   os.Getwd()
来源：http://hz.yangfankeji.com/gtuurmpdag.html

Ruby: Dir.pwd
来源：http://hz.gaohongyu789.top/gttowukkph.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tianlin.xyz/gtlxdyeqty.html

[M05] 设置退出码
来源：http://hz.ivvv.top/gtbozsadss.html

Py:   sys.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtygibxmat.html

PHP:  exit(1);
来源：http://hz.nanxinkj.top/gtwqgucflc.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtowifsnju.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtaxlpbbqo.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtjzvnksih.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtqndtrllg.html

Ruby: exit 1
来源：http://hz.guowangkeji.top/gtpdlrpczo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinyuanbaomall.cn/gtbmbpbxmj.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangkeji.top/gtytxykosg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gtpwaqzjrl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtjtqdricw.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtmwbflpvr.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtqexlpqzm.html

Java: System.err.println("err")
来源：http://hz.hnxiangtu.top/gtmtayezdx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtonmxyvdm.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtyoipfbjl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tian-w.cn/gtuobpcxas.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtcmnfngev.html

Py:   if __name__ == "__main__":
来源：http://hz.chenjidiqi.icu/gtzyimhime.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.mhx1999.top/gtleuzkvhh.html

JS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtkkgzlnrc.html

TS:   require.main === module
来源：http://hz.wangdashe.top/gtecngpfxk.html

Java: public static void main(String[] args)
来源：http://hz.kuanghao11.cn/gtqhnkuyud.html

Go:   func main()
来源：http://hz.svipenyu.cn/gtstyhgdxa.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gtmrcgnung.html

C#:   static void Main(string[] args)
来源：http://hz.chenzaomai.com/gtqycqlpfw.html

[M08] 获取系统与运行时信息
来源：http://hz.ydzc1.top/gthonmjjof.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtoqxszssw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.mhx1999.top/gtmjixcggf.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtijfiqykx.html

TS:   process.platform;  process.version
来源：http://hz.jiagoushi.top/gtuwcpdeue.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtxfjqiidw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.andypj.xyz/gtsfadzqzi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtpmupscbh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnxiangtu.top/gtenwhrffi.html

================================================================================
来源：http://hz.xziqi.cn/gtqwjygvam.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtjycvaphn.html

================================================================================
来源：http://hz.cdnleiting.top/gtxuigkqod.html

[N01] 二分查找（有序数组）
来源：http://hz.zhengqikj.top/gtvwaqkfiu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.wangdashe.top/gtwtbwrduu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtaffxutla.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtbttkewht.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtijagiehy.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.andypj.xyz/gtmuexzari.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gogol.net.cn/gtuouxyqgm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhengqikj.top/gttbxfiyui.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gttwqirdzc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hongshengwenyu.top/gtjnzvwipw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtdgtllxkf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gtuijyahqe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuxming.cn/gtyfmuevoc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtuwmzmawj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.shanyushiyangkeji.top/gtznzbrlvp.html

Go:   slices.Sort(arr)
来源：http://hz.cashguo.top/gtzkujpfyu.html

Ruby: arr.sort
来源：http://hz.jiagoushi.top/gtznoogoot.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shuidangran.top/gtuljwunwl.html

[N03] 快速排序（分治示例）
来源：http://hz.haohaochexian.top/gtpvyjqjkb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtggctiljy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yanxiufei.cn/gtzkbvkpur.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ywan-chungtsiang.top/gtsulxctxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtvkdbwbrc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtbyrjirez.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.gaohongyu789.top/gtawgndmci.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.52xcode.cn/gtmntaymxv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gtferxtqvr.html

[N04] 斐波那契数列
来源：http://hz.dianchejie.cn/gtulcxgarb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jqgufenzy.top/gtdlpjcpqi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.cucudq.cn/gthyqffald.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cheryme.top/gtjzlnipnn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtkkhfopoz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hammf.cn/gtqvjpphxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangkeji.top/gtvnfnhkip.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtvwvmdimr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenjidiqi.icu/gttjmncols.html

[N05] 最大公约数
来源：http://hz.quarkkingdee.top/gtrlanoxlb.html

Py:   math.gcd(a, b)
来源：http://hz.yongpay.top/gtpvwpkada.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtgmyljjyt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtalcidlbc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cucudq.cn/gtssfxcucd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jinghuilouyu.cn/gtxrmeuplg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtursvwvjp.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gtqfizpwjy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hfpthk.cn/gtjabsomks.html

[N06] 判断回文字符串
来源：http://hz.shanyushiyangkeji.top/gtpnlocypl.html

Py:   s == s[::-1]
来源：http://hz.jianghu66.top/gtmmyjbajg.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtdqxtgjua.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtirrxgzzp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtdhrttblt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shangyingyoupin.top/gtmvjxqslv.html

Go:   // 双指针从两端比较
来源：http://hz.gotoacloud.top/gtcmapdono.html

Ruby: s == s.reverse
来源：http://hz.xuetiantiany.cn/gtwweuctzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtfsxqooyg.html

[N07] 两数之和（返回下标）
来源：http://hz.zhongyouzk.top/gtwrlswkia.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.haohaochexian.top/gtpgqxpldj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cdnleiting.top/gthpbkhnvz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.andypj.xyz/gtrsjodfsl.html

TS:   // 手写 Map<string, number>
来源：http://hz.ydjk.org.cn/gtrnfbzmyl.html

Java: // 手写 HashMap
来源：http://hz.nanxinkj.top/gtvmmctnjr.html

Go:   // 手写 map[int]int
来源：http://hz.haohaochexian.top/gtpusibjqk.html

Ruby: // 手写 Hash
来源：http://hz.hnqzz.top/gtkmmmmpej.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.ywan-chungtsiang.top/gtklohyqkn.html

[N08] 生成全排列
来源：http://hz.yueranfly.top/gtysqeqqfs.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtzkfrquee.html

PHP:  // 手写递归交换
来源：http://hz.daria6918.cn/gtdhzygwfd.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtdcscfjnj.html

TS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtffglxulh.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtyvqwmjkm.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtykynlego.html

Ruby: arr.permutation.to_a
来源：http://hz.iojbl.cn/gtpzjhvnzv.html

C#:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtgnrasmlm.html

[N09] 栈与队列
来源：http://hz.gaohongyu789.top/gtaybsznfk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtnukwihig.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenjidiqi.icu/gttvxanryd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinghuilouyu.cn/gtslvfaalh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tanke756.top/gtjnjpqilx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.cashguo.top/gtezefouvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.shuidangran.top/gthaikrxsl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.316326.xyz/gtdntiyzul.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nwbrower.top/gtdgtcfqga.html

[N10] 链表节点定义
来源：http://hz.cheryme.top/gtukeozzsw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtbfacqcgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtubiognnr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhaomingkeji.xyz/gtwyaqlgct.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.cdnleiting.top/gtzimbiqvf.html

Java: class Node { int v; Node next; }
来源：http://hz.daria6918.cn/gtfostusel.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtfzosoabi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.wangshuangyany.cn/gtrbhjjlaq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.hnxiangtu.top/gtcymxfnwm.html

[N11] 二叉树中序遍历
来源：http://hz.aibaodan.cn/gtmitpzggb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.quarkkingdee.top/gticxhodof.html

PHP:  // 手写递归函数
来源：http://hz.daxiang520.top/gtebtpdehm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtzgvlqozd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cucudq.cn/gtqrhbnqgl.html

Java: // 手写递归
来源：http://hz.shanyushiyangtech.top/gtvqvyvzhm.html

Go:   // 手写递归
来源：http://hz.bjfxy.top/gtbzywawml.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.hnxiangtu.top/gtfirxdsga.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gtiqjwiqmy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhongyouzk.top/gthauzpktr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.cdnleiting.top/gtfzostfhi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jinqigfzy.top/gtdcpzfzec.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gtvdpbkyos.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.feifeiyinyue.top/gtedjxzziv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtfwdtolkj.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtcxysqula.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtscjdajsj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yanxiufei.cn/gtvpwlbwxc.html

================================================================================
来源：http://hz.andypj.xyz/gtcawsjtve.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtaihgxjma.html

================================================================================
来源：http://hz.xuanzx.com/gtsslgdjnq.html

[O01] 启动一个线程
来源：http://hz.tianlin.xyz/gtlcewuray.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ivvv.top/gtaphdntsx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.daria6918.cn/gtqounlwwf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.meibo888.top/gtsfakmwjw.html

TS:   // 同 JS
来源：http://hz.dianchejie.cn/gtoolrqovh.html

Java: new Thread(() -> f()).start()
来源：http://hz.bjfxy.top/gtgsheemav.html

Go:   go f()
来源：http://hz.tianlin.xyz/gtgdgekfyb.html

Ruby: Thread.new { f }
来源：http://hz.zdqjudy.top/gtfwtqjspk.html

C#:   Task.Run(() => F());
来源：http://hz.jqgufenzy.top/gtafeooctc.html

[O02] 使用线程池
来源：http://hz.xingfuxueyuan.xyz/gtwtrpvomi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.sufxvd.cn/gtgvyiaxdw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hongshengwenyu.top/gtbthkhkpk.html

JS:   // worker_threads 线程池
来源：http://hz.zhaomingkeji.xyz/gtzlbzfatl.html

TS:   // worker_threads 线程池
来源：http://hz.yanxiufei.cn/gtxbxjvhyr.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gtkyrjcwdt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuxming.cn/gtxpvayvkl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhengqikj.top/gtevarmrza.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.kuanghao11.cn/gtqdklnmzy.html

[O03] 加锁保护共享数据
来源：http://hz.hfpthk.cn/gtefmbtejy.html

Py:   with lock: shared += 1
来源：http://hz.gaohongyu789.top/gtlwvnxdul.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.daxiang520.top/gtxtwsplgc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ywan-chungtsiang.top/gtzdtiqsls.html

TS:   // 同 JS
来源：http://hz.xingfuxueyuan.xyz/gtlmwpdewl.html

Java: synchronized (this) { shared++; }
来源：http://hz.xuetiantiany.cn/gtfckebnst.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.dianchejie.cn/gtmcpnioim.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jlsjyb.cn/gtxvigqkfm.html

C#:   lock (gate) { shared++; }
来源：http://hz.yj20258888.top/gthsnzobef.html

[O04] 定义异步函数并等待
来源：http://hz.cdnleiting.top/gtgopstpmg.html

Py:   async def f():⏎    await g()
来源：http://hz.xylfe.cn/gtiebfkjga.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jyoumei.cn/gtrqbwsybl.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtrtxjxeye.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.cqqwz.cn/gtkgvxuqjg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.yongpay.top/gtziqwhtyz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.pycfn.com/gtkbbzggce.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.yongpay.top/gthyovsauf.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtsbgqmhyv.html

[O05] 并发执行并等待全部完成
来源：http://hz.redwolf501.top/gtlywzefvv.html

Py:   asyncio.gather(*tasks)
来源：http://hz.kuanghao11.cn/gtkmnepkcz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.jqgufenzy.top/gtlwotlffh.html

JS:   await Promise.all(tasks)
来源：http://hz.cdnleiting.top/gtwqtlucwi.html

TS:   await Promise.all(tasks)
来源：http://hz.yangfankeji.com/gtsudpzrft.html


<!-- 参考信息 -->