代发 wailian999

L. 网络请求
来源：http://hz.316326.xyz/gtfehnoraj.html

================================================================================
来源：http://hz.redwolf501.top/gtxtvdjjkf.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtsimmfknv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinyuanbaomall.cn/gtpidwrkjb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtcngmjolb.html

JS:   await fetch(url)
来源：http://hz.snrcjt.cn/gtgekjfrie.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gteisqjinq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gtzdqhtxcu.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtnelhvqmw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtpkzpljtr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gtzskuedju.html

[L02] 发送 POST JSON
来源：http://hz.kuanghao11.cn/gtexuzjsov.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtetjlnzud.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.iojbl.cn/gtuvwpeylm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtcvhgismw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtdvaqvlqj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.meibo888.top/gtzhgcaeer.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yangfankeji.com/gtgsonltme.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj20258888.top/gthpyjxank.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.andypj.xyz/gtljmwiaxd.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtahhhowjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtoashvmru.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenjidiqi.icu/gtmydqhwaz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtrkcvhitn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gzhubu.top/gtsbtllcmt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtfegwbhgd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tanke756.top/gtteedmpux.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.pengpengdd.cyou/gtpsvgqgwt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtddygorua.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gthiuwtmlj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtwsqsedzt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtmtptpdvx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtmufqcwwy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtnigfmmua.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtibxithkz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtutdtrdzy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jianghu66.top/gtulpnuvxb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258.top/gtjmzenmzc.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtuqusazfa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtkstvoacw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yongpay.top/gttnxsufnu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtmtdekrpf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtwfohdcxv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hysaishi.cn/gtzgqdgimb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jianghu66.top/gtidzftwwx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtcoyqerwt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhongyouzk.top/gthhbwtpsp.html

[L06] 解析响应为 JSON
来源：http://hz.chenlongwang.top/gtxghaksha.html

Py:   resp.json()
来源：http://hz.zhixingplan.top/gtapbgftab.html

PHP:  json_decode($body, true);
来源：http://hz.zdqjudy.top/gtdfgkuszk.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtwiwqxbjd.html

TS:   await resp.json()
来源：http://hz.ywan-chungtsiang.top/gtnxywvmqz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cucudq.cn/gtntvywhgt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gtpejmneji.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtslzadbri.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ybcxt.top/gtvhseilzm.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtzcsbgrks.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtshtqhqoc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtbtpdryzu.html

JS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gturdbrgzo.html

TS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtbhcyuxah.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gtiudgjmub.html

Go:   resp.StatusCode
来源：http://hz.cqqwz.cn/gtmtglyqnm.html

Ruby: resp.code.to_i
来源：http://hz.zhijiandao.cn/gtibvrxdkw.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gtlxhjgwlr.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtjfwafeir.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtllrwkleu.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtvncpgpgc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtbotflfku.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gteuxehroa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhixingplan.top/gtfcvawjyy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtuzhmcsfr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.pycfn.com/gtsgcfxkis.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtchtqewgn.html

================================================================================
来源：http://hz.52xcode.cn/gtozdmxnuk.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtxpymybtp.html

================================================================================
来源：http://hz.xziqi.cn/gtzaeiucqj.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtnwbkysnk.html

Py:   sys.argv[1:]
来源：http://hz.birdmap.top/gtefckehiv.html

PHP:  $argv;  $argc;
来源：http://hz.haohaochexian.top/gtxojhuztm.html

JS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtxttiqaiq.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtmmsoylas.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxinkj.top/gtpnwjzytw.html

Go:   os.Args[1:]
来源：http://hz.haohaochexian.top/gtgtbcjtgr.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtztbewrtm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtrsxviuhc.html

[M02] 读取环境变量
来源：http://hz.pycfn.com/gtgzpvwopp.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtvjafiigp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tianlin.xyz/gtdljhyncc.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtqbbmzbcs.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gtvsyphbwm.html

Java: System.getenv("HOME")
来源：http://hz.zhoulong.xyz/gterqkdwik.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jlsjyb.cn/gtvnxtikmr.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtrkbszbzo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ppjwa.cn/gtmbztibbc.html

[M03] 执行外部命令
来源：http://hz.9152youxi.cn/gtvjbcegbx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhiwuduotai.top/gtpxtpesjg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtyrklmwxz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtlebzhzoo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtdlsaqqam.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtefqqbdga.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtjiyhlxha.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtrodpedfr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xinyue.icu/gtxvkmaivp.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtourehfhu.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtbhlfodao.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtsdxsdywb.html

JS:   process.cwd()
来源：http://hz.jqgfzy.top/gtabqdvvjp.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtdnayxvyx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cdnleiting.top/gtxhwpltpo.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtlaukdgar.html

Ruby: Dir.pwd
来源：http://hz.gotoacloud.top/gtnhxuuqtg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cucudq.cn/gtbpnssskv.html

[M05] 设置退出码
来源：http://hz.hysaishi.cn/gtsaoglbyo.html

Py:   sys.exit(1)
来源：http://hz.shanyushiyangkeji.top/gttuautzjk.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gtnkyakeuq.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtwqecvxdo.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtavifdspb.html

Java: System.exit(1)
来源：http://hz.cheryme.top/gtmirkswzf.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtfnqumnhw.html

Ruby: exit 1
来源：http://hz.chenzaomai.com/gtgaxgbdwi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtduyjnpur.html

[M06] 向标准错误输出
来源：http://hz.xuanzx.com/gttcstlkeh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtrbjcmcaz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gtzvpctjtb.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtcqzpicju.html

TS:   console.error("err")
来源：http://hz.meibo888.top/gtmfrjojfw.html

Java: System.err.println("err")
来源：http://hz.zycfv.cn/gtluhjvkse.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtotcpadca.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtjhmldqra.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtsvikxeil.html

[M07] 判断是否为主入口
来源：http://hz.meibo888.top/gttjslidox.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtnuilkzfd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guowangkeji.top/gtgimyywsg.html

JS:   require.main === module
来源：http://hz.fzhhl.top/gtybracfkk.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtzkbylmxa.html

Java: public static void main(String[] args)
来源：http://hz.ppjwa.cn/gthrhzuxoj.html

Go:   func main()
来源：http://hz.hfpthk.cn/gtwpkgmyqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxinkj.top/gtibtfbyei.html

C#:   static void Main(string[] args)
来源：http://hz.snrcjt.cn/gthntexzlg.html

[M08] 获取系统与运行时信息
来源：http://hz.yj202588.top/gtoaoblsyt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtvzlnqqgy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.andypj.xyz/gtybdbfrpv.html

JS:   process.platform;  process.version
来源：http://hz.iojbl.cn/gtpjssaatd.html

TS:   process.platform;  process.version
来源：http://hz.zhiwuduotai.top/gtcwcaehzp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xziqi.cn/gtwbhnbdji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yongpay.top/gtoxuenjwn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xuanzx.com/gtcsszwxeg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.snrcjt.cn/gtnnrmaypo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdkwcptzc.html

N. 数据结构与算法
来源：http://hz.xziqi.cn/gtmhazumxv.html

================================================================================
来源：http://hz.jyoumei.cn/gtthpcjtcq.html

[N01] 二分查找（有序数组）
来源：http://hz.chenlongwang.top/gtzqbrlkut.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.c1oappe.top/gtxeoqlrwx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.iojbl.cn/gthvhehtst.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtkgruxopn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dashuyun.cn/gtzczwgzsi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yongpay.top/gtamlejnxv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgfzy.top/gteahdoacm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jlsjyb.cn/gtnoeqcrjr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtxqgkogyx.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtjkkmwhvf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtnuyutsyb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.sweek.top/gtoujhmroo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtfqvadwvs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtwtpqaxwe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtnuhmagya.html

Go:   slices.Sort(arr)
来源：http://hz.zhengqikj.top/gtwtlmbnyd.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtpuegfpds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.svipenyu.cn/gtswpjucoj.html

[N03] 快速排序（分治示例）
来源：http://hz.tianlin.xyz/gtqiqtkpbc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.aibaodan.cn/gtprmhlfax.html

PHP:  // 递归实现，或用 usort
来源：http://hz.tian-w.cn/gtfetkgpiy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtrwpbhqnq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtkrothjwp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ywan-chungtsiang.top/gtntiwssvg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gtlfabvsxi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xuetiantiany.cn/gtwxkcuxee.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtkwxuicxd.html

[N04] 斐波那契数列
来源：http://hz.zhongyouzk.top/gttkppqptm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtpmnxgpub.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtznxagunf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtuvychjrd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sxryk.cn/gtcqakkodm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zhoulong.xyz/gtqjpkknik.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.daxiang520.top/gtqtvhpirl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtbmxacyzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.mhx1999.top/gtitysaulr.html

[N05] 最大公约数
来源：http://hz.chenjidiqi.icu/gtjoxgppjp.html

Py:   math.gcd(a, b)
来源：http://hz.guannengcc.top/gtaandysjc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtldxrlino.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhiwuduotai.top/gtfdckegod.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guannengcc.top/gtpvdrdvfn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.wangdashe.top/gtasqcwcgl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gtxrkhpskx.html

Ruby: a.gcd(b)
来源：http://hz.fzhhl.top/gtysehipxq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtjyduolak.html

[N06] 判断回文字符串
来源：http://hz.yongpay.top/gtmzoyuzmz.html

Py:   s == s[::-1]
来源：http://hz.yuanzhike.top/gtqxisktuu.html

PHP:  $s === strrev($s);
来源：http://hz.yuanzhike.top/gtpnywaqsp.html

JS:   s === [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtimlshxke.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cashguo.top/gtdybokmvf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shzxlz.cn/gtedmjyahd.html

Go:   // 双指针从两端比较
来源：http://hz.aizwys.cn/gtpkkatugk.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtxbeuwclq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtzmuycxat.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gthkfvswcz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daxiang520.top/gtneomglcs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hfpthk.cn/gtkymoxoay.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xuanzx.com/gtkaawpiaf.html

TS:   // 手写 Map<string, number>
来源：http://hz.pengpengdd.cyou/gtafmkzymf.html

Java: // 手写 HashMap
来源：http://hz.yongpay.top/gtyyewphng.html

Go:   // 手写 map[int]int
来源：http://hz.daria6918.cn/gtvvqkcttx.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtyiwsrfkj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yongpay.top/gtmjxmpoth.html

[N08] 生成全排列
来源：http://hz.meibo888.top/gthrwttjqh.html

Py:   itertools.permutations(arr)
来源：http://hz.fzhhl.top/gtuihkvfjo.html

PHP:  // 手写递归交换
来源：http://hz.daxiang520.top/gtwhrhadmh.html

JS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtocmkomcw.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtcyiswetm.html

Java: // 手写回溯递归
来源：http://hz.yuanzhike.top/gthdzxtcpa.html

Go:   // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtwkvdyljv.html

Ruby: arr.permutation.to_a
来源：http://hz.tianlin.xyz/gtgqgsekli.html

C#:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtmcxabcor.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtonlzaihj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hywenlv.cn/gtfxsgjtiz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.fengsongda.top/gteriebaiz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zycfv.cn/gtszxrdfxw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.yueranfly.top/gtwsvbcxbs.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.316326.xyz/gtbzkmfpob.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhijiandao.cn/gtslpcavpe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.yonumen.top/gtltuuyfup.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xuanzx.com/gtrulqxpdk.html

[N10] 链表节点定义
来源：http://hz.yuanzhike.top/gtoewzowvz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yongpay.top/gtwxbzdrcv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hammf.cn/gtwtfyzkvg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.9152youxi.cn/gtwcnexbzm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.9152youxi.cn/gterkvrrsj.html

Java: class Node { int v; Node next; }
来源：http://hz.jinqigufen.top/gtwhumhqzs.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.xuanzx.com/gtahyspxzg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.sufxvd.cn/gtzioiwpqu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenlongwang.top/gtqfsfrmui.html

[N11] 二叉树中序遍历
来源：http://hz.smart0.xyz/gteroehcks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nanxuanxn.top/gtezjofalj.html

PHP:  // 手写递归函数
来源：http://hz.jqgufenzy.top/gtsszmsvgy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtrvfpqfez.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zhiwuduotai.top/gtynvugnck.html

Java: // 手写递归
来源：http://hz.yueranfly.top/gtlviyiecz.html

Go:   // 手写递归
来源：http://hz.wangshuangyany.cn/gtwvbjcacu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.bjfxy.top/gtwmblymfi.html

C#:   // 手写递归
来源：http://hz.cdnleiting.top/gttljkwgwy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.dashuyun.cn/gtddhddtlq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ywan-chungtsiang.top/gtajfedzgg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.shanyushiyangkeji.top/gtuzluouba.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.jinghuilouyu.cn/gtiuktbqor.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtzlphbunr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yj20258.top/gtjufjhmbq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.meibo888.top/gtbmhxgsty.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.sufxvd.cn/gttjwwgnte.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.tian-w.cn/gtkefhuqwf.html

================================================================================
来源：http://hz.yj20258.top/gtcuuemjar.html

O. 并发与异步
来源：http://hz.jinqigfzy.top/gtcidfawyy.html

================================================================================
来源：http://hz.redwolf501.top/gtzriklspr.html

[O01] 启动一个线程
来源：http://hz.nanxuanxn.top/gtoxtujvap.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cashguo.top/gtycqpjnzd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yongpay.top/gtulmyasbt.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.0kj1m.cn/gtdfdhapfg.html

TS:   // 同 JS
来源：http://hz.ppjwa.cn/gtyeuntthg.html

Java: new Thread(() -> f()).start()
来源：http://hz.9152youxi.cn/gtnxouujqp.html

Go:   go f()
来源：http://hz.havefunace.top/gtqaphiumf.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gtwexvgyok.html

C#:   Task.Run(() => F());
来源：http://hz.52xcode.cn/gttfjirojx.html

[O02] 使用线程池
来源：http://hz.cashguo.top/gtjnblpilb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yj20258888.top/gtilgnhvxp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pycfn.com/gtstjjvpqv.html

JS:   // worker_threads 线程池
来源：http://hz.zhoulong.xyz/gtgxfvzsew.html

TS:   // worker_threads 线程池
来源：http://hz.yj202588.top/gtlcztohrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.zhiwuduotai.top/gtrnychbpg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtonjapjdi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.gaohongyu789.top/gtzlpqghfn.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.bjfxy.top/gtmsgxupmk.html

[O03] 加锁保护共享数据
来源：http://hz.ppjwa.cn/gtxxkqtnep.html

Py:   with lock: shared += 1
来源：http://hz.dianchejie.cn/gtkekfllvt.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.sxryk.cn/gtolrvlhvj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.yuxming.cn/gtkmoevach.html

TS:   // 同 JS
来源：http://hz.pengpengdd.cyou/gtayayzrap.html

Java: synchronized (this) { shared++; }
来源：http://hz.guowangkeji.top/gtecgxalrv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.daxiang520.top/gtwmvievld.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.ivvv.top/gtvyfmumfl.html

C#:   lock (gate) { shared++; }
来源：http://hz.hfpthk.cn/gtworgommr.html

[O04] 定义异步函数并等待
来源：http://hz.9152youxi.cn/gtqsyvwcnr.html

Py:   async def f():⏎    await g()
来源：http://hz.zhoulong.xyz/gtkqlfqnpn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.hfpthk.cn/gtfaliafdo.html

JS:   async function f() { await g(); }
来源：http://hz.iojbl.cn/gtfhtwukcp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.jyoumei.cn/gtwbroeevz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.xziqi.cn/gtbvdwssuf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.hnxiangtu.top/gtdfcjeilx.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.gzhubu.top/gtlffrfciz.html

C#:   async Task F() { await G(); }
来源：http://hz.mhx1999.top/gtlafvgqfw.html

[O05] 并发执行并等待全部完成
来源：http://hz.jinqigufen.top/gtsladeeyo.html


<!-- 参考信息 -->