代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtbmludeds.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtylrbwety.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtdncikhyo.html

[L02] 发送 POST JSON
来源：http://hz.ivvv.top/gtdlezodnq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtzviednah.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gtuemueplg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtpvivbbzc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhaomingkeji.xyz/gtqeznnlwu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yonumen.top/gtfcuiisym.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.bjfxy.top/gtfdrbfvij.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ehwqpu.com/gtpwwaeyww.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtqhyhspqe.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtznjykrzw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.iojbl.cn/gtoyvvkzic.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtlxwfxaxy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtqdjczsya.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnxiangtu.top/gtxwgfgafb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtmywktlyw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtmfpbscig.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtihpnqdnh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gteabsrypv.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtkhydslem.html

Py:   requests.get(url, timeout=5)
来源：http://hz.aizwys.cn/gtxuemmppa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtmhjegiee.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtrtupahos.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daxiang520.top/gtcyqvmuon.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtwbasliof.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtzlquvklm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gotoacloud.top/gtnjdfrtac.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cdnleiting.top/gtdhtbsqcs.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtedzunvmc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtlqvhspij.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtaostucqv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtdvvhpmsa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtaqljqhll.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.dianchejie.cn/gtcwexayyy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.meibo888.top/gtewlbuliq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnqzz.top/gtclpowlhp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtbvajvrdo.html

[L06] 解析响应为 JSON
来源：http://hz.sxryk.cn/gtwsxmbknc.html

Py:   resp.json()
来源：http://hz.guowangkeji.top/gttmonlcst.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gtuzznkotb.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtkjcyauem.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtayfyvawp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtuqzuzclb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sweek.top/gtlvambblh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtcebztsvt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydzc1.top/gtubzgtneo.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtrkduwdho.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xinyue.icu/gtwbapcxtl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xingfuxueyuan.xyz/gtknsirgnt.html

JS:   resp.ok;  resp.status
来源：http://hz.andypj.xyz/gtnikrsayd.html

TS:   resp.ok;  resp.status
来源：http://hz.jianghu66.top/gttjseflsh.html

Java: resp.statusCode()
来源：http://hz.vqdsnc.cn/gtppokywna.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gtcbqgtxyw.html

Ruby: resp.code.to_i
来源：http://hz.yj20258888.top/gtjbjqyfxa.html

C#:   (int)resp.StatusCode
来源：http://hz.ivvv.top/gtyxskkrtb.html

[L08] 并发请求多个地址
来源：http://hz.hysaishi.cn/gtzjzgnkke.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtouzhdjhm.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuxming.cn/gtnmxlkidv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtkaotvmli.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtsyegxvja.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtdkmxaeas.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtizunhdsb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgfzy.top/gtzejlvxsj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ywan-chungtsiang.top/gtucrrfyfl.html

================================================================================
来源：http://hz.fengsongda.top/gtnjwirwcc.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtzazuxdav.html

================================================================================
来源：http://hz.jinqigufen.top/gtuttufdjg.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtlnaaddia.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gttwbwqnlg.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtheawkhpl.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258888.top/gtelagzvlq.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtxfhysjsq.html

Java: args 数组（main 方法参数）
来源：http://hz.xinyue.icu/gtzbpetdog.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gteetbzvjw.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtddbagodt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtceeyeqac.html

[M02] 读取环境变量
来源：http://hz.jyoumei.cn/gtmsipduwp.html

Py:   os.environ.get("HOME")
来源：http://hz.hnxiangtu.top/gtarbinjyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sysykeji.top/gtpyfsmkqx.html

JS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtlxxuzmne.html

TS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtwoqshovv.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtrhjijdgn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxuanxn.top/gtfyzrvhnc.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtryzxrpta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtorgslqrk.html

[M03] 执行外部命令
来源：http://hz.cashguo.top/gtbojdhitw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtzqbupgmp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtnbgvhdnq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gttbkxssjy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtwkekdrwy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aibaodan.cn/gtyopqehfr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtsnwjxotj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.52xcode.cn/gtbayjstcg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shzxlz.cn/gtwdoewinb.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtkxwuitza.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtqmcmjyzi.html

PHP:  getcwd();
来源：http://hz.yangfankeji.com/gtrcetnzsv.html

JS:   process.cwd()
来源：http://hz.shuidangran.top/gtfdohfqoe.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtqgtkqmlc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxinkj.top/gtwnitgsun.html

Go:   os.Getwd()
来源：http://hz.xziqi.cn/gtiqlcwdem.html

Ruby: Dir.pwd
来源：http://hz.redwolf501.top/gtpzenbros.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtuleyxsfb.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtwletsvcb.html

Py:   sys.exit(1)
来源：http://hz.zycfv.cn/gtttkgzpca.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtmjelydrx.html

JS:   process.exit(1)
来源：http://hz.fengsongda.top/gttstbdayu.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtsribzaex.html

Java: System.exit(1)
来源：http://hz.c1oappe.top/gtzyrweuzh.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtzsqyvdje.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtewzfhspf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zycfv.cn/gthvligjco.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gtkgdionkp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtftqqsarp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtozzhumpz.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtcnnxgxqx.html

TS:   console.error("err")
来源：http://hz.fzhhl.top/gtkyihkkii.html

Java: System.err.println("err")
来源：http://hz.316326.xyz/gtkunbmlhs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtbjwkhkkw.html

Ruby: warn "err"
来源：http://hz.fzhhl.top/gtinmfiibb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenlongwang.top/gtnwgermch.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gthlstjlgp.html

Py:   if __name__ == "__main__":
来源：http://hz.redwolf501.top/gtyfbnhbej.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.gotoacloud.top/gtxhcduouv.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtbkvrntng.html

TS:   require.main === module
来源：http://hz.bjfxy.top/gtfkfsfhuz.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gticgkjzbt.html

Go:   func main()
来源：http://hz.iojbl.cn/gtvblmuyfn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtlrdkizap.html

C#:   static void Main(string[] args)
来源：http://hz.tanke756.top/gtdldoqnwe.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtqphnngsj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.dianchejie.cn/gtgpoydxrj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shzxlz.cn/gtzkfvakat.html

JS:   process.platform;  process.version
来源：http://hz.316326.xyz/gtebpnzkkg.html

TS:   process.platform;  process.version
来源：http://hz.zhengqikj.top/gtybrcavgf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.c1oappe.top/gtweqlspem.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtqlyukgod.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gtxazdabqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.havefunace.top/gtddajqjzy.html

================================================================================
来源：http://hz.zhongyouzk.top/gtuzpslhxn.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtwzgilmzu.html

================================================================================
来源：http://hz.jiagoushi.top/gthjndfdmq.html

[N01] 二分查找（有序数组）
来源：http://hz.xylfe.cn/gtkivvgyyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhiwuduotai.top/gtlvyqwsvt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.wangdashe.top/gticfmzrws.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gtjuicvawp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gthbrxbzrx.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtyijsvtka.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gzhubu.top/gtxgfyhdrb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.feifeiyinyue.top/gtappvtbah.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yonumen.top/gtknbjkntv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.pengpengdd.cyou/gtddczorsb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtjkfbldig.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.52xcode.cn/gtblfohhpt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.andypj.xyz/gtidenxnsz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sxryk.cn/gtkavulogb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.havefunace.top/gtpozurqqh.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gtsyjxlink.html

Ruby: arr.sort
来源：http://hz.havefunace.top/gtkrhltddo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtcescfhrf.html

[N03] 快速排序（分治示例）
来源：http://hz.yvedp.cn/gtahloupll.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.meibo888.top/gtkebmwguf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gthjgdijbw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yvedp.cn/gthkazrdbv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ivvv.top/gtzlehylso.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.dashuyun.cn/gtprlukxpn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shangyingyoupin.top/gtgetsarzo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.chenjidiqi.icu/gtizleswne.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.pycfn.com/gtfolitblg.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gttrsffrvv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtkchzmwcq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ydzc1.top/gtuzeqtgur.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtlmmuhiwe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.c1oappe.top/gteqmgyykl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtvjjqptpd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xylfe.cn/gtntnkiutr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtjtwbjjjx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtwjlimvdw.html

[N05] 最大公约数
来源：http://hz.jianghu66.top/gtuxyrhopr.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtjjjlzoyc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shangyingyoupin.top/gtjsoywvrw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gturzwwxip.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shzxlz.cn/gtzkrmxcan.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258888.top/gtokucqdeo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.316326.xyz/gtsxfccztj.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtvgcvodkx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hysaishi.cn/gtuwcmlhjq.html

[N06] 判断回文字符串
来源：http://hz.chenlongwang.top/gthlihwtwo.html

Py:   s == s[::-1]
来源：http://hz.yueranfly.top/gtmysvcpmo.html

PHP:  $s === strrev($s);
来源：http://hz.jinyuanbaomall.cn/gtjwzjbthw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtzeycgujn.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtojjhfgyu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shanyushiyangtech.top/gtermtyawa.html

Go:   // 双指针从两端比较
来源：http://hz.hammf.cn/gtjpreoukz.html

Ruby: s == s.reverse
来源：http://hz.dashuyun.cn/gtwjgearni.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtzzvbndwo.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtqjssxmwu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtxhbhuxod.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.redwolf501.top/gtvoiaxxpj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shanyushiyangtech.top/gtbsfzvtod.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtjnncwlnk.html

Java: // 手写 HashMap
来源：http://hz.ywan-chungtsiang.top/gtcacmwttp.html

Go:   // 手写 map[int]int
来源：http://hz.jqgfzy.top/gtqozqoclw.html

Ruby: // 手写 Hash
来源：http://hz.sysykeji.top/gtfjyqvdxf.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yonumen.top/gtpnuexlby.html

[N08] 生成全排列
来源：http://hz.guowangkeji.top/gtcxqcrewa.html

Py:   itertools.permutations(arr)
来源：http://hz.snrcjt.cn/gtgltnrqwt.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtkfiynlqr.html

JS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtejedmphr.html

TS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtntxsrpwu.html

Java: // 手写回溯递归
来源：http://hz.gotoacloud.top/gtwqwdmqor.html

Go:   // 手写回溯递归
来源：http://hz.pycfn.com/gtxlzjfjxp.html

Ruby: arr.permutation.to_a
来源：http://hz.jiagoushi.top/gtstepzbhu.html

C#:   // 手写回溯递归
来源：http://hz.daria6918.cn/gtzjghhntg.html

[N09] 栈与队列
来源：http://hz.sufxvd.cn/gtxxdneudn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.fzhhl.top/gtyacuskgn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.xuetiantiany.cn/gtngjrgyuv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhixingplan.top/gtfkmqpaky.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cdnleiting.top/gtuwjckbad.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gttgzouydl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.sufxvd.cn/gtimcofcrh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yuanzhike.top/gtejydmpqx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yj20258888.top/gtilfgsfim.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtmrmqnonx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangkeji.top/gtkmvfuvar.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.svipenyu.cn/gtmfujjegu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cheryme.top/gtszydmqqa.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jqgfzy.top/gtgowsgmhs.html

Java: class Node { int v; Node next; }
来源：http://hz.dianchejie.cn/gttyuvlief.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.c1oappe.top/gtaztvsgza.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhijiandao.cn/gttjxdlmrf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.svipenyu.cn/gtllnxawbb.html

[N11] 二叉树中序遍历
来源：http://hz.jinyuanbaomall.cn/gtixsbrikl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.gotoacloud.top/gtxsoyecio.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtwrwplxgk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtasudxbny.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hongshengwenyu.top/gtnspzttxb.html

Java: // 手写递归
来源：http://hz.cqqwz.cn/gtzroompsw.html

Go:   // 手写递归
来源：http://hz.xinyue.icu/gtzjbukwnc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.chenzaomai.com/gteexpvnzf.html

C#:   // 手写递归
来源：http://hz.fzhhl.top/gtgfzukrgj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhiwuduotai.top/gtpxdebtlr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.shanyushiyangkeji.top/gtppidtyae.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yuanzhike.top/gtjnwnskjx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ppjwa.cn/gtdwhfmbko.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.cashguo.top/gtcyblszvy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtpjgrwajr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtgftxzrqn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.cqqwz.cn/gtwjpdontp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.havefunace.top/gtwumbzmoo.html

================================================================================
来源：http://hz.hnqzz.top/gttwdfthpy.html

O. 并发与异步
来源：http://hz.wangshuangyany.cn/gtzwqtuqyi.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxuxeyreg.html

[O01] 启动一个线程
来源：http://hz.yongpay.top/gtwglrmxwc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.hammf.cn/gtdkghgxfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.fzhhl.top/gtlktmnqzr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.9152youxi.cn/gthnnhmkol.html

TS:   // 同 JS
来源：http://hz.fzhhl.top/gtulkbgcor.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gttojkvqzi.html

Go:   go f()
来源：http://hz.shzxlz.cn/gtkffbgccw.html

Ruby: Thread.new { f }
来源：http://hz.wangdashe.top/gtwhmqwkha.html

C#:   Task.Run(() => F());
来源：http://hz.smart0.xyz/gtwnjqjwye.html

[O02] 使用线程池
来源：http://hz.jqgufenzy.top/gtektypdxl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jyoumei.cn/gttnbzadin.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ydzc1.top/gtesbggcof.html

JS:   // worker_threads 线程池
来源：http://hz.jqgufenzy.top/gtylybzzvp.html

TS:   // worker_threads 线程池
来源：http://hz.nwbrower.top/gtngblgesn.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.cucudq.cn/gtfowfwpsu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yanxiufei.cn/gtukoghpbj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.cucudq.cn/gtqrjhtvxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.chenjidiqi.icu/gtdpcqzdhn.html

[O03] 加锁保护共享数据
来源：http://hz.0kj1m.cn/gtvmsyatuj.html

Py:   with lock: shared += 1
来源：http://hz.316326.xyz/gtjrjuygjj.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sysykeji.top/gtciqlwazy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.jiagoushi.top/gtsnfuwhdc.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtnlxyrwdg.html

Java: synchronized (this) { shared++; }
来源：http://hz.hysaishi.cn/gtyqftlygf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtbmaftmla.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.jqgfzy.top/gtgjrkzuwt.html

C#:   lock (gate) { shared++; }
来源：http://hz.hongshengwenyu.top/gtixgqquwb.html

[O04] 定义异步函数并等待
来源：http://hz.0kj1m.cn/gtutbbueby.html

Py:   async def f():⏎    await g()
来源：http://hz.jinghuilouyu.cn/gtnplrmsgg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.dashuyun.cn/gtezxpdvym.html

JS:   async function f() { await g(); }
来源：http://hz.sysykeji.top/gtundoange.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.sufxvd.cn/gtlcnnufsy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.iojbl.cn/gtnjxysnrl.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.fzhhl.top/gtdqkuepfg.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.fzhhl.top/gtvmirmvtg.html

C#:   async Task F() { await G(); }
来源：http://hz.zhaomingkeji.xyz/gtuqjjrabi.html

[O05] 并发执行并等待全部完成
来源：http://hz.zhaomingkeji.xyz/gtokeugvpp.html

Py:   asyncio.gather(*tasks)
来源：http://hz.ivvv.top/gtdpyeanqw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gticxrdujz.html

JS:   await Promise.all(tasks)
来源：http://hz.jianghu66.top/gtnkamtigj.html

TS:   await Promise.all(tasks)
来源：http://hz.meibo888.top/gtbpaiyyjo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.316326.xyz/gteyjtopxo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.yj202588.top/gtncmkigfj.html

Ruby: threads.map(&:join)
来源：http://hz.gotoacloud.top/gtvxzzmvhf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.shanyushiyangkeji.top/gtezuvcevp.html


<!-- 参考信息 -->