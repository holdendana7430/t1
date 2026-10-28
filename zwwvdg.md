代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.vqdsnc.cn/gtokpsgzlv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtmxswkaho.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gtepdgkddo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtdqbtoasf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.redwolf501.top/gtxbywtimt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangtech.top/gtxaytxamj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtwomjfuyk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtxwxknodx.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtgtjekevh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtjmelbqbz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hnqzz.top/gteambifzk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xingfuxueyuan.xyz/gtoaevevct.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gttmrtfcea.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gtrqvsnxyr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fengsongda.top/gtqxegtckb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gtszrofyml.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yongpay.top/gtzmahqeek.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtiegsvgwq.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtlossyzub.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.svipenyu.cn/gtfbhvgdom.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtbftfdymu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtjfmgksmg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtdcvsjdsd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtilpsssda.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jiagoushi.top/gtpdtjukej.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtcaveidqc.html

[L05] 上传文件（multipart）
来源：http://hz.fzhhl.top/gtoidaaqrr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aizwys.cn/gtnzenbgqd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtsjncbnlm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sufxvd.cn/gtgmcgkhha.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtujcpbwzc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gteijqqjcx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ehwqpu.com/gtceuaqkom.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gtxhzgiixq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.smart0.xyz/gthmlyqfsf.html

[L06] 解析响应为 JSON
来源：http://hz.ehwqpu.com/gtrmdcawja.html

Py:   resp.json()
来源：http://hz.haohaochexian.top/gtjsoruerv.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtaikkzayy.html

JS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtzpbmrhef.html

TS:   await resp.json()
来源：http://hz.tanke756.top/gtwobpzkfc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aizwys.cn/gtorntvnvx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gtmpavxruw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yanxiufei.cn/gtuoarukqz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pycfn.com/gtvamxezaf.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj202588.top/gtmhitsphu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sxryk.cn/gtanvmtzje.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtnbzyjpze.html

JS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gticvorift.html

TS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtsonczltu.html

Java: resp.statusCode()
来源：http://hz.zdqjudy.top/gtmtxxzzvv.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtmskkhimy.html

Ruby: resp.code.to_i
来源：http://hz.yongpay.top/gttrqqxirv.html

C#:   (int)resp.StatusCode
来源：http://hz.daxiang520.top/gtsgwbrnur.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gttessskea.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuxming.cn/gtivwytkdq.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtibwzvsvh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtqgqutqov.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gthhsgzosc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtsgzbbvun.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.nanxinkj.top/gtldyebcpz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sufxvd.cn/gtbdypwowl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.feifeiyinyue.top/gteyyzwblz.html

================================================================================
来源：http://hz.fzhhl.top/gtnpllimor.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtdbbtsaix.html

================================================================================
来源：http://hz.52xcode.cn/gtsenogtgl.html

[M01] 读取命令行参数
来源：http://hz.shzxlz.cn/gtdknyzlns.html

Py:   sys.argv[1:]
来源：http://hz.xuetiantiany.cn/gtlvbtyset.html

PHP:  $argv;  $argc;
来源：http://hz.jqgufenzy.top/gtuqabinsu.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtbilacpdv.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtzkfwacex.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gtcutnmyek.html

Go:   os.Args[1:]
来源：http://hz.jlsjyb.cn/gtdiuhqkvq.html

Ruby: ARGV
来源：http://hz.yj202588.top/gticewxrnu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtlqvbhmyl.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gtborcekpt.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gttqqrhxxp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtycolwgxa.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtcueqtrdw.html

TS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtlpsduxek.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtwtroairc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ppjwa.cn/gtguzokijl.html

Ruby: ENV["HOME"]
来源：http://hz.gotoacloud.top/gtplbuvivq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.316326.xyz/gtgxbfgkdp.html

[M03] 执行外部命令
来源：http://hz.chenjidiqi.icu/gtkpfzuufb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sysykeji.top/gtbkemzttr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenzaomai.com/gtqsucybwk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtktozludb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtyczsycqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtemegmqym.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sweek.top/gtogkfmlva.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtukwqtgjn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gthtdfkmvs.html

[M04] 获取当前工作目录
来源：http://hz.yanxiufei.cn/gtxupmdcyx.html

Py:   os.getcwd()
来源：http://hz.hfpthk.cn/gtejiynkrs.html

PHP:  getcwd();
来源：http://hz.kuanghao11.cn/gtarbploun.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtpguhuxdj.html

TS:   process.cwd()
来源：http://hz.gaohongyu789.top/gteflcuxbe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.birdmap.top/gtnspwiovh.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtxbsmsfyb.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtyhkfyshu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dashuyun.cn/gtisrwvbkn.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gtnuragijs.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gttiomplet.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtwarjrdub.html

JS:   process.exit(1)
来源：http://hz.tanke756.top/gtitbjmprz.html

TS:   process.exit(1)
来源：http://hz.guannengcc.top/gtyoymjcqn.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtbztsvyal.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gtgoklyeyj.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtyxavzmsr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtokurvbyo.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtvmugapmn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtzxvclkrn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.havefunace.top/gtdbvfkblg.html

JS:   console.error("err")
来源：http://hz.sxryk.cn/gtqjsdqdqh.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtjwrqbthq.html

Java: System.err.println("err")
来源：http://hz.ydjk.org.cn/gtkciobgzy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinyuanbaomall.cn/gttxgrpqpi.html

Ruby: warn "err"
来源：http://hz.cheryme.top/gtewppmpsr.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.vqdsnc.cn/gthmyjybmt.html

[M07] 判断是否为主入口
来源：http://hz.sufxvd.cn/gtabpexrnw.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtiqmeqzka.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtpqpqwtdb.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtgimudjwz.html

TS:   require.main === module
来源：http://hz.yj20258.top/gtrmiyditr.html

Java: public static void main(String[] args)
来源：http://hz.kuanghao11.cn/gtpricwdwb.html

Go:   func main()
来源：http://hz.zycfv.cn/gtlaneibhm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhiwuduotai.top/gtdhbnsylg.html

C#:   static void Main(string[] args)
来源：http://hz.sxryk.cn/gtpgzdlttc.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtcoiwunxq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pycfn.com/gtrlvdwlvv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shanyushiyangtech.top/gtlydkogux.html

JS:   process.platform;  process.version
来源：http://hz.jqgufenzy.top/gthepeaxbk.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtbokcvtnw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jiagoushi.top/gtyesejqtm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.dashuyun.cn/gtomdfmjqo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.chenjidiqi.icu/gtnnnkumtq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.meibo888.top/gticifwvlv.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwautqzxz.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtsgbnucov.html

================================================================================
来源：http://hz.jqgfzy.top/gtaxnqybom.html

[N01] 二分查找（有序数组）
来源：http://hz.tian-w.cn/gtpnhobosd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtxvvapgbq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtrswpnqbe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gtlwrevypo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtfmwooomq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gthcfngnhs.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtbcgplbey.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtabyyazqn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtopgtsrdn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.nanxuanxn.top/gtnswivuvf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gttfldgnqj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.andypj.xyz/gtspvjopno.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xuetiantiany.cn/gtbbcomzze.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gturscsngn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hnxiangtu.top/gtjpxttgpi.html

Go:   slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtjdtihdvh.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gttjarrnbf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.fzhhl.top/gtedoccarc.html

[N03] 快速排序（分治示例）
来源：http://hz.jinyuanbaomall.cn/gtjkobbysw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yuxming.cn/gtjtduscsu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhaomingkeji.xyz/gtlvzrsyud.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtvbgrtxrv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cdnleiting.top/gtlcqeiiwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gaohongyu789.top/gtkauzikhq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jyoumei.cn/gtacehemjj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhongyouzk.top/gtykepcllb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtaezdrigq.html

[N04] 斐波那契数列
来源：http://hz.shuidangran.top/gtbvmnlgpr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtdbcigfuo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtsgxcuipu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtyoxygxjn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gttdrspttx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guowangkeji.top/gtnwalaajb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtbsftcllw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtvoewhdeq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.ehwqpu.com/gtaikfvncz.html

[N05] 最大公约数
来源：http://hz.guowangkeji.top/gtmporailj.html

Py:   math.gcd(a, b)
来源：http://hz.shanyushiyangkeji.top/gtbrxjgjeb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hnxiangtu.top/gtxqkhexht.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtmegrsomt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ppjwa.cn/gtyrvyhkzw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sysykeji.top/gtqvsvmufg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtiswgepoa.html

Ruby: a.gcd(b)
来源：http://hz.xziqi.cn/gtasnfsuzx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtmbxdebkk.html

[N06] 判断回文字符串
来源：http://hz.tianlin.xyz/gtlmfjhtov.html

Py:   s == s[::-1]
来源：http://hz.yangfankeji.com/gtppjfwcjz.html

PHP:  $s === strrev($s);
来源：http://hz.ybcxt.top/gtfihwmifa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtbliojtlg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtzmxbxduv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.dashuyun.cn/gtqfokwctm.html

Go:   // 双指针从两端比较
来源：http://hz.ybcxt.top/gtloqtsqct.html

Ruby: s == s.reverse
来源：http://hz.chenjidiqi.icu/gtknppnxyv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtvniakkxx.html

[N07] 两数之和（返回下标）
来源：http://hz.chenjidiqi.icu/gtuatgkvla.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.dashuyun.cn/gtujscncyd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.jinqigfzy.top/gtlfhesvqa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtldmmuqnb.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtgblwkczb.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtuqxgovop.html

Go:   // 手写 map[int]int
来源：http://hz.zhoulong.xyz/gtylauqagy.html

Ruby: // 手写 Hash
来源：http://hz.hnxiangtu.top/gtfxavrtdg.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yangfankeji.com/gttrhyzjuq.html

[N08] 生成全排列
来源：http://hz.smart0.xyz/gtwsxrnged.html

Py:   itertools.permutations(arr)
来源：http://hz.hnqzz.top/gtiwnkxuwo.html

PHP:  // 手写递归交换
来源：http://hz.sweek.top/gtzxohnbol.html

JS:   // 手写回溯递归
来源：http://hz.meibo888.top/gtragtxhgm.html

TS:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtzeppdmyh.html

Java: // 手写回溯递归
来源：http://hz.haohaochexian.top/gtvvdslfhz.html

Go:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtvkkpmhhu.html

Ruby: arr.permutation.to_a
来源：http://hz.yj202588.top/gtjtrgfzdj.html

C#:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtfpviaoor.html

[N09] 栈与队列
来源：http://hz.c1oappe.top/gtsriuxbah.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtthwaxqpk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenjidiqi.icu/gtzltmttlz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtwescjhrb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.andypj.xyz/gtxwwijidb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtcadxnkkk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtpmiaxnjk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtugqnfczx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.nanxuanxn.top/gtfypmuawp.html

[N10] 链表节点定义
来源：http://hz.ydzc1.top/gthoapmdfn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtkroogqmg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.jqgfzy.top/gtkspqeifw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.redwolf501.top/gtzbqmisqs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.iojbl.cn/gtboomnmbk.html

Java: class Node { int v; Node next; }
来源：http://hz.hnxiangtu.top/gtzfddszfc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.svipenyu.cn/gtndlaupmg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.hnxiangtu.top/gtxnxkzpnk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.xylfe.cn/gtanyfnjek.html

[N11] 二叉树中序遍历
来源：http://hz.dashuyun.cn/gtglumndir.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jiagoushi.top/gtpnrcahen.html

PHP:  // 手写递归函数
来源：http://hz.yonumen.top/gtrlyttnvk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shzxlz.cn/gtsjkgfsvs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.shanyushiyangkeji.top/gtydgcvsrn.html

Java: // 手写递归
来源：http://hz.aizwys.cn/gtzwjycykh.html

Go:   // 手写递归
来源：http://hz.yonumen.top/gtvzthrpoi.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yvedp.cn/gtknfhtcjk.html

C#:   // 手写递归
来源：http://hz.ywan-chungtsiang.top/gtvdlacokx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xuanzx.com/gttxbjbczw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.hnxiangtu.top/gtqivldydf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gtgjiumrga.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.fengsongda.top/gtudroqgpv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.gogol.net.cn/gtnxpayvqj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.shanyushiyangkeji.top/gtknjengyy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.shanyushiyangtech.top/gtverhqxel.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jlsjyb.cn/gtdvqhwgre.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.vqdsnc.cn/gtknakasqg.html

================================================================================
来源：http://hz.smart0.xyz/gtihzkppvn.html

O. 并发与异步
来源：http://hz.quarkkingdee.top/gtyzsjxeda.html

================================================================================
来源：http://hz.iojbl.cn/gtnxowpgdo.html

[O01] 启动一个线程
来源：http://hz.shzxlz.cn/gtbhrrynuy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jqgufenzy.top/gtygkralqs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.tianlin.xyz/gttkbmqxqz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.quarkkingdee.top/gtkbhbhsaf.html

TS:   // 同 JS
来源：http://hz.gaohongyu789.top/gtyydleede.html

Java: new Thread(() -> f()).start()
来源：http://hz.aizwys.cn/gtghphldhu.html

Go:   go f()
来源：http://hz.snrcjt.cn/gtaczdbjwa.html

Ruby: Thread.new { f }
来源：http://hz.gotoacloud.top/gtbosdwkgm.html

C#:   Task.Run(() => F());
来源：http://hz.cdnleiting.top/gtsqxkgmvi.html

[O02] 使用线程池
来源：http://hz.daria6918.cn/gtiobdjgwx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj202588.top/gtywjlluad.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.kuanghao11.cn/gttijqifoc.html

JS:   // worker_threads 线程池
来源：http://hz.chenzaomai.com/gtmdupopjf.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gttgtjpzkx.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtjbbqihlt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gotoacloud.top/gtsccqqrwi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.pengpengdd.cyou/gtaklhfgxh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.xuanzx.com/gtjehaoyuh.html

[O03] 加锁保护共享数据
来源：http://hz.gaohongyu789.top/gtryljaqzi.html

Py:   with lock: shared += 1
来源：http://hz.shuidangran.top/gtyluxzrqa.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.snrcjt.cn/gtbkmulmhw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cqqwz.cn/gtvazjssft.html

TS:   // 同 JS
来源：http://hz.haohaochexian.top/gtwdykaymz.html

Java: synchronized (this) { shared++; }
来源：http://hz.yonumen.top/gtspoeqjte.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.sxryk.cn/gtqumjhhdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.yj20258.top/gtobfzadjr.html

C#:   lock (gate) { shared++; }
来源：http://hz.pycfn.com/gtdovmxbqy.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtkhmtefdg.html

Py:   async def f():⏎    await g()
来源：http://hz.daria6918.cn/gthdnbyaxp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.cqqwz.cn/gtumfjnygf.html

JS:   async function f() { await g(); }
来源：http://hz.nanxuanxn.top/gtwssltzpd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.hnxiangtu.top/gtpjyanfrv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.pycfn.com/gtzufuaqcw.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sxryk.cn/gtghhakgcv.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.ywan-chungtsiang.top/gtmukbgnez.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtkvtgrjtk.html

[O05] 并发执行并等待全部完成
来源：http://hz.xinyue.icu/gtpizfkrtk.html

Py:   asyncio.gather(*tasks)
来源：http://hz.dianchejie.cn/gthpwsafcq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.iojbl.cn/gtonkvvbrg.html

JS:   await Promise.all(tasks)
来源：http://hz.pengpengdd.cyou/gtnqylogty.html

TS:   await Promise.all(tasks)
来源：http://hz.cheryme.top/gtdlnrdrzx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.yongpay.top/gteuvbjcim.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.zhoulong.xyz/gtlyxhqwxz.html

Ruby: threads.map(&:join)
来源：http://hz.daxiang520.top/gtvduqjeag.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.aibaodan.cn/gtuzogbrgj.html

[O06] 使用进程池
来源：http://hz.havefunace.top/gtvqnfhtal.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.guowangkeji.top/gtvuircgmr.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.c1oappe.top/gtcfpjxiko.html

JS:   // child_process / cluster 模块
来源：http://hz.sxryk.cn/gtgytrdbpz.html


<!-- 参考信息 -->