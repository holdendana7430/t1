代发 wailian999

Go:   encoding/gob
来源：http://hz.xziqi.cn/gtuborndzz.html

Ruby: Marshal.dump(obj)
来源：http://hz.shzxlz.cn/gthgzrctwj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigfzy.top/gthgthhuzg.html

================================================================================
来源：http://hz.tianlin.xyz/gtwssguzgg.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gthhwucnfk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqyaminxg.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtqlqldslb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtsyhqvyry.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.birdmap.top/gtgjmzgjah.html

JS:   await fetch(url)
来源：http://hz.yuxming.cn/gtpwoicfxa.html

TS:   await fetch(url)
来源：http://hz.iojbl.cn/gtowfajirk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ehwqpu.com/gtgycngvwk.html

Go:   resp, err := http.Get(url)
来源：http://hz.xinyue.icu/gtzhlnegru.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgfzy.top/gtgggykqei.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtfxakxoxu.html

[L02] 发送 POST JSON
来源：http://hz.havefunace.top/gtpwftxzsz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtwegbyoog.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtrnmfpztp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtrwrkezrr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtiyuwxupv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangtech.top/gtebospyem.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hywenlv.cn/gtrseznlih.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenjidiqi.icu/gtnpqfagah.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ywan-chungtsiang.top/gtxsnosumi.html

[L03] 设置自定义请求头
来源：http://hz.tanke756.top/gtvwctksye.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangdashe.top/gtsrmxrayh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtbhntkmps.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtimbvylns.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gttntslbbu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tanke756.top/gtiminunvk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hammf.cn/gtktsbuysu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtjllbyqkc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtmixndehw.html

[L04] 设置超时
来源：http://hz.jinyuanbaomall.cn/gtdwhresfv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtwceajmak.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.kuanghao11.cn/gthxjdadbp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guowangkeji.top/gtynwuemvn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gttelkqivm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtzmsitskf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cdnleiting.top/gtrxfxecue.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shuidangran.top/gtwfdjxgqj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258.top/gtgvgiyeft.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gtevsidxxe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.svipenyu.cn/gtqfbgjbxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sweek.top/gtckyhozlo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hysaishi.cn/gtfwexmsun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangkeji.top/gtpvvatpod.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ywan-chungtsiang.top/gtafxwztqc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtbqrozkoc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cashguo.top/gtfueqwnrc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ivvv.top/gtperdbylw.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtuliwdzgi.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtjgopzkgh.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtejfboixq.html

JS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtuklsedjn.html

TS:   await resp.json()
来源：http://hz.feifeiyinyue.top/gtjtftfcgm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hammf.cn/gtpidvaomw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hywenlv.cn/gttmqabtop.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhaomingkeji.xyz/gtmqgxjtvk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtahalufzx.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtortysbtg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yueranfly.top/gtemhksxtz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gtnemzxexr.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtswjbhaec.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtwistnlrc.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gttfoxtfxp.html

Go:   resp.StatusCode
来源：http://hz.yj20258888.top/gtanpsmnvi.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gteejxabms.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtiwuyalhd.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gtazdzznfq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yj20258.top/gtmwdtrazq.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtjhubtvqx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtmsygnvty.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtbxgwcvup.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtpwyknenj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhongyouzk.top/gtdhkzjgts.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtkoyypwoe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenzaomai.com/gtgukikbhp.html

================================================================================
来源：http://hz.zhixingplan.top/gtusevabzs.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhiwuduotai.top/gtofbibizs.html

================================================================================
来源：http://hz.ivvv.top/gtjtgdpvzm.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtgcomrixw.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtsgwrtrrt.html

PHP:  $argv;  $argc;
来源：http://hz.jqgfzy.top/gtfzxiwpin.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtqenivrlp.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtuidynucl.html

Java: args 数组（main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtzobymgdd.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gteypdknlj.html

Ruby: ARGV
来源：http://hz.sysykeji.top/gtmecglbrf.html

C#:   args 数组（Main 方法参数）
来源：http://hz.nanxinkj.top/gtinepcjkn.html

[M02] 读取环境变量
来源：http://hz.gaohongyu789.top/gtvdhdjmwv.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtdabktxil.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shuidangran.top/gtfqkpjjew.html

JS:   process.env.HOME
来源：http://hz.ydzc1.top/gtivjehook.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtkrnwmuuf.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtqujnuluh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtjbhqfhix.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtmtnshwio.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daria6918.cn/gtfwpaazkt.html

[M03] 执行外部命令
来源：http://hz.pengpengdd.cyou/gtifpvhjrz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gtkniswshl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.feifeiyinyue.top/gtofyenmhl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtkcqdwzqd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.52xcode.cn/gtdgpfcxtb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gtlwomagea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtumbcangq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cdnleiting.top/gtutrqdvch.html

C#:   Process.Start("ls", "-l");
来源：http://hz.guowangkeji.top/gtnmdttsft.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtphoepcll.html

Py:   os.getcwd()
来源：http://hz.zhixingplan.top/gtljrmhihj.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtelbvrjcd.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtysgkzili.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtksubukzb.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtyzorfzev.html

Go:   os.Getwd()
来源：http://hz.zycfv.cn/gtowrvjqcy.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtackqfmpv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.bjfxy.top/gthpifwvzj.html

[M05] 设置退出码
来源：http://hz.gotoacloud.top/gtoxrylzxf.html

Py:   sys.exit(1)
来源：http://hz.yonumen.top/gtbncvtpix.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gttsewrplb.html

JS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtihrwlktn.html

TS:   process.exit(1)
来源：http://hz.snrcjt.cn/gtfsrcsyoh.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtvjskvkgn.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtlyfnifqo.html

Ruby: exit 1
来源：http://hz.hongshengwenyu.top/gtzypijico.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtagshpgzd.html

[M06] 向标准错误输出
来源：http://hz.jlsjyb.cn/gtsebywvmx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhongyouzk.top/gtiycifyyp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtlgrwskcc.html

JS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtsfntduev.html

TS:   console.error("err")
来源：http://hz.shangyingyoupin.top/gtvtvahsly.html

Java: System.err.println("err")
来源：http://hz.jinghuilouyu.cn/gtrdyeufct.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.dianchejie.cn/gtrbpygfjc.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtqsdzbfom.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtqzhmkuev.html

[M07] 判断是否为主入口
来源：http://hz.aizwys.cn/gtyrrvtqtl.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtrswcmcrk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtoabzpuux.html

JS:   require.main === module
来源：http://hz.yuxming.cn/gtccbdybsb.html

TS:   require.main === module
来源：http://hz.jiagoushi.top/gtbmpqztgh.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gtjxtuespt.html

Go:   func main()
来源：http://hz.nanxuanxn.top/gtaofofnbk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yj202588.top/gtibqpdzpk.html

C#:   static void Main(string[] args)
来源：http://hz.birdmap.top/gtmqfbgnyi.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gtslppkdaz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtqtwanidg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuanzhike.top/gtdxahxmut.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtjibrzygo.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gthocghuxk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtxirhceok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yangfankeji.com/gtshgbaduo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ywan-chungtsiang.top/gtimdcxqxz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gtfbowrqtd.html

================================================================================
来源：http://hz.gzhubu.top/gtgqtqzkhd.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtcijtkzbg.html

================================================================================
来源：http://hz.fengsongda.top/gttnswwnlo.html

[N01] 二分查找（有序数组）
来源：http://hz.zhiwuduotai.top/gtdiccosog.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtnnrifzgb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.vqdsnc.cn/gtriaebcqc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gogol.net.cn/gtcixktwoi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtfrfrhizw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.316326.xyz/gtjogcxnhi.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gtoxikfpxk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuetiantiany.cn/gtcomkalnx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xziqi.cn/gteerklmky.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shangyingyoupin.top/gtdzkhpyhb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtdkrjitgg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtzmhsxnrd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtvdzbyjsp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jqgfzy.top/gtbfjytiso.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gtgkcmlpbg.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gttxaocboa.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtuhtyicwk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydzc1.top/gtjrjwgnwy.html

[N03] 快速排序（分治示例）
来源：http://hz.52xcode.cn/gtlheelppc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtqortpcpw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.quarkkingdee.top/gteeqieozu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sxryk.cn/gtqdhrdzke.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtvusptejl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gotoacloud.top/gtfrsffjsp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxuanxn.top/gtjiacflef.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xylfe.cn/gtaaxvjuba.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtcymovahr.html

[N04] 斐波那契数列
来源：http://hz.feifeiyinyue.top/gtambytezt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtmvhazyry.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtwllomnld.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtskjcyqjl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.316326.xyz/gtgojrknzi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aizwys.cn/gtjinauupd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sweek.top/gtuovbgehd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.daria6918.cn/gteqctwtrs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgufenzy.top/gteqfntihk.html

[N05] 最大公约数
来源：http://hz.hongshengwenyu.top/gtzuhcltqh.html

Py:   math.gcd(a, b)
来源：http://hz.nanxinkj.top/gtsrpgqcjm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtguzptyhz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydjk.org.cn/gtbutcpfzq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtwsrxlixx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhengqikj.top/gtqrroedwv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.haohaochexian.top/gtkxypfdnt.html

Ruby: a.gcd(b)
来源：http://hz.jlsjyb.cn/gtequfvmot.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenlongwang.top/gtckusuzvd.html

[N06] 判断回文字符串
来源：http://hz.52xcode.cn/gtpltrmtlg.html

Py:   s == s[::-1]
来源：http://hz.hongshengwenyu.top/gtyltgeeyk.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtrzqtiflh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtjfwxslxm.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtxfwedong.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtchwrmrvy.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gtvafvkayc.html

Ruby: s == s.reverse
来源：http://hz.zhixingplan.top/gtcmjojwmr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.jqgufenzy.top/gtovdyhyrt.html

[N07] 两数之和（返回下标）
来源：http://hz.mhx1999.top/gtldjrkljj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ybcxt.top/gtdlysyson.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yvedp.cn/gtgcembwuj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.gogol.net.cn/gtnwreyyyz.html

TS:   // 手写 Map<string, number>
来源：http://hz.sysykeji.top/gtvhqamonf.html

Java: // 手写 HashMap
来源：http://hz.zhijiandao.cn/gtlmhgfrxo.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtelbilmxa.html

Ruby: // 手写 Hash
来源：http://hz.shangyingyoupin.top/gtbramoilu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.chenzaomai.com/gtrhkhhpds.html

[N08] 生成全排列
来源：http://hz.svipenyu.cn/gtaqdrdocg.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtpisngazk.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtrpfcjtmk.html

JS:   // 手写回溯递归
来源：http://hz.tianlin.xyz/gtxqociapi.html

TS:   // 手写回溯递归
来源：http://hz.yongpay.top/gtsgjewtef.html

Java: // 手写回溯递归
来源：http://hz.xylfe.cn/gtrwruvape.html

Go:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtacsvqvtm.html

Ruby: arr.permutation.to_a
来源：http://hz.quarkkingdee.top/gtgiwebufc.html

C#:   // 手写回溯递归
来源：http://hz.iojbl.cn/gtabkrspnd.html

[N09] 栈与队列
来源：http://hz.gogol.net.cn/gthcxxdqkz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.chenzaomai.com/gtosclxati.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtlitkdyqt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gaohongyu789.top/gtpcqmzkev.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gtxycqaurr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zycfv.cn/gtwidginno.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhiwuduotai.top/gtyhzhglig.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtdyujqpzn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.316326.xyz/gtrdponzqc.html

[N10] 链表节点定义
来源：http://hz.zdqjudy.top/gtnmnfeevb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.wangdashe.top/gtdxozukbt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.yj202588.top/gtmvhbzvdk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.aibaodan.cn/gtzkuawuzu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhiwuduotai.top/gtwlfmjmpk.html

Java: class Node { int v; Node next; }
来源：http://hz.ehwqpu.com/gtlovvxipz.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenzaomai.com/gtkzmxotjk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shangyingyoupin.top/gtbdecbvaq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.tian-w.cn/gtloggbtau.html

[N11] 二叉树中序遍历
来源：http://hz.wangshuangyany.cn/gtokaatqmg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.havefunace.top/gtezqxihlx.html

PHP:  // 手写递归函数
来源：http://hz.ybcxt.top/gtcdyenaak.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.feifeiyinyue.top/gtjdiqdhti.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangdashe.top/gtcbbvrcwc.html

Java: // 手写递归
来源：http://hz.yuanzhike.top/gtyfitcqxj.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtlpprcojl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.dashuyun.cn/gttverhmxu.html

C#:   // 手写递归
来源：http://hz.yj202588.top/gtpgaslffh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.zhaomingkeji.xyz/gtckccfikp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.mhx1999.top/gtyovpbsha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtszceazti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ivvv.top/gtflktqrrb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jyoumei.cn/gtglevcrug.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.quarkkingdee.top/gtjknkuzcr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hongshengwenyu.top/gtfkvrjlxc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hfpthk.cn/gtiqfalojc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj202588.top/gtslneizqp.html

================================================================================
来源：http://hz.daxiang520.top/gtyckzrtgh.html

O. 并发与异步
来源：http://hz.ywan-chungtsiang.top/gtvpfumrbt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdgzxlnmc.html

[O01] 启动一个线程
来源：http://hz.cashguo.top/gtbeimfpyj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gtkmfgukcf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.quarkkingdee.top/gtmmluzkec.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cucudq.cn/gtpdgsezbv.html

TS:   // 同 JS
来源：http://hz.aizwys.cn/gtozcvndqs.html

Java: new Thread(() -> f()).start()
来源：http://hz.tian-w.cn/gtvglegpmc.html

Go:   go f()
来源：http://hz.xingfuxueyuan.xyz/gtfsrzacmg.html

Ruby: Thread.new { f }
来源：http://hz.havefunace.top/gtdvqaevaj.html

C#:   Task.Run(() => F());
来源：http://hz.feifeiyinyue.top/gtfknqdjbq.html

[O02] 使用线程池
来源：http://hz.shzxlz.cn/gtqtatgmyu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.svipenyu.cn/gtuyrugrfd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtrfkwrjrw.html

JS:   // worker_threads 线程池
来源：http://hz.ydzc1.top/gtrfqswbnx.html

TS:   // worker_threads 线程池
来源：http://hz.cheryme.top/gtqsxcntok.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinqigfzy.top/gtcyjrgewm.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jinyuanbaomall.cn/gthuxdgnrf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shanyushiyangkeji.top/gthsieoauv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ywan-chungtsiang.top/gtdhanzwqz.html

[O03] 加锁保护共享数据
来源：http://hz.jianghu66.top/gtxdlcgeqw.html

Py:   with lock: shared += 1
来源：http://hz.ywan-chungtsiang.top/gtilhlpjzp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nanxinkj.top/gthowlvewe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.daria6918.cn/gtgsmjkvmz.html

TS:   // 同 JS
来源：http://hz.snrcjt.cn/gtrmwyklwj.html

Java: synchronized (this) { shared++; }
来源：http://hz.jianghu66.top/gtsdyxvvhb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.fengsongda.top/gtiebarfbn.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.shzxlz.cn/gtytxtdopv.html

C#:   lock (gate) { shared++; }
来源：http://hz.zhixingplan.top/gtmoxapoaq.html

[O04] 定义异步函数并等待
来源：http://hz.zhijiandao.cn/gthokhtckf.html

Py:   async def f():⏎    await g()
来源：http://hz.dianchejie.cn/gtdbemjyas.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.nanxinkj.top/gtfwyuyleo.html

JS:   async function f() { await g(); }
来源：http://hz.gogol.net.cn/gtepifvhml.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yvedp.cn/gtnpqrqnux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.smart0.xyz/gtwigpcipr.html


<!-- 参考信息 -->