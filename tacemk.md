代发 wailian999

L. 网络请求
来源：http://hz.sweek.top/gtvedgnrmc.html

================================================================================
来源：http://hz.xylfe.cn/gtpfnounli.html

[L01] 发送 GET 请求
来源：http://hz.xuetiantiany.cn/gtkplggshd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtrqwltzjg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gtdiydtdgq.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtktwxkhya.html

TS:   await fetch(url)
来源：http://hz.ehwqpu.com/gtigiqlzws.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.316326.xyz/gtjkafejtx.html

Go:   resp, err := http.Get(url)
来源：http://hz.ywan-chungtsiang.top/gtvcyodfwg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.redwolf501.top/gtljhfcmns.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtgqxpbawc.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtwkuswyit.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtnxpsejac.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtsrxjvnsp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtfeogkyyy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtskhfppgv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtqmbhgxkq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pycfn.com/gtfyebepdu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtlaffkhpf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gttzniweld.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtmxynqdwm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.c1oappe.top/gtsxhlthcd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtnobtkqls.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtvqhncevr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtdjxrjsjb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hysaishi.cn/gtrfqrrjsl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.birdmap.top/gtlbtbqqlc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gotoacloud.top/gtpbysufon.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtwwagaiht.html

[L04] 设置超时
来源：http://hz.fzhhl.top/gtwxtlwocw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtalyedimd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sxryk.cn/gteuczvvaa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtnzvkotyn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtysyurnud.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtemvzgfhb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtlqpsepad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenzaomai.com/gtqzhebdqn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenzaomai.com/gtoxjkyhwc.html

[L05] 上传文件（multipart）
来源：http://hz.sweek.top/gttwseangy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.ydjk.org.cn/gtukqaelkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydjk.org.cn/gtvyhzfuic.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gttapjzstd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtzpnxifzy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtefulviro.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinghuilouyu.cn/gtwberpalc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtvxhpazzq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtvncpvogq.html

[L06] 解析响应为 JSON
来源：http://hz.kuanghao11.cn/gtrygoqnch.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtudfxliwq.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtyqeousho.html

JS:   await resp.json()
来源：http://hz.hammf.cn/gtbbjwtnvg.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gtfblfmylv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtzreljmdg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ydjk.org.cn/gtnovcxgma.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtxlajpngr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtwszgthok.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtbcqobuse.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtkljabmwb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtrqphvrym.html

JS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtrpggmenh.html

TS:   resp.ok;  resp.status
来源：http://hz.redwolf501.top/gthmitaaep.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gthjiyuehf.html

Go:   resp.StatusCode
来源：http://hz.jyoumei.cn/gtpnlobwwo.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtomlqcynj.html

C#:   (int)resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtxbwicamk.html

[L08] 并发请求多个地址
来源：http://hz.zhoulong.xyz/gtaruvvesy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gthdvvqwxv.html

PHP:  curl_multi_init() 系列
来源：http://hz.xylfe.cn/gtesgrurqj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtgpiuwzuh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtlrqvhbcr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtiatntpir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhoulong.xyz/gtiedesrqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shuidangran.top/gtorjquuzd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtyhovyxkq.html

================================================================================
来源：http://hz.meibo888.top/gtmsefisfr.html

M. 命令行 / 进程 / 环境
来源：http://hz.guannengcc.top/gtvtquyhlt.html

================================================================================
来源：http://hz.cdnleiting.top/gtlsememik.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtyszslnla.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gtpmfsdejv.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtwjrqosgf.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtqavfaxil.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtxksifszz.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtphazhfqi.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtndrtyotl.html

Ruby: ARGV
来源：http://hz.yuxming.cn/gtebbocksm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtihltwehi.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gtytkdhvlt.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtyfedjzrq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gttvlexonu.html

JS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtztfxuqhj.html

TS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtsvgogcov.html

Java: System.getenv("HOME")
来源：http://hz.chenzaomai.com/gtakpzroja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zycfv.cn/gtvbezjwtx.html

Ruby: ENV["HOME"]
来源：http://hz.pycfn.com/gtrwtfcuau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jyoumei.cn/gtwayibhev.html

[M03] 执行外部命令
来源：http://hz.zdqjudy.top/gtzcszbqpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xziqi.cn/gtytpbmmrf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtdpbdwhgo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gttsoeznkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtdvehnhct.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangkeji.top/gtemrsuhtj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gotoacloud.top/gttbtkwdxs.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtmgsnimnf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yj20258.top/gtjtgjygdi.html

[M04] 获取当前工作目录
来源：http://hz.zhijiandao.cn/gtmnqcwikl.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtgqysnmmm.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtkomxipjd.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtnjdlcbfk.html

TS:   process.cwd()
来源：http://hz.redwolf501.top/gtuhvyktpe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtxcuwpowm.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtepfflwdv.html

Ruby: Dir.pwd
来源：http://hz.fengsongda.top/gtggzgageq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tian-w.cn/gteilhtnqp.html

[M05] 设置退出码
来源：http://hz.gzhubu.top/gtlzirxmoj.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtpbokfjtm.html

PHP:  exit(1);
来源：http://hz.haohaochexian.top/gthbqbjzli.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtxpemqqpg.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gtbnuhoorj.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtuytrotqc.html

Go:   os.Exit(1)
来源：http://hz.chenzaomai.com/gtsgalrmfa.html

Ruby: exit 1
来源：http://hz.c1oappe.top/gtdchvsliu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gaohongyu789.top/gtivblvxsl.html

[M06] 向标准错误输出
来源：http://hz.nwbrower.top/gtbiludnvg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shuidangran.top/gtgbusaaaw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangkeji.top/gtdybntoku.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtfveadbto.html

TS:   console.error("err")
来源：http://hz.gogol.net.cn/gtrhokioos.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtnapqeyzx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hfpthk.cn/gtvpdpguuf.html

Ruby: warn "err"
来源：http://hz.zhijiandao.cn/gtlosyojmf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtltnhpykp.html

[M07] 判断是否为主入口
来源：http://hz.hnqzz.top/gtlwfpdiof.html

Py:   if __name__ == "__main__":
来源：http://hz.svipenyu.cn/gtbffuzkgx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinghuilouyu.cn/gtoulorwjd.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gthsuoxyib.html

TS:   require.main === module
来源：http://hz.cheryme.top/gtgrxxgpuc.html

Java: public static void main(String[] args)
来源：http://hz.dianchejie.cn/gtyrlbwpos.html

Go:   func main()
来源：http://hz.zhengqikj.top/gtsyfmvqjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hysaishi.cn/gtywxmmnda.html

C#:   static void Main(string[] args)
来源：http://hz.c1oappe.top/gtqapngxgb.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gthlrtkria.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtrpxdkhmp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtxsahenbb.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtulcdyvoo.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gttjushtyx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xingfuxueyuan.xyz/gtfadwrbvg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xinyue.icu/gtwailshoh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ydjk.org.cn/gtftiklkgj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.andypj.xyz/gtbpqptfjm.html

================================================================================
来源：http://hz.guannengcc.top/gtryetmmhm.html

N. 数据结构与算法
来源：http://hz.mhx1999.top/gtgltajevt.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlqpwmveg.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtcszjwayr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtjnuxwcrw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtmxyggfec.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tianlin.xyz/gtzqqqtgvg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtvhrewccs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.bjfxy.top/gtoyqfmuyi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gtyateuxxc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tanke756.top/gtvwmkcdpj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtgmmujgsh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yongpay.top/gtizhlvspm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtikzjqvaw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtkauxkuwb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtfeltxlkw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtdwevuhgh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.iojbl.cn/gtavselcvn.html

Go:   slices.Sort(arr)
来源：http://hz.yj20258888.top/gtolywpqmj.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtwazxzeuj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.cdnleiting.top/gtqhilsjqh.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxinkj.top/gtwwzbfkhf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gzhubu.top/gthtjrloeg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.redwolf501.top/gtmnllfluv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hywenlv.cn/gtlkvaofhb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.chenjidiqi.icu/gtazarqgpu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.andypj.xyz/gtqqvingnc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangkeji.top/gtcolrnqjh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gthputvmfa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yangfankeji.com/gtmwrzygkf.html

[N04] 斐波那契数列
来源：http://hz.xinyue.icu/gtvvgnmres.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtolvjwywb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ybcxt.top/gtdodjoolz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtkrxfqwfd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.havefunace.top/gtgkxrennl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.pengpengdd.cyou/gtbvubfkmi.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zdqjudy.top/gtqggiixri.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gttggwbzlh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtesqjtdjp.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gtwftkdkwl.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtivohigmz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtkagtbgwi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtkanlcfnc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.0kj1m.cn/gtwgkgsslm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nwbrower.top/gturaccyld.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jinqigfzy.top/gtnieksrct.html

Ruby: a.gcd(b)
来源：http://hz.snrcjt.cn/gtjixpuoes.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gotoacloud.top/gtmrykviox.html

[N06] 判断回文字符串
来源：http://hz.yj20258.top/gtacrioiig.html

Py:   s == s[::-1]
来源：http://hz.feifeiyinyue.top/gtjqygpcwh.html

PHP:  $s === strrev($s);
来源：http://hz.nwbrower.top/gtcrdfjxkn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtyhezxquf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtxdnnfoae.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cqqwz.cn/gtxopahfme.html

Go:   // 双指针从两端比较
来源：http://hz.aibaodan.cn/gtzwgwdrhs.html

Ruby: s == s.reverse
来源：http://hz.nwbrower.top/gtcsgkclop.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtcqssicuk.html

[N07] 两数之和（返回下标）
来源：http://hz.zhaomingkeji.xyz/gtciuzmtlo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtttxgcjne.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ehwqpu.com/gtjmrxcvco.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtlsbsvkmu.html

TS:   // 手写 Map<string, number>
来源：http://hz.xuanzx.com/gtapsiijwr.html

Java: // 手写 HashMap
来源：http://hz.pycfn.com/gtikjlsxfg.html

Go:   // 手写 map[int]int
来源：http://hz.hysaishi.cn/gtgkzlxvbg.html

Ruby: // 手写 Hash
来源：http://hz.0kj1m.cn/gtunsviemk.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtuwvckldf.html

[N08] 生成全排列
来源：http://hz.zycfv.cn/gtiyfvgaec.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtahkbynzy.html

PHP:  // 手写递归交换
来源：http://hz.zdqjudy.top/gtyvokhfow.html

JS:   // 手写回溯递归
来源：http://hz.zhoulong.xyz/gtihjozufd.html

TS:   // 手写回溯递归
来源：http://hz.zhengqikj.top/gtflinjlek.html

Java: // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtfxbrekmn.html

Go:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtibbjskbh.html

Ruby: arr.permutation.to_a
来源：http://hz.jinghuilouyu.cn/gtlkzbzamc.html

C#:   // 手写回溯递归
来源：http://hz.ppjwa.cn/gtuxoffygc.html

[N09] 栈与队列
来源：http://hz.zhengqikj.top/gtuppguykv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhongyouzk.top/gtchmlmste.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtulmvtfch.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yj202588.top/gtgkolldal.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jyoumei.cn/gtftmbthgn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.meibo888.top/gtagzqkwkt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gtvfxyqgko.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.dianchejie.cn/gtkpnotlxm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.birdmap.top/gtojyehpry.html

[N10] 链表节点定义
来源：http://hz.hnxiangtu.top/gtahkhmtrd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yuxming.cn/gthwcewzru.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hywenlv.cn/gtodiapjfd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtktvzzlui.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hongshengwenyu.top/gtunmxrywz.html

Java: class Node { int v; Node next; }
来源：http://hz.ppjwa.cn/gtlfgaepya.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.wangshuangyany.cn/gtnwrukkrq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jinghuilouyu.cn/gtlcvqzkbk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jianghu66.top/gtelgqmzjc.html

[N11] 二叉树中序遍历
来源：http://hz.zhengqikj.top/gtxnqkkune.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.smart0.xyz/gtknlofwty.html

PHP:  // 手写递归函数
来源：http://hz.cdnleiting.top/gtbeubcorg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xuanzx.com/gttlecfsrh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yangfankeji.com/gtckrihxgz.html

Java: // 手写递归
来源：http://hz.andypj.xyz/gtzrnwgzru.html

Go:   // 手写递归
来源：http://hz.cqqwz.cn/gtbyytaqrg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yanxiufei.cn/gtavhkupof.html

C#:   // 手写递归
来源：http://hz.hfpthk.cn/gtftdsrhcd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.chenlongwang.top/gtwqkclhcg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtuvwstuko.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.yj202588.top/gtafqgeyec.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtdtmktzgt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhijiandao.cn/gtqfvunfky.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yonumen.top/gtrhopouhr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.yj202588.top/gticjyjgrz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ivvv.top/gthtljbtnv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tanke756.top/gtiwtivguz.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtofkzkove.html

O. 并发与异步
来源：http://hz.xuetiantiany.cn/gtmolxgeso.html

================================================================================
来源：http://hz.zhoulong.xyz/gthxiwlvvh.html

[O01] 启动一个线程
来源：http://hz.vqdsnc.cn/gtqaywnchx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtqpfanclm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.xylfe.cn/gttboxebbl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.ybcxt.top/gtticthzgu.html

TS:   // 同 JS
来源：http://hz.daria6918.cn/gtegsdlytl.html

Java: new Thread(() -> f()).start()
来源：http://hz.jinqigfzy.top/gtipyzzptv.html

Go:   go f()
来源：http://hz.zhoulong.xyz/gtnoyatsny.html

Ruby: Thread.new { f }
来源：http://hz.hammf.cn/gtihfmoinv.html

C#:   Task.Run(() => F());
来源：http://hz.yvedp.cn/gtjzmppoqa.html

[O02] 使用线程池
来源：http://hz.chenzaomai.com/gtbknysfbi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtedjldlpv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.tanke756.top/gteigqzlid.html

JS:   // worker_threads 线程池
来源：http://hz.yj20258888.top/gtqsseltmk.html

TS:   // worker_threads 线程池
来源：http://hz.quarkkingdee.top/gtqsqpjhes.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.hammf.cn/gtpriotztb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gaohongyu789.top/gtddnwfeah.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shzxlz.cn/gtpmdkisjp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.yj20258888.top/gtejtwhyzl.html

[O03] 加锁保护共享数据
来源：http://hz.yj20258888.top/gtmkbgbtky.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtlxpowpzd.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.yvedp.cn/gtsptyirqx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.gzhubu.top/gtriffwrkr.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtzuabybwl.html

Java: synchronized (this) { shared++; }
来源：http://hz.sysykeji.top/gtvwpgoajt.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.aizwys.cn/gtskgxdciy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.zycfv.cn/gtupzsskwe.html

C#:   lock (gate) { shared++; }
来源：http://hz.yuanzhike.top/gthlqykrhh.html

[O04] 定义异步函数并等待
来源：http://hz.ppjwa.cn/gtjewdynpx.html

Py:   async def f():⏎    await g()
来源：http://hz.ywan-chungtsiang.top/gtvbrwkrcw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.316326.xyz/gtkaaujjzl.html

JS:   async function f() { await g(); }
来源：http://hz.daria6918.cn/gteeakhpyr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hongshengwenyu.top/gtnnapdeou.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shanyushiyangtech.top/gtnfriclyr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.svipenyu.cn/gtjepilrje.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.cheryme.top/gtoifeipzx.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigfzy.top/gtsngvdgov.html

[O05] 并发执行并等待全部完成
来源：http://hz.birdmap.top/gtfjdjlwew.html


<!-- 参考信息 -->