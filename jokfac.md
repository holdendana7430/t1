代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtzreyitud.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hfpthk.cn/gtjbzfilri.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtldfmmfwy.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gttzuwbmkg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gogol.net.cn/gtatqwgpmg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtcsequcuf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtdnwdozrn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gtwqqsiyvn.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtahxlowlp.html

Ruby: Marshal.dump(obj)
来源：http://hz.cqqwz.cn/gtpradhafk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtzyxikyjq.html

================================================================================
来源：http://hz.aibaodan.cn/gtvsaorrgj.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtcairlppu.html

================================================================================
来源：http://hz.cucudq.cn/gtonjponhu.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtxmztwdbq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ehwqpu.com/gtbblsfqmz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtdmhdwlff.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gttcorkgyy.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtnfgugqza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtdrsdszdj.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtxbpkwfzd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtulqgpbgc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtgredycti.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtnniczulo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtwqrxgqoc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gttliglcbr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.0kj1m.cn/gtuutyixuu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtqsqxdepd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuetiantiany.cn/gtcyuayafg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtaqwyfxes.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shangyingyoupin.top/gtpqprleyg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtovkdwzun.html

[L03] 设置自定义请求头
来源：http://hz.xylfe.cn/gtlubyzgve.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtrsobhlhg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtjhpiylzx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.svipenyu.cn/gtmcsxtmyb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtiprjxfsj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shangyingyoupin.top/gtnfgpibbz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtekajdlwo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aibaodan.cn/gtsgwvwaap.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.quarkkingdee.top/gtotlofxgu.html

[L04] 设置超时
来源：http://hz.xingfuxueyuan.xyz/gtdjplaknq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtstkoakxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinghuilouyu.cn/gtvamyeggu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yueranfly.top/gtllmphtgc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtfnercsvs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gtoynqycxb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangdashe.top/gtplypltzo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtkyijptxz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.iojbl.cn/gtvqzyoiuh.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtguxialmg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sysykeji.top/gtmdcujqli.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtknczclno.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtpuokekmg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtmsgyxyvj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtdodcchrp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtjusmawmt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jqgufenzy.top/gtfkiixxoh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtkxwrtajy.html

[L06] 解析响应为 JSON
来源：http://hz.tianlin.xyz/gtfwiuytgh.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtufuamwzs.html

PHP:  json_decode($body, true);
来源：http://hz.gzhubu.top/gtqtnohxag.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtqslkurwk.html

TS:   await resp.json()
来源：http://hz.xuanzx.com/gtwzakmurs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtsklqrkhu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtdorjhqcy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtccygzjjm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.52xcode.cn/gtydgaiuan.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtapauuuls.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtqalgnktv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtepfrndzv.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtdricrlqf.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gthvszejjl.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtuzjyigzz.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtxjhblavm.html

Ruby: resp.code.to_i
来源：http://hz.ywan-chungtsiang.top/gtgflsjfji.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtifjlrgne.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtrovnigce.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtcvqbrjzb.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtggsyvciu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtvwvhywgc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtahwpoyft.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgfzy.top/gtvytehxag.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhixingplan.top/gtojqwbapm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtzrhqldok.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtkrtedoov.html

================================================================================
来源：http://hz.yj20258888.top/gtvybmdcxe.html

M. 命令行 / 进程 / 环境
来源：http://hz.redwolf501.top/gtnsftlmgy.html

================================================================================
来源：http://hz.yonumen.top/gtjflphfzy.html

[M01] 读取命令行参数
来源：http://hz.birdmap.top/gtmccihjiw.html

Py:   sys.argv[1:]
来源：http://hz.cqqwz.cn/gtkyrfvcoo.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gtlvzaulwx.html

JS:   process.argv.slice(2)
来源：http://hz.xuetiantiany.cn/gtkazaohkn.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtshwgnmqm.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtkjknnuyd.html

Go:   os.Args[1:]
来源：http://hz.ydjk.org.cn/gtsgtjyepv.html

Ruby: ARGV
来源：http://hz.kuanghao11.cn/gtplrutvrq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnqzz.top/gtwfnlhzqv.html

[M02] 读取环境变量
来源：http://hz.ydzc1.top/gtjlbzixoj.html

Py:   os.environ.get("HOME")
来源：http://hz.gaohongyu789.top/gtrauozetp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guannengcc.top/gtrgwpxpvy.html

JS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtrywehoqz.html

TS:   process.env.HOME
来源：http://hz.nanxinkj.top/gtchytcklv.html

Java: System.getenv("HOME")
来源：http://hz.cashguo.top/gtrjjpvllr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.tianlin.xyz/gtievwcjos.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtyatlcnfp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ybcxt.top/gtbleikles.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gtkiryveyf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtiebcfwds.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.kuanghao11.cn/gtnhrzwpnf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtbctdmbxb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jyoumei.cn/gtqbksegxu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtkivnddzf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.9152youxi.cn/gtuaccjogi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydzc1.top/gtcmkreowq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.dashuyun.cn/gtcdlzhooy.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtweufnxoh.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtaktzzhdr.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtgbjgizhr.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtxykmpzdi.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtmrabaiyl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtiakecldp.html

Go:   os.Getwd()
来源：http://hz.snrcjt.cn/gtticdyixv.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtrzovadxo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtpnjybyrf.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtvrkzwcog.html

Py:   sys.exit(1)
来源：http://hz.hongshengwenyu.top/gtijvvmxnl.html

PHP:  exit(1);
来源：http://hz.sufxvd.cn/gtlbiwnoig.html

JS:   process.exit(1)
来源：http://hz.cheryme.top/gtsmtsetkg.html

TS:   process.exit(1)
来源：http://hz.jqgfzy.top/gtactipmae.html

Java: System.exit(1)
来源：http://hz.guowangkeji.top/gtxihmwukk.html

Go:   os.Exit(1)
来源：http://hz.pycfn.com/gtyssvbipf.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gthzkgwshr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gttcebuydb.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtzfifsnll.html

Py:   print("err", file=sys.stderr)
来源：http://hz.smart0.xyz/gtvzplzdsd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtbtfzyzsw.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtnltryymc.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtpoecpoor.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtvivmsgey.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xinyue.icu/gtnkzdssog.html

Ruby: warn "err"
来源：http://hz.haohaochexian.top/gtfhnuzdiz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuanzhike.top/gtrsevicxg.html

[M07] 判断是否为主入口
来源：http://hz.vqdsnc.cn/gtulafvuqu.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtjpwxkate.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gthusosgcd.html

JS:   require.main === module
来源：http://hz.sysykeji.top/gtclkkefkn.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtwfpntrje.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gttbtvuhxd.html

Go:   func main()
来源：http://hz.52xcode.cn/gtjazdecys.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shuidangran.top/gteygaxbqb.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtdppmrbme.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtpbwthdpq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenzaomai.com/gtxjrcdsps.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zycfv.cn/gtbkaqazsm.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtmzxgfukg.html

TS:   process.platform;  process.version
来源：http://hz.dianchejie.cn/gtdtrliskq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtdnheqrfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtxuefwgcf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gthldfqeie.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenlongwang.top/gtszfsolvy.html

================================================================================
来源：http://hz.jyoumei.cn/gtiuspwlmg.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtcbjetnaz.html

================================================================================
来源：http://hz.jianghu66.top/gtjyfzndxb.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtvpzovzna.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.mhx1999.top/gtxiypzhjz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtxuivggxi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtimywfabt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cheryme.top/gteymjiltc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtrxfjdpss.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.316326.xyz/gtqdfwgmwn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.redwolf501.top/gterfbjzue.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtjfhlcrcn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zdqjudy.top/gtwyyrgyuz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hywenlv.cn/gtmfkxdtkr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtybfhemnm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtegvrmjkt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtdasnayfx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtucwibpli.html

Go:   slices.Sort(arr)
来源：http://hz.316326.xyz/gtaigjraui.html

Ruby: arr.sort
来源：http://hz.guannengcc.top/gtbckacksw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.mhx1999.top/gttmsjoucl.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gtttlrvzye.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shanyushiyangkeji.top/gtolnavboo.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtoslqngyx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtfofswqmj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gtpkuhzyum.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj202588.top/gtbhxbeanf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gtehnuyjhn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ppjwa.cn/gtvvuoobiz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtmadbojnc.html

[N04] 斐波那契数列
来源：http://hz.quarkkingdee.top/gtsikoiedx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtseemtivj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuxming.cn/gtrtitkkpx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtnokvfxvv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtfhccfcto.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yonumen.top/gtgkoivamt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yongpay.top/gtvwscknja.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ydzc1.top/gtqzlrvgae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtnxjusmxw.html

[N05] 最大公约数
来源：http://hz.aibaodan.cn/gtudonzaok.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtspktihyp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.zhijiandao.cn/gtnfacgofz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zdqjudy.top/gtbzoiqsdn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hongshengwenyu.top/gtijenqpxa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.birdmap.top/gtvnwmcehv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.snrcjt.cn/gtwxtukiyz.html

Ruby: a.gcd(b)
来源：http://hz.yj20258888.top/gtuuwlttjh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhiwuduotai.top/gtxxnmtbho.html

[N06] 判断回文字符串
来源：http://hz.yuxming.cn/gtuwowxiui.html

Py:   s == s[::-1]
来源：http://hz.tanke756.top/gtbdybdjnz.html

PHP:  $s === strrev($s);
来源：http://hz.cqqwz.cn/gtndbnrqoy.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtpngrpayj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtyaekiouh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gtffzacctc.html

Go:   // 双指针从两端比较
来源：http://hz.cashguo.top/gtqavxwxqv.html

Ruby: s == s.reverse
来源：http://hz.chenlongwang.top/gtvzvfkowy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gtwkfcupcr.html

[N07] 两数之和（返回下标）
来源：http://hz.hnqzz.top/gtdwewaijm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xingfuxueyuan.xyz/gtzbyrkqnb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ybcxt.top/gtvoackuwo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jiagoushi.top/gtpftetwyb.html

TS:   // 手写 Map<string, number>
来源：http://hz.haohaochexian.top/gtdoaanrpv.html

Java: // 手写 HashMap
来源：http://hz.yonumen.top/gttpcorinj.html

Go:   // 手写 map[int]int
来源：http://hz.ppjwa.cn/gtarpgjbkz.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtaiyoenmu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zycfv.cn/gtejrssyyn.html

[N08] 生成全排列
来源：http://hz.shuidangran.top/gtrsbzygor.html

Py:   itertools.permutations(arr)
来源：http://hz.aizwys.cn/gtxlamhsps.html

PHP:  // 手写递归交换
来源：http://hz.yongpay.top/gtlzqfwvqp.html

JS:   // 手写回溯递归
来源：http://hz.havefunace.top/gtgftnltfi.html

TS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtufeexkkd.html

Java: // 手写回溯递归
来源：http://hz.jianghu66.top/gtpzyoyvkv.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtzkkynyoq.html

Ruby: arr.permutation.to_a
来源：http://hz.nwbrower.top/gtfjkovkdj.html

C#:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtkmthpger.html

[N09] 栈与队列
来源：http://hz.hysaishi.cn/gtdyctyuqd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.sufxvd.cn/gtbdysoomg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nwbrower.top/gtxrizxrcx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhengqikj.top/gtiovqdtbz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ivvv.top/gtrmvuobvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.snrcjt.cn/gtgvwqzhxh.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.tian-w.cn/gtkglzvdlf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.quarkkingdee.top/gtzbjlwkxq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxinkj.top/gtmtlqptfu.html

[N10] 链表节点定义
来源：http://hz.jinqigfzy.top/gtjefszeeb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.ydjk.org.cn/gttjsjyhay.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.quarkkingdee.top/gttswdwmez.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hongshengwenyu.top/gtbxnqlans.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.gaohongyu789.top/gthwnvdwwg.html

Java: class Node { int v; Node next; }
来源：http://hz.shuidangran.top/gtksmwbkrd.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ywan-chungtsiang.top/gtyslgceks.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.ehwqpu.com/gtujaynuho.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtjdyzcyea.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtlqonczkc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xuetiantiany.cn/gtgvnissyh.html

PHP:  // 手写递归函数
来源：http://hz.yongpay.top/gtmjitubhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258.top/gtfeflnklq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hysaishi.cn/gtmxnfrbob.html

Java: // 手写递归
来源：http://hz.ehwqpu.com/gtxkmsxqbj.html

Go:   // 手写递归
来源：http://hz.meibo888.top/gtgpqyuirg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xziqi.cn/gtmhvyeciy.html

C#:   // 手写递归
来源：http://hz.hywenlv.cn/gtdplveedd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ywan-chungtsiang.top/gtkzqpcrmb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtpartyrbl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zdqjudy.top/gtzasiufux.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtdsidnkwd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.vqdsnc.cn/gthwkowrlm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gzhubu.top/gtgbnxvfuf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.aibaodan.cn/gtsauwvhky.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.nwbrower.top/gtvwfgphya.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gogol.net.cn/gtpfrnbblb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqzpdyfaa.html

O. 并发与异步
来源：http://hz.jqgfzy.top/gtgjufxvyd.html

================================================================================
来源：http://hz.yonumen.top/gtshyqiabi.html

[O01] 启动一个线程
来源：http://hz.pengpengdd.cyou/gtdvpgzyve.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.dashuyun.cn/gtvexalryo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xinyue.icu/gtfxauiifb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuxming.cn/gtfvmyjcyp.html

TS:   // 同 JS
来源：http://hz.xuetiantiany.cn/gtqqojwuoq.html

Java: new Thread(() -> f()).start()
来源：http://hz.quarkkingdee.top/gtxbruulze.html

Go:   go f()
来源：http://hz.hnqzz.top/gteyfphxsl.html

Ruby: Thread.new { f }
来源：http://hz.shuidangran.top/gtphuesqsa.html

C#:   Task.Run(() => F());
来源：http://hz.bjfxy.top/gtaycgrmmk.html

[O02] 使用线程池
来源：http://hz.cucudq.cn/gtxgquwckc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydjk.org.cn/gthhcwtjci.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.guowangkeji.top/gtbtvnktui.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258.top/gtqqqucppo.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtoqmqybph.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.tianlin.xyz/gtilvjetqt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.sufxvd.cn/gtiijonknd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.meibo888.top/gtqecdhsna.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.fzhhl.top/gtqmlxcynl.html

[O03] 加锁保护共享数据
来源：http://hz.guannengcc.top/gtsoyzpiqr.html

Py:   with lock: shared += 1
来源：http://hz.gzhubu.top/gtnyobljfi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.dashuyun.cn/gtlyybqtaz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.c1oappe.top/gtwshrtpsq.html

TS:   // 同 JS
来源：http://hz.xylfe.cn/gtfraewnxb.html

Java: synchronized (this) { shared++; }
来源：http://hz.zhixingplan.top/gtmxymwatr.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sufxvd.cn/gtmtpafnwz.html


<!-- 参考信息 -->