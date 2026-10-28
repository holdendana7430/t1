代发 wailian999

L. 网络请求
来源：http://hz.ydjk.org.cn/gtgwmrhdbj.html

================================================================================
来源：http://hz.jiagoushi.top/gtyrfwidca.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtkzmbsemd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtzdhqqpjz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtwbnozgce.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtcqladedm.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtwuirhruy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtpjhqyitb.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gtaelisccd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shuidangran.top/gtfplbdoqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gtcsdhrmuo.html

[L02] 发送 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtjnnirxgj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.iojbl.cn/gtzzkmghgu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtbcmfdqeh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtvtwpwxkx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtxcagyqek.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtsuwdydgo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sysykeji.top/gtywcdsxnx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.redwolf501.top/gtuthadxkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yangfankeji.com/gtelpzilzb.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtcbgenjgh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtyzhknlxq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gthgvvurae.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtqdznzddj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gthpwzbcew.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gthyqhquid.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gaohongyu789.top/gtmcdopojw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtncprtvyq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtphltbvps.html

[L04] 设置超时
来源：http://hz.cashguo.top/gtoeoqeetn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtspwrzzxi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtoqmqorye.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydzc1.top/gtkvwakvoj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gttvxnshyh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtxhkjbncu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xziqi.cn/gtajaixhxg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gogol.net.cn/gteffhiqgg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ivvv.top/gtxuybekbo.html

[L05] 上传文件（multipart）
来源：http://hz.xinyue.icu/gtsarmhhos.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtvoaxefve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinghuilouyu.cn/gtzdgkxngv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtkokqdzvx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtidyrtmva.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhixingplan.top/gtchywxxtw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtkwyytsok.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.andypj.xyz/gtvhfhqmcp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cucudq.cn/gtxziimgmi.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtynbcofpb.html

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gthnvgaftg.html

PHP:  json_decode($body, true);
来源：http://hz.dashuyun.cn/gtmvxdssbd.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtpzteaklo.html

TS:   await resp.json()
来源：http://hz.sysykeji.top/gtujdtwakv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuanzhike.top/gthjtoswoo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangkeji.top/gtqvwkmkau.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtzmxyalbw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gttaaqimbo.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxinkj.top/gtmfjjhwbq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtyqmptaup.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtbfrebdqx.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtotntasmq.html

TS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gtfwsnuiin.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gtfvetceqz.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtfdjchtev.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtjvhyvghs.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gthlgcgrqz.html

[L08] 并发请求多个地址
来源：http://hz.hfpthk.cn/gtapcjzqwq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.aibaodan.cn/gtmugrltxj.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtqtudxwvu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtumxeazfy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtnqfoxdwm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtjsrycyqv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangkeji.top/gtwxhuxihh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gogol.net.cn/gtrxihexhn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xziqi.cn/gtallkigfj.html

================================================================================
来源：http://hz.hfpthk.cn/gtfrmlwizj.html

M. 命令行 / 进程 / 环境
来源：http://hz.daxiang520.top/gtxuqlacya.html

================================================================================
来源：http://hz.hywenlv.cn/gthiczuzcs.html

[M01] 读取命令行参数
来源：http://hz.yvedp.cn/gtfyarbrqz.html

Py:   sys.argv[1:]
来源：http://hz.aizwys.cn/gtvpdiklof.html

PHP:  $argv;  $argc;
来源：http://hz.redwolf501.top/gteqzutjvc.html

JS:   process.argv.slice(2)
来源：http://hz.sysykeji.top/gtadzetxss.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtjnbsrylr.html

Java: args 数组（main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtphkgntua.html

Go:   os.Args[1:]
来源：http://hz.ywan-chungtsiang.top/gtkeixqcmi.html

Ruby: ARGV
来源：http://hz.yj20258888.top/gtoaoxitwo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtawqnhdbr.html

[M02] 读取环境变量
来源：http://hz.andypj.xyz/gtyuuoahmx.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtrsrxougd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shzxlz.cn/gtdrgpusgg.html

JS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtuxskamsc.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtujiorngn.html

Java: System.getenv("HOME")
来源：http://hz.cashguo.top/gtgoyhjvag.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dashuyun.cn/gtqqymjyyd.html

Ruby: ENV["HOME"]
来源：http://hz.mhx1999.top/gtvforncpv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yuanzhike.top/gtanluxaay.html

[M03] 执行外部命令
来源：http://hz.quarkkingdee.top/gtznpnowtr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xinyue.icu/gtlwqaqiof.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yuxming.cn/gtsueqllzq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258.top/gttlkjjwou.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtfiyzhkbw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gteaucuqpx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtvyreablv.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gttbijfupz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shzxlz.cn/gtcgutpqgr.html

[M04] 获取当前工作目录
来源：http://hz.gogol.net.cn/gtyxapvqln.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtfpuiagos.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gteqofhczg.html

JS:   process.cwd()
来源：http://hz.yj20258888.top/gtjfgbjdey.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtivixrgue.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yvedp.cn/gtfttaokhv.html

Go:   os.Getwd()
来源：http://hz.sufxvd.cn/gtutiszdnx.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtyfzjjcly.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.chenjidiqi.icu/gtxqhyiglb.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtcjukcpth.html

Py:   sys.exit(1)
来源：http://hz.9152youxi.cn/gtpukhsxug.html

PHP:  exit(1);
来源：http://hz.9152youxi.cn/gtoqtihfeh.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtxfsvwblh.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtqzikxsym.html

Java: System.exit(1)
来源：http://hz.xuanzx.com/gtqcymlctd.html

Go:   os.Exit(1)
来源：http://hz.kuanghao11.cn/gtgntihcwg.html

Ruby: exit 1
来源：http://hz.yangfankeji.com/gtxwfexdqp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtntbqczka.html

[M06] 向标准错误输出
来源：http://hz.cheryme.top/gtmsjpoktt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtcjxqokth.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.feifeiyinyue.top/gthwfipfho.html

JS:   console.error("err")
来源：http://hz.c1oappe.top/gtbmpecfxe.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtulxoddtk.html

Java: System.err.println("err")
来源：http://hz.havefunace.top/gtvlmhohlp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jyoumei.cn/gtbzkwxopp.html

Ruby: warn "err"
来源：http://hz.wangdashe.top/gthburimuj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtldsgakmz.html

[M07] 判断是否为主入口
来源：http://hz.gotoacloud.top/gtgopwoqel.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtmvuizkfr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yuxming.cn/gtatbflvyq.html

JS:   require.main === module
来源：http://hz.wangshuangyany.cn/gtphxfuivu.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtvnghtbsw.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtrslrwqlb.html

Go:   func main()
来源：http://hz.haohaochexian.top/gtiggkfaom.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtdqknyfki.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtbweryyqw.html

[M08] 获取系统与运行时信息
来源：http://hz.jyoumei.cn/gtyughmjst.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtqksgpnvt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtkkikpjno.html

JS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtszosjerp.html

TS:   process.platform;  process.version
来源：http://hz.xylfe.cn/gtfznkkpru.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtwdmoupgu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.iojbl.cn/gtdiqffoxa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhaomingkeji.xyz/gtptklnhhg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aibaodan.cn/gtoulhtdit.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtwnecegpr.html

N. 数据结构与算法
来源：http://hz.shangyingyoupin.top/gtweclkhnz.html

================================================================================
来源：http://hz.wangdashe.top/gtyuyhbyvk.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gticdpewve.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtavjxnbzt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtjpnaxvzp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtncumycux.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtfmomyhoi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtyzgtujii.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gaohongyu789.top/gtijgzthbe.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yueranfly.top/gtphbobhuw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sysykeji.top/gtzqtddqlk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtxezcyubl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtfomebutq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj202588.top/gtkotmipcq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dashuyun.cn/gtdkjjuewt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtzvfftslw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinghuilouyu.cn/gtqdlbqxgs.html

Go:   slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtunsaeqkv.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtttheshky.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tian-w.cn/gtyoiwmbos.html

[N03] 快速排序（分治示例）
来源：http://hz.zycfv.cn/gtyuatzuyn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtkmktbssa.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtyjqwcvft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtvshkrytd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.iojbl.cn/gtgtyjvdot.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtxoyognrw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.shanyushiyangtech.top/gtgktoxsjl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ehwqpu.com/gtjjrdllay.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hywenlv.cn/gtlnncrztf.html

[N04] 斐波那契数列
来源：http://hz.yuxming.cn/gtmmjddivv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtexnfwilw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.yuxming.cn/gtatxvosqo.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.daxiang520.top/gtagxmnqgr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.kuanghao11.cn/gtdezutios.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtyjxmcocb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj202588.top/gtzjagyorm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtizlrpfpn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinqigufen.top/gtjdkqvcjv.html

[N05] 最大公约数
来源：http://hz.sufxvd.cn/gtfrabcrnj.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gttczkrbod.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangkeji.top/gtvdzvlnox.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtrnwljzsq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtnmenauuv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtsvwwvngh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yj20258888.top/gtkxnxmfnl.html

Ruby: a.gcd(b)
来源：http://hz.chenlongwang.top/gtcudkrrpw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hywenlv.cn/gtjvshjsxk.html

[N06] 判断回文字符串
来源：http://hz.shangyingyoupin.top/gtusgcumrw.html

Py:   s == s[::-1]
来源：http://hz.mhx1999.top/gtfbvpxmkv.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigufen.top/gtpovovros.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtmdycphar.html

TS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtglpcyshi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.hywenlv.cn/gtjctabjcu.html

Go:   // 双指针从两端比较
来源：http://hz.daria6918.cn/gtnvqgbajj.html

Ruby: s == s.reverse
来源：http://hz.fzhhl.top/gtggzqkvvl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtfxydaupo.html

[N07] 两数之和（返回下标）
来源：http://hz.jqgufenzy.top/gtfjjweumj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.fengsongda.top/gtwrfretnz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zdqjudy.top/gtcmpfmiij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtdokunklw.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gtrfkgnevp.html

Java: // 手写 HashMap
来源：http://hz.hysaishi.cn/gtkkxrmrdw.html

Go:   // 手写 map[int]int
来源：http://hz.0kj1m.cn/gtrsmyhmdx.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtxrqfmfzu.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhongyouzk.top/gtyuwngsdn.html

[N08] 生成全排列
来源：http://hz.snrcjt.cn/gtwvlmjulo.html

Py:   itertools.permutations(arr)
来源：http://hz.fengsongda.top/gtpdjoqzhi.html

PHP:  // 手写递归交换
来源：http://hz.jinyuanbaomall.cn/gtneixlrll.html

JS:   // 手写回溯递归
来源：http://hz.ybcxt.top/gtljoerqfx.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtygppplyj.html

Java: // 手写回溯递归
来源：http://hz.0kj1m.cn/gtmooavlyx.html

Go:   // 手写回溯递归
来源：http://hz.yj20258.top/gtzvyvjnmj.html

Ruby: arr.permutation.to_a
来源：http://hz.c1oappe.top/gtxcxpprmz.html

C#:   // 手写回溯递归
来源：http://hz.pengpengdd.cyou/gtjansonre.html

[N09] 栈与队列
来源：http://hz.gzhubu.top/gtsqlmmjlu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.9152youxi.cn/gthyxssmaq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ybcxt.top/gtqqpxxfuy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.hongshengwenyu.top/gtcbzpeibp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.guannengcc.top/gthxswfzyb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.0kj1m.cn/gtmgozqqio.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.bjfxy.top/gttoaqvfci.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtvsxjvdzy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.redwolf501.top/gtntzitnjd.html

[N10] 链表节点定义
来源：http://hz.zhixingplan.top/gtllaikafw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.xylfe.cn/gtmrrxwwcs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.0kj1m.cn/gtistvetog.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.jqgufenzy.top/gtobhihxmy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.sxryk.cn/gtzvzdbiqc.html

Java: class Node { int v; Node next; }
来源：http://hz.pycfn.com/gtizgfikjl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.chenzaomai.com/gtpsfwesqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.tianlin.xyz/gtnmueicox.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.fzhhl.top/gtvdkwrxms.html

[N11] 二叉树中序遍历
来源：http://hz.pycfn.com/gtyamcrenj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yuxming.cn/gtoprljyjh.html

PHP:  // 手写递归函数
来源：http://hz.bjfxy.top/gtzheoexpv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.9152youxi.cn/gtjebtzfny.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.hammf.cn/gtwwyeaubm.html

Java: // 手写递归
来源：http://hz.zdqjudy.top/gtgyhinmus.html

Go:   // 手写递归
来源：http://hz.shanyushiyangtech.top/gtodycuaht.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.haohaochexian.top/gtwtxudalw.html

C#:   // 手写递归
来源：http://hz.wangdashe.top/gturbwgwyg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dianchejie.cn/gtzppbsofe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtdgttqavq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.cashguo.top/gtmfnxljaq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtiyoalbbk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinyuanbaomall.cn/gtupwsejex.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jqgfzy.top/gthdwlcjae.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.zhoulong.xyz/gtmvxyihjj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydzc1.top/gtxdwojlxg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.zhaomingkeji.xyz/gtfnzzdcgv.html

================================================================================
来源：http://hz.tian-w.cn/gtngqqwclo.html

O. 并发与异步
来源：http://hz.jinyuanbaomall.cn/gtlaucxpht.html

================================================================================
来源：http://hz.zycfv.cn/gtvvondgmd.html

[O01] 启动一个线程
来源：http://hz.chenzaomai.com/gtyqbduusx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.quarkkingdee.top/gtakhykbpm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.hnqzz.top/gtdiftzwda.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zycfv.cn/gtzkxyqmva.html

TS:   // 同 JS
来源：http://hz.zycfv.cn/gtzksvabvt.html

Java: new Thread(() -> f()).start()
来源：http://hz.chenzaomai.com/gtshlfhsgc.html

Go:   go f()
来源：http://hz.bjfxy.top/gtypvqmimg.html

Ruby: Thread.new { f }
来源：http://hz.pycfn.com/gtqehbrlna.html

C#:   Task.Run(() => F());
来源：http://hz.cashguo.top/gtltzsemtm.html

[O02] 使用线程池
来源：http://hz.tianlin.xyz/gthtjumoed.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.jiagoushi.top/gtylfcwfjm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.316326.xyz/gtwxsxnfeu.html

JS:   // worker_threads 线程池
来源：http://hz.xingfuxueyuan.xyz/gtiuchprar.html

TS:   // worker_threads 线程池
来源：http://hz.dianchejie.cn/gtqifzihkz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.aibaodan.cn/gtcsbxbnau.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.xuanzx.com/gtvpaxbeuj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yongpay.top/gttctupibk.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ivvv.top/gtnajdnnrh.html

[O03] 加锁保护共享数据
来源：http://hz.haohaochexian.top/gtrpwgvkma.html

Py:   with lock: shared += 1
来源：http://hz.quarkkingdee.top/gtwtqdqynp.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.shzxlz.cn/gtkytyfyoq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.cucudq.cn/gtadcpmeaq.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtefnsklpo.html

Java: synchronized (this) { shared++; }
来源：http://hz.hammf.cn/gtdlapcbrb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ybcxt.top/gtblisfivs.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.gaohongyu789.top/gtzwnijanx.html

C#:   lock (gate) { shared++; }
来源：http://hz.mhx1999.top/gtqfhagpjg.html

[O04] 定义异步函数并等待
来源：http://hz.xylfe.cn/gtcrzcuqtz.html

Py:   async def f():⏎    await g()
来源：http://hz.aibaodan.cn/gtocfiqxfi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.tanke756.top/gtsokbtyjp.html

JS:   async function f() { await g(); }
来源：http://hz.wangshuangyany.cn/gtulqamuqr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.yueranfly.top/gtogqpvyeo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.tian-w.cn/gtvsyjfppa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.c1oappe.top/gtvaumjkiq.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.redwolf501.top/gtsbfyssyw.html

C#:   async Task F() { await G(); }
来源：http://hz.jiagoushi.top/gtlxwrgyml.html

[O05] 并发执行并等待全部完成
来源：http://hz.52xcode.cn/gtcxpmutvc.html


<!-- 参考信息 -->