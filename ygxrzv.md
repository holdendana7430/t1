代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zdqjudy.top/gtvcrkujme.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtmvmfqoxb.html

TS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtxnzuezsb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtutuiozlx.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtqxubxrjg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hysaishi.cn/gtcsfywhho.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tanke756.top/gtoduwkgcy.html

[L02] 发送 POST JSON
来源：http://hz.hywenlv.cn/gtmwkgjqpg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtnuemspmz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtylzvfbem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtxvbolxrc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gthccnjwnv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtcabzvorz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtrztiarxb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtddcpjmua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtepyuyxed.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gttwvaigcj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtgflrpngj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxuanxn.top/gtxrryhwgy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gthdymrbmu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hywenlv.cn/gtdkkdrxbu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daxiang520.top/gtvfkzjhpb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtjnpgzvxs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dashuyun.cn/gtpoamxgop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sysykeji.top/gtbculpwps.html

[L04] 设置超时
来源：http://hz.aibaodan.cn/gtlrzsorkq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jinqigfzy.top/gtudimjzlh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gtbsumeuvk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtgcmbcikn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtgpdiwdlv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtvyphtqhx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtgqcutnkb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtpguxzqeo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aibaodan.cn/gtmhxnkupp.html

[L05] 上传文件（multipart）
来源：http://hz.52xcode.cn/gtyoxfbbqj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtcpcdphdr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.tian-w.cn/gtnykbyovx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtczgyvvpj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtvmvnrtas.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtfbytiuzd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yonumen.top/gtmcetsfcr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.nwbrower.top/gtscvztwwy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gttbludmcg.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtjlhicpre.html

Py:   resp.json()
来源：http://hz.smart0.xyz/gtzwqloduf.html

PHP:  json_decode($body, true);
来源：http://hz.shanyushiyangtech.top/gtkugdrtur.html

JS:   await resp.json()
来源：http://hz.wangdashe.top/gthkzmeija.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtxwfajnjh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gttuiurhfp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zycfv.cn/gtuwoixcdr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ywan-chungtsiang.top/gtkyixekgy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtnjhpluff.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtlqcactne.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hysaishi.cn/gttyliskgi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtmsxybywe.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtfykeuobd.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtiyvlczsc.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtoykqkliz.html

Go:   resp.StatusCode
来源：http://hz.yangfankeji.com/gtdlbxcwpr.html

Ruby: resp.code.to_i
来源：http://hz.hnxiangtu.top/gtusqjhzix.html

C#:   (int)resp.StatusCode
来源：http://hz.vqdsnc.cn/gtvkycadsg.html

[L08] 并发请求多个地址
来源：http://hz.jyoumei.cn/gttujwjoqh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zhijiandao.cn/gtsaxucvxd.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtqxhwsfla.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtdwrsxzcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtmunwcxok.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtwiqrwzdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtlvgdvisr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtpxcedsfb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtsvfiulki.html

================================================================================
来源：http://hz.haohaochexian.top/gtzofqvnoj.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtfzruupal.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkmvbxubd.html

[M01] 读取命令行参数
来源：http://hz.redwolf501.top/gtvhfqcxaj.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtsulzfeco.html

PHP:  $argv;  $argc;
来源：http://hz.zhijiandao.cn/gtlwrahjxo.html

JS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtuvnywivm.html

TS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gtftmzhyxc.html

Java: args 数组（main 方法参数）
来源：http://hz.ydjk.org.cn/gtofdnivfy.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtmdddbptu.html

Ruby: ARGV
来源：http://hz.zdqjudy.top/gtmpgbucak.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yonumen.top/gteojrnucx.html

[M02] 读取环境变量
来源：http://hz.aizwys.cn/gtzvjiexgf.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gtscefzqpu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tian-w.cn/gtvshmjqgs.html

JS:   process.env.HOME
来源：http://hz.cdnleiting.top/gtscueqckq.html

TS:   process.env.HOME
来源：http://hz.tian-w.cn/gtluzstngj.html

Java: System.getenv("HOME")
来源：http://hz.tianlin.xyz/gtnsdudonx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nwbrower.top/gtfxgdqdke.html

Ruby: ENV["HOME"]
来源：http://hz.cheryme.top/gtzhznmsmg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtirrsntwu.html

[M03] 执行外部命令
来源：http://hz.jyoumei.cn/gtypilxwcr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhiwuduotai.top/gtczyaqnao.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtenbqlthm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtkmqesktt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtcteythmi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.pengpengdd.cyou/gtulvilyyy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtxlknnklb.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.aizwys.cn/gtuhcyxmpe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.svipenyu.cn/gthycbahsv.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtluwmpple.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtdjppyyrx.html

PHP:  getcwd();
来源：http://hz.fzhhl.top/gtlrkpgirk.html

JS:   process.cwd()
来源：http://hz.chenlongwang.top/gtvhrrjlua.html

TS:   process.cwd()
来源：http://hz.hnqzz.top/gtztxgjplp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhaomingkeji.xyz/gtbvusxgev.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtniiyheld.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtvliaoals.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtyozodcgn.html

[M05] 设置退出码
来源：http://hz.tanke756.top/gtqaksaabm.html

Py:   sys.exit(1)
来源：http://hz.ivvv.top/gtgzvgjtuu.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtqprrvnln.html

JS:   process.exit(1)
来源：http://hz.yj20258.top/gtslizdcse.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtwggbyuha.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtjiiyqiph.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtmqcaisej.html

Ruby: exit 1
来源：http://hz.cashguo.top/gtpjpfwwxj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cashguo.top/gtmrgtfdru.html

[M06] 向标准错误输出
来源：http://hz.jyoumei.cn/gtzragntlo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jqgfzy.top/gtuzvccgvy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shangyingyoupin.top/gtemmljgvh.html

JS:   console.error("err")
来源：http://hz.dashuyun.cn/gtmxbdlhjn.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gteekdkswp.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtweuokuum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gttcsmaipn.html

Ruby: warn "err"
来源：http://hz.zhixingplan.top/gtfqbhhysx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gteiuzwaxy.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtrlpbgequ.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258888.top/gtkyjlgxzv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtfpfdmwve.html

JS:   require.main === module
来源：http://hz.zdqjudy.top/gtdrkthiin.html

TS:   require.main === module
来源：http://hz.andypj.xyz/gtxhhcbjgb.html

Java: public static void main(String[] args)
来源：http://hz.ivvv.top/gtycedpstf.html

Go:   func main()
来源：http://hz.daxiang520.top/gtaokwkpgy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jlsjyb.cn/gtethhaveo.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gthjevdyie.html

[M08] 获取系统与运行时信息
来源：http://hz.havefunace.top/gtknhcgwfa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtwvdkauec.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxuanxn.top/gtiuxgtepw.html

JS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtgwdezswx.html

TS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtxlfudrmb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtzhaouoxw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hnxiangtu.top/gtblknmzrm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtwmapayad.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.haohaochexian.top/gtrratvbgp.html

================================================================================
来源：http://hz.yanxiufei.cn/gtjpiyooko.html

N. 数据结构与算法
来源：http://hz.bjfxy.top/gtmgmgeltj.html

================================================================================
来源：http://hz.zhijiandao.cn/gtskjjjnxp.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtzkxalhji.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hysaishi.cn/gtwfyokfdi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtudwxyqni.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtvleqjmrl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtrdxenwkk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yueranfly.top/gtrhlvgtxu.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zdqjudy.top/gtdfeskulu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gtwshkngan.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtnvhsytxe.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtskcccgpp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtxcloatnb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yuanzhike.top/gtpaxzeubm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtzqpilnqx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xingfuxueyuan.xyz/gtawcgiwej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhixingplan.top/gtcveemthc.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gtovqeqeaa.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtkumseyxx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jyoumei.cn/gtbzyyogln.html

[N03] 快速排序（分治示例）
来源：http://hz.chenjidiqi.icu/gtbxnspknk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jiagoushi.top/gttxcmepqa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.kuanghao11.cn/gtuxxsipgg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhiwuduotai.top/gtnovhcvtw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gtzkuddmap.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhixingplan.top/gtftdinwei.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.smart0.xyz/gtyvpawbtk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gtjvgzvddy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tanke756.top/gtyyetndrv.html

[N04] 斐波那契数列
来源：http://hz.guannengcc.top/gtgojmatyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtyjozctyo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.guannengcc.top/gtuxhewstr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guowangkeji.top/gtywtynydl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtpvficfyd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.c1oappe.top/gtrfbkkzbc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtkeaseyha.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cucudq.cn/gtwesbnpqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xuetiantiany.cn/gttwwllbph.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtwclqzelo.html

Py:   math.gcd(a, b)
来源：http://hz.tian-w.cn/gtursnebqb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtxeoopdwz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtuapmkhqn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.meibo888.top/gtaugxrfqb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtuaurclnq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtnoxhxvcn.html

Ruby: a.gcd(b)
来源：http://hz.mhx1999.top/gtfntaxzup.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jyoumei.cn/gtkuoyylli.html

[N06] 判断回文字符串
来源：http://hz.hnxiangtu.top/gttmyihrky.html

Py:   s == s[::-1]
来源：http://hz.wangdashe.top/gtwlmiggjf.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtcctpchyu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtosalnkkv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtguetnslh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.bjfxy.top/gtkjssjucy.html

Go:   // 双指针从两端比较
来源：http://hz.chenzaomai.com/gtdktbpvte.html

Ruby: s == s.reverse
来源：http://hz.hysaishi.cn/gtyssjnqkh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtvjqinxsz.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtgbirvgrh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtycaecxpa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.birdmap.top/gtcfqptcvx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yonumen.top/gtqsuylyar.html

TS:   // 手写 Map<string, number>
来源：http://hz.yonumen.top/gtoztizjje.html

Java: // 手写 HashMap
来源：http://hz.yj20258888.top/gtwykdsxeq.html

Go:   // 手写 map[int]int
来源：http://hz.hfpthk.cn/gtnrwyxmgh.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtpmswglka.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sufxvd.cn/gtyqixphyl.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtyfsmqwil.html

Py:   itertools.permutations(arr)
来源：http://hz.shangyingyoupin.top/gtjcpmnaer.html

PHP:  // 手写递归交换
来源：http://hz.hysaishi.cn/gtqqkzdogf.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtswqcedsh.html

TS:   // 手写回溯递归
来源：http://hz.ivvv.top/gtchiytsfy.html

Java: // 手写回溯递归
来源：http://hz.sufxvd.cn/gtnbvtzatt.html

Go:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gteoruvacl.html

Ruby: arr.permutation.to_a
来源：http://hz.zhijiandao.cn/gtmaloxjop.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtubgadzws.html

[N09] 栈与队列
来源：http://hz.pycfn.com/gtiuhvjcym.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtoqjzpgsd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.haohaochexian.top/gtmkfnclck.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.kuanghao11.cn/gtprkuwbzl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.gaohongyu789.top/gtteicuvsi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.pengpengdd.cyou/gtlimqwtnr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtrsosuxmm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.nwbrower.top/gtizvvhcny.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinqigfzy.top/gticxfzcmg.html

[N10] 链表节点定义
来源：http://hz.jqgfzy.top/gtvshqsfnl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jinyuanbaomall.cn/gtozwhjccc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.ywan-chungtsiang.top/gtlenrkjao.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.0kj1m.cn/gtlultglej.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hnqzz.top/gttijrghqi.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtpmbfjdzi.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gzhubu.top/gtrzlvjiwc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sxryk.cn/gtmmkkmjxh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.bjfxy.top/gtazyvdabb.html

[N11] 二叉树中序遍历
来源：http://hz.zhijiandao.cn/gtimieaija.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.zycfv.cn/gtpqnrmivv.html

PHP:  // 手写递归函数
来源：http://hz.yj20258888.top/gtnlpfyaup.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yvedp.cn/gtwaawducc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtzlcwcjmj.html

Java: // 手写递归
来源：http://hz.gogol.net.cn/gtajfavrro.html

Go:   // 手写递归
来源：http://hz.hywenlv.cn/gtiiesuhrp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.svipenyu.cn/gtvrdxmoey.html

C#:   // 手写递归
来源：http://hz.yj20258888.top/gtwjmzlsxs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.shangyingyoupin.top/gtrvgaapqu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.jyoumei.cn/gtheweisnr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.kuanghao11.cn/gtxjkkmzyq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cdnleiting.top/gtmajlrcdn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhengqikj.top/gthuvhonaj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhiwuduotai.top/gthapwhzwc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.quarkkingdee.top/gtnmgaxhdz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hnqzz.top/gtcbhxzksb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sxryk.cn/gtsnzdkhlf.html

================================================================================
来源：http://hz.yuanzhike.top/gtzvutohhn.html

O. 并发与异步
来源：http://hz.shangyingyoupin.top/gtbvhnqycz.html

================================================================================
来源：http://hz.vqdsnc.cn/gtufbktfop.html

[O01] 启动一个线程
来源：http://hz.fzhhl.top/gtcgshkjlb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.aizwys.cn/gtyatxyhtg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yonumen.top/gtldzfpzzu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.jiagoushi.top/gtgxbcblng.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtqtcctdqe.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gthdohspik.html

Go:   go f()
来源：http://hz.vqdsnc.cn/gtuopbqvyu.html

Ruby: Thread.new { f }
来源：http://hz.pycfn.com/gtnkmnsyre.html

C#:   Task.Run(() => F());
来源：http://hz.shangyingyoupin.top/gthnoccegj.html

[O02] 使用线程池
来源：http://hz.hongshengwenyu.top/gtcnefxwzn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gtmszydocj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.gzhubu.top/gtphihgwkg.html

JS:   // worker_threads 线程池
来源：http://hz.daxiang520.top/gtbwocsqpv.html

TS:   // worker_threads 线程池
来源：http://hz.jinqigfzy.top/gtnnnqwbrh.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtcwszksqv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xziqi.cn/gtvmrulesd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.chenlongwang.top/gtnxkcbcwa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jiagoushi.top/gtnbtssobs.html

[O03] 加锁保护共享数据
来源：http://hz.havefunace.top/gtweyovucx.html

Py:   with lock: shared += 1
来源：http://hz.hysaishi.cn/gtyvnlhhwf.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhoulong.xyz/gtngxnoyvl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.nanxuanxn.top/gtydelfclk.html

TS:   // 同 JS
来源：http://hz.shuidangran.top/gtnxjpzshv.html

Java: synchronized (this) { shared++; }
来源：http://hz.yuanzhike.top/gticfsowkx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.xziqi.cn/gtovfqwnad.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.xingfuxueyuan.xyz/gtthuhahwm.html

C#:   lock (gate) { shared++; }
来源：http://hz.iojbl.cn/gtqoonbseh.html

[O04] 定义异步函数并等待
来源：http://hz.haohaochexian.top/gttpeinrzd.html

Py:   async def f():⏎    await g()
来源：http://hz.gotoacloud.top/gtnxrmcggj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.iojbl.cn/gtcddglpoy.html

JS:   async function f() { await g(); }
来源：http://hz.jqgufenzy.top/gtbjqrnvbi.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.pengpengdd.cyou/gtpoiyphyb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shzxlz.cn/gtexojrrif.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtzcmkknmh.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.shuidangran.top/gtxdcmiruh.html

C#:   async Task F() { await G(); }
来源：http://hz.andypj.xyz/gtjdxizihc.html

[O05] 并发执行并等待全部完成
来源：http://hz.gzhubu.top/gtzayzkmgz.html

Py:   asyncio.gather(*tasks)
来源：http://hz.meibo888.top/gtvthdgoql.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.chenzaomai.com/gtvdvybcos.html

JS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtymxyveal.html

TS:   await Promise.all(tasks)
来源：http://hz.zhengqikj.top/gtenbraplz.html


<!-- 参考信息 -->