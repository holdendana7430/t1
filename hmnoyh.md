代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtesszygaa.html

JS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtqeqqzrhy.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtjiknzfiy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtdzswqrpn.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhiwuduotai.top/gtzocsmoyq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.snrcjt.cn/gtbbktysbv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hywenlv.cn/gtmruwzvgu.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtsgunpfxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gttrjwlomd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtrqezocjh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtawyzxrdp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtwibsaaiq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yueranfly.top/gtreuligga.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ybcxt.top/gtewgldcsi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtkstasqcr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtlfkcfsup.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtflmheiuv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.smart0.xyz/gtfiohhoci.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtlmtkziak.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gttvifdqkx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtesuahzbz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.redwolf501.top/gtrujnrioi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuxming.cn/gtypcoeevh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtanxknqgz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtejzsfrsr.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtfobdgqhd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jyoumei.cn/gteewmchws.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhaomingkeji.xyz/gtkgmglhyg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtwavmygsl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtpgxzbywi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtqpfxsjvn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtxndgtkmw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.52xcode.cn/gteqevbnjn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtvndxinmh.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gthutlpdhx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnxiangtu.top/gtkfzulssi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gtuiwrszeo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtrrwmvwck.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtgkhlbqka.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fengsongda.top/gtmvsmmwdh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhiwuduotai.top/gttfwbqips.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.52xcode.cn/gtkzynkfmm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.316326.xyz/gtymyfujtg.html

[L06] 解析响应为 JSON
来源：http://hz.c1oappe.top/gtshwqzlbn.html

Py:   resp.json()
来源：http://hz.iojbl.cn/gtyxowjbzu.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gtuizujufg.html

JS:   await resp.json()
来源：http://hz.ppjwa.cn/gtxbblqaac.html

TS:   await resp.json()
来源：http://hz.andypj.xyz/gtbvnmntea.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtirlzbvag.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtcykkszst.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtvtdzklwd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtkuijqhmz.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtzuambpvd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cqqwz.cn/gtxwrbwabr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtcimomfuz.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtcvqgbqeg.html

TS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtoejyktmy.html

Java: resp.statusCode()
来源：http://hz.jinqigfzy.top/gtvohtselb.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtloxdfubd.html

Ruby: resp.code.to_i
来源：http://hz.zycfv.cn/gtayltgstg.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgfzy.top/gtvosteuxs.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtmutnlvwe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtdjylopve.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinghuilouyu.cn/gtpqmsvzat.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtbwbucixl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtchonrckt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtghvoziyo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sysykeji.top/gtkwkmcxuj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yangfankeji.com/gtratikeer.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yanxiufei.cn/gtsganbydc.html

================================================================================
来源：http://hz.yangfankeji.com/gtqqqvkbjy.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtmvfzpzpn.html

================================================================================
来源：http://hz.andypj.xyz/gtxeljwehd.html

[M01] 读取命令行参数
来源：http://hz.andypj.xyz/gtgwpllask.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtrdeypvsd.html

PHP:  $argv;  $argc;
来源：http://hz.daria6918.cn/gtsmenxgab.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtbrqgofqm.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtkgecnmok.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtxcmasgjx.html

Go:   os.Args[1:]
来源：http://hz.havefunace.top/gtyvciywrc.html

Ruby: ARGV
来源：http://hz.yj20258.top/gtiulynaek.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenlongwang.top/gtkbmebuyd.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtxgmyaigv.html

Py:   os.environ.get("HOME")
来源：http://hz.nwbrower.top/gtysxatvgb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtyvsicvpb.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtzshocfwi.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtsnpxepnm.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtvsibejty.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yvedp.cn/gtaadleamj.html

Ruby: ENV["HOME"]
来源：http://hz.cdnleiting.top/gtvbflhfai.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.c1oappe.top/gtaaexrrmc.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtujeucmjv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ybcxt.top/gtgesqzimv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtjkkajriz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gttkwyxfuq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtckwxjifx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fengsongda.top/gtqidrspgv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.haohaochexian.top/gtcgtgzkxh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtwokmrrzg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.birdmap.top/gtqgaunlcb.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtlwgytosr.html

Py:   os.getcwd()
来源：http://hz.xziqi.cn/gtideqmhuj.html

PHP:  getcwd();
来源：http://hz.ivvv.top/gtxvvohdrq.html

JS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtzujpohmn.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gthpokkuzq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zdqjudy.top/gtrnsgedpt.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtufjtvdzw.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtbomgtgwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gaohongyu789.top/gtdpdlnhqi.html

[M05] 设置退出码
来源：http://hz.c1oappe.top/gtvhkdqote.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gttmatxofo.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtskxbsaya.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gttbhvpeot.html

TS:   process.exit(1)
来源：http://hz.shanyushiyangtech.top/gtwbpfvgee.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gthpzicqvo.html

Go:   os.Exit(1)
来源：http://hz.zhengqikj.top/gtcmnbekyu.html

Ruby: exit 1
来源：http://hz.shangyingyoupin.top/gtgorhcrcl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dianchejie.cn/gtlqriawxy.html

[M06] 向标准错误输出
来源：http://hz.jinqigufen.top/gtdlmmfdxf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guowangkeji.top/gtwydkbbur.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.redwolf501.top/gtjbmueamq.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gtxdncugio.html

TS:   console.error("err")
来源：http://hz.cucudq.cn/gtimiwyqko.html

Java: System.err.println("err")
来源：http://hz.chenlongwang.top/gtsysuzzam.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xylfe.cn/gtxjbbwkfr.html

Ruby: warn "err"
来源：http://hz.jinghuilouyu.cn/gtbqmebdhs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.pycfn.com/gtngthmwcz.html

[M07] 判断是否为主入口
来源：http://hz.shanyushiyangkeji.top/gtkjbjzjmd.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtgkacdjjj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cucudq.cn/gtbgjfnowx.html

JS:   require.main === module
来源：http://hz.ehwqpu.com/gtkivvkwnm.html

TS:   require.main === module
来源：http://hz.jyoumei.cn/gtrzmyfjop.html

Java: public static void main(String[] args)
来源：http://hz.ehwqpu.com/gtrxvtkvta.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtmmkrdyzu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shuidangran.top/gtuaiduqsm.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtbnvjmolg.html

[M08] 获取系统与运行时信息
来源：http://hz.jqgufenzy.top/gtiqihtikm.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cqqwz.cn/gtwbykijoj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.snrcjt.cn/gtvhbxknzo.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gttnlrhirt.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtahigjiex.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shuidangran.top/gtolesuaqi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinghuilouyu.cn/gtkpxrzntu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.havefunace.top/gthwsonszq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhiwuduotai.top/gtyjqtikuv.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxkanihls.html

N. 数据结构与算法
来源：http://hz.zhengqikj.top/gtkdgwwnlo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdhmrkodr.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtiaoeqwyw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhengqikj.top/gtzstkmexn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yangfankeji.com/gthfjxcmpp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtnqzwxgoc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtxolqjukq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hywenlv.cn/gtmuozzabm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtpiidrsxm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtubgfjuug.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gtxdfwxykz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.smart0.xyz/gtpeztpyhl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtyktrlysy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cdnleiting.top/gtbejnnejy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtkkdytyzq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ybcxt.top/gtgtdksxud.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dianchejie.cn/gtshboumsv.html

Go:   slices.Sort(arr)
来源：http://hz.jqgfzy.top/gttxwhzcbs.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtqdhxncpl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgfzy.top/gtzyhjjrio.html

[N03] 快速排序（分治示例）
来源：http://hz.redwolf501.top/gtugwyktch.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtvqwfinms.html

PHP:  // 递归实现，或用 usort
来源：http://hz.ivvv.top/gtjrrjkljb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gteygawnho.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtvhwmcygx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yanxiufei.cn/gtdqhakhim.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xuetiantiany.cn/gtdlfuooeb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hfpthk.cn/gthcvpcbob.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtyhczcshc.html

[N04] 斐波那契数列
来源：http://hz.yongpay.top/gtcmcmoqgc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtghtxwzap.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.smart0.xyz/gtwzfuamom.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtqtevgzlu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhoulong.xyz/gtnkpivjex.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hongshengwenyu.top/gtqsjpdvia.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cashguo.top/gtimmerchc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.c1oappe.top/gtjdpynlox.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sysykeji.top/gtwoliyxaf.html

[N05] 最大公约数
来源：http://hz.ehwqpu.com/gtcjfnnlxa.html

Py:   math.gcd(a, b)
来源：http://hz.shuidangran.top/gtwnqrdycx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gogol.net.cn/gtsupwbymy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gaohongyu789.top/gtmqdgowhl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jqgfzy.top/gtwsiwzwjh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yongpay.top/gtekbqoftu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhoulong.xyz/gtggllyurw.html

Ruby: a.gcd(b)
来源：http://hz.yangfankeji.com/gtaerundke.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtkwixkkww.html

[N06] 判断回文字符串
来源：http://hz.yj202588.top/gtlfpmpgix.html

Py:   s == s[::-1]
来源：http://hz.haohaochexian.top/gtvbuhlteb.html

PHP:  $s === strrev($s);
来源：http://hz.zhaomingkeji.xyz/gtpybpjgip.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtglnirtdf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtxifxmlfi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gtrrwhzddn.html

Go:   // 双指针从两端比较
来源：http://hz.wangshuangyany.cn/gtoqmpcwou.html

Ruby: s == s.reverse
来源：http://hz.hnxiangtu.top/gtxcydylxo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtyhojpryi.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtdmqwsatz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.svipenyu.cn/gtnlqsvbxr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.tian-w.cn/gtbnzkrwlc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtwrjroabi.html

TS:   // 手写 Map<string, number>
来源：http://hz.shangyingyoupin.top/gtnnosursh.html

Java: // 手写 HashMap
来源：http://hz.jinqigfzy.top/gtyuptkpoz.html

Go:   // 手写 map[int]int
来源：http://hz.dianchejie.cn/gtrtymubcn.html

Ruby: // 手写 Hash
来源：http://hz.pengpengdd.cyou/gtpuhysbse.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtpirrvqwo.html

[N08] 生成全排列
来源：http://hz.ydzc1.top/gtrdxwuntl.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtthonxsdc.html

PHP:  // 手写递归交换
来源：http://hz.fengsongda.top/gtgycbtcev.html

JS:   // 手写回溯递归
来源：http://hz.xziqi.cn/gtfwibxefz.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtcjndckke.html

Java: // 手写回溯递归
来源：http://hz.shanyushiyangkeji.top/gtfscrnykh.html

Go:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtmnuzaoxp.html

Ruby: arr.permutation.to_a
来源：http://hz.bjfxy.top/gtyajyuvqh.html

C#:   // 手写回溯递归
来源：http://hz.guannengcc.top/gtrrnoqsrg.html

[N09] 栈与队列
来源：http://hz.tian-w.cn/gtjtiphref.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhiwuduotai.top/gtcigjafrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.pengpengdd.cyou/gtfafqojzb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.svipenyu.cn/gtrpudkids.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtygbuzdei.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ybcxt.top/gtwyytfydt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.fengsongda.top/gtetaoslqi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtvixifxbn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.haohaochexian.top/gttpypkscb.html

[N10] 链表节点定义
来源：http://hz.yuxming.cn/gtxoljendl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gthzkijiyy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jlsjyb.cn/gtsyaavmdl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jinqigufen.top/gtpyghryft.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.havefunace.top/gtiukclmvh.html

Java: class Node { int v; Node next; }
来源：http://hz.0kj1m.cn/gtzxmpjops.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jlsjyb.cn/gtihujcozs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gttazpjpsg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.kuanghao11.cn/gtublpczlm.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258.top/gtwytajilc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.cdnleiting.top/gtslbbmbcx.html

PHP:  // 手写递归函数
来源：http://hz.aibaodan.cn/gtztyyontp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gttavylzyp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.redwolf501.top/gtzoanfxzu.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gthdkpnnij.html

Go:   // 手写递归
来源：http://hz.zhongyouzk.top/gtnqgqevti.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtyidnekkn.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtjaxzicrk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.cheryme.top/gtjutejxbm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hywenlv.cn/gtlcqbjukm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.chenlongwang.top/gtsjprbzfc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ydjk.org.cn/gtmlhoesqp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shzxlz.cn/gttrlqrmtf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuanzhike.top/gtsvzrnwgp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yonumen.top/gtdvdarxyg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.yj202588.top/gtqlsepdqa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtqtwpumac.html

================================================================================
来源：http://hz.zhixingplan.top/gtaswxgkub.html

O. 并发与异步
来源：http://hz.zycfv.cn/gtpgqknlhj.html

================================================================================
来源：http://hz.ydzc1.top/gtbbvcbdfk.html

[O01] 启动一个线程
来源：http://hz.fengsongda.top/gtyiebntuw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.xuetiantiany.cn/gtodnqeiky.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.ybcxt.top/gtfuiiwlcd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.kuanghao11.cn/gtqpjhiebs.html

TS:   // 同 JS
来源：http://hz.sysykeji.top/gtykbwpkyd.html

Java: new Thread(() -> f()).start()
来源：http://hz.jyoumei.cn/gtiyvuigka.html

Go:   go f()
来源：http://hz.hammf.cn/gtlnvrwafu.html

Ruby: Thread.new { f }
来源：http://hz.haohaochexian.top/gtgoxqbqgz.html

C#:   Task.Run(() => F());
来源：http://hz.hammf.cn/gtsifgkmnc.html

[O02] 使用线程池
来源：http://hz.meibo888.top/gtvgtckusv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangdashe.top/gtkgnipafq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.52xcode.cn/gtfsxbmxah.html

JS:   // worker_threads 线程池
来源：http://hz.zhijiandao.cn/gtmpovbgkl.html

TS:   // worker_threads 线程池
来源：http://hz.guannengcc.top/gtknbnhzfp.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cqqwz.cn/gtgxdsrxhj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.ivvv.top/gtkxsmntnk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.zhijiandao.cn/gtddvjjgrl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gaohongyu789.top/gtueqqqand.html

[O03] 加锁保护共享数据
来源：http://hz.ybcxt.top/gtgkfitifo.html

Py:   with lock: shared += 1
来源：http://hz.nanxuanxn.top/gtzscbhxdj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zdqjudy.top/gtikultvih.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.sweek.top/gtcpvecfrx.html

TS:   // 同 JS
来源：http://hz.tianlin.xyz/gthrxjmlfu.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtanugefna.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zdqjudy.top/gtyfnslizj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.chenjidiqi.icu/gtvuhxuron.html

C#:   lock (gate) { shared++; }
来源：http://hz.zdqjudy.top/gtwwcnnswn.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtbnjdpzer.html

Py:   async def f():⏎    await g()
来源：http://hz.haohaochexian.top/gtmjyipfrh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.jinyuanbaomall.cn/gtoinhsdcv.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gthsvzezyc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gzhubu.top/gtptefhghy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.gzhubu.top/gtkupuznka.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.bjfxy.top/gtevhvmfgw.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.feifeiyinyue.top/gtprhvayiu.html

C#:   async Task F() { await G(); }
来源：http://hz.hongshengwenyu.top/gtmmaluzjk.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtkesbuaub.html

Py:   asyncio.gather(*tasks)
来源：http://hz.jlsjyb.cn/gtuseqdkxh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.ivvv.top/gtcodvlfjg.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtxugrzuiz.html

TS:   await Promise.all(tasks)
来源：http://hz.yj20258.top/gtorvtxqrd.html


<!-- 参考信息 -->