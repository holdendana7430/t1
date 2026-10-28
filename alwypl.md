代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gteihtjauk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aibaodan.cn/gtfjrqitkb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtzkygluyr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtngcvhhzq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.haohaochexian.top/gtqlzqbmxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangshuangyany.cn/gtazypifzi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtkgysbbjw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtbjlpxnog.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtrplhwlbd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.tanke756.top/gtbruoufri.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xylfe.cn/gtjxybslzh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtytvxcryu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtmidyjqve.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangtech.top/gtzpddyykv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtnpsxfchp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gthnxlhvcf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtzaqqgmsh.html

[L04] 设置超时
来源：http://hz.jyoumei.cn/gtfsdvdbfb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.vqdsnc.cn/gtkukbjhmo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuanzhike.top/gtnqpqsouz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtmtxbuwie.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtcfefddbv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gaohongyu789.top/gtubffptwa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.havefunace.top/gtrzvkokjc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtxbjhyjig.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtzrojfiyr.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtqfmyfczz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yueranfly.top/gtdxkybdtj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.mhx1999.top/gtdxzpurwj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtdqjksigm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtljsuwqau.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xylfe.cn/gtapanohnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtzkwgkocu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhoulong.xyz/gtmjbzofuq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinghuilouyu.cn/gtydlzlaxz.html

[L06] 解析响应为 JSON
来源：http://hz.xylfe.cn/gtoxdhqdqn.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gtielhdkby.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtdvymojfj.html

JS:   await resp.json()
来源：http://hz.c1oappe.top/gthquedwpd.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gtlxrzdqoj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtrzpdpate.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gzhubu.top/gtmgjxbbhk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtgsozpmhg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtqkzqsxnw.html

[L07] 处理 HTTP 状态码
来源：http://hz.gotoacloud.top/gtizruadan.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ehwqpu.com/gthnlfdolu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daria6918.cn/gtgphhroce.html

JS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtsgbvvpcp.html

TS:   resp.ok;  resp.status
来源：http://hz.cqqwz.cn/gtyzwzgpwb.html

Java: resp.statusCode()
来源：http://hz.nanxinkj.top/gtanogdfhj.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangkeji.top/gtzfqbghui.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtmjcppxah.html

C#:   (int)resp.StatusCode
来源：http://hz.zhongyouzk.top/gtjyibsgyd.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtdteojatb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtzqpgathp.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj202588.top/gtifpefeqz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtbgdbwjgh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cdnleiting.top/gtayjjfekh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuetiantiany.cn/gtbfcwkvjm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtpcsinisi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtnakujesn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtyudgsjll.html

================================================================================
来源：http://hz.jqgufenzy.top/gttapyserw.html

M. 命令行 / 进程 / 环境
来源：http://hz.birdmap.top/gtqvyresqm.html

================================================================================
来源：http://hz.ivvv.top/gtznfessbx.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtyxhwlifd.html

Py:   sys.argv[1:]
来源：http://hz.hongshengwenyu.top/gtefmsniah.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtxzejzacr.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtsglkorgv.html

TS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtwdgbfxqd.html

Java: args 数组（main 方法参数）
来源：http://hz.9152youxi.cn/gtnbiahbjc.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gttuitcguz.html

Ruby: ARGV
来源：http://hz.gzhubu.top/gtyryafwaj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtqnlvsish.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtrcmyrtfn.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgfzy.top/gtezpyzjpk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtdifvvoup.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtcxhwtiyn.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtpveapejk.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtkuwjwlwh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtrnxeljcx.html

Ruby: ENV["HOME"]
来源：http://hz.tian-w.cn/gtgndmxhpi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gtvkqaukdm.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtijcgibnt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xingfuxueyuan.xyz/gtqsnnwygy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jiagoushi.top/gtinvyvnvc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtvwqkpmln.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gttzicoixk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hysaishi.cn/gtuymqcmmd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigufen.top/gtfumxzplm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gthtczxyws.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtypkaljli.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtanpgqtbg.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gtababoaio.html

PHP:  getcwd();
来源：http://hz.cheryme.top/gtytkrrvju.html

JS:   process.cwd()
来源：http://hz.wangdashe.top/gtptidmgpl.html

TS:   process.cwd()
来源：http://hz.redwolf501.top/gtyuckicgs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.haohaochexian.top/gtxqqckmbc.html

Go:   os.Getwd()
来源：http://hz.shangyingyoupin.top/gtjzxpgwyp.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtctrwsakq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtfnvpjqal.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtqirjdwpg.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtcagvcdmp.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gtbqduloat.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtftaveavf.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtxjmxnhsw.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtbftjtlyc.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtfiueocdx.html

Ruby: exit 1
来源：http://hz.zhengqikj.top/gtqceoxvwg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtkrntytcc.html

[M06] 向标准错误输出
来源：http://hz.fengsongda.top/gtmjmnohxm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuxming.cn/gtcxjcysoh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtjailibpa.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtjiarfbon.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtgxluhjzk.html

Java: System.err.println("err")
来源：http://hz.redwolf501.top/gttpqmufzp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gttanwluus.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtwdlneuof.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hysaishi.cn/gtpamkqjcv.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtjshtamkw.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtfwtyisft.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sufxvd.cn/gtzvvsobef.html

JS:   require.main === module
来源：http://hz.chenzaomai.com/gtrbbmgsvz.html

TS:   require.main === module
来源：http://hz.smart0.xyz/gtzvhfgisx.html

Java: public static void main(String[] args)
来源：http://hz.xinyue.icu/gtyuubacaw.html

Go:   func main()
来源：http://hz.sweek.top/gtjlyrpnwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.dashuyun.cn/gtltbbmgxp.html

C#:   static void Main(string[] args)
来源：http://hz.hnxiangtu.top/gtrtcrhads.html

[M08] 获取系统与运行时信息
来源：http://hz.wangshuangyany.cn/gtztebsmkt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.sweek.top/gtzhjwwgyv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fzhhl.top/gtnkmguzhy.html

JS:   process.platform;  process.version
来源：http://hz.gzhubu.top/gtqrlmltsu.html

TS:   process.platform;  process.version
来源：http://hz.tian-w.cn/gtgeiziqup.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tian-w.cn/gtvgevqvsr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtqipedmnu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gtkaywtjrc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258888.top/gtppzlosrq.html

================================================================================
来源：http://hz.zhoulong.xyz/gttbiowsqb.html

N. 数据结构与算法
来源：http://hz.shanyushiyangtech.top/gtuavxtflp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtuvodcxsu.html

[N01] 二分查找（有序数组）
来源：http://hz.pengpengdd.cyou/gtkmmrtilz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtddwbcpad.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gtrhkzhwms.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtlkuskdod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fengsongda.top/gtnzowmuns.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtviuyaerd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.vqdsnc.cn/gtzwijqvbv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhoulong.xyz/gtveogmjmz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtjjojxutr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtfzbowsob.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fzhhl.top/gtwjxbyphw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hywenlv.cn/gtllxppeza.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtzkrrdtpq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ywan-chungtsiang.top/gtgginpnjs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yj20258888.top/gtaewdkxpc.html

Go:   slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtpdvydlfl.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gthyqirbwf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.gotoacloud.top/gtwtepccgd.html

[N03] 快速排序（分治示例）
来源：http://hz.yangfankeji.com/gtlnzdntsh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtwvvjbmbs.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nwbrower.top/gtfujfsmrs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtnazxgrze.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhongyouzk.top/gtyevdsiac.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.cucudq.cn/gtpvbrztyp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.dianchejie.cn/gtxejplmcd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guowangkeji.top/gtcjawkpjf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj20258888.top/gtjffueapk.html

[N04] 斐波那契数列
来源：http://hz.ybcxt.top/gtokriebyo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtxieyalie.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.c1oappe.top/gtxkioercl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtsdmbfjiv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gteuzuydea.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.vqdsnc.cn/gtgwkngheq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yanxiufei.cn/gtidrzkfqq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ivvv.top/gtbqpgcear.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.daxiang520.top/gtwtpijfqe.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtpwkcrlwu.html

Py:   math.gcd(a, b)
来源：http://hz.gzhubu.top/gtfadddzui.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gaohongyu789.top/gtxmpcyhaf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.feifeiyinyue.top/gtnxihmbtr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtuuybsthg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.nanxuanxn.top/gtzzxmnxxr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hywenlv.cn/gtidnvzacf.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtkafngzao.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.iojbl.cn/gtgmepcvfv.html

[N06] 判断回文字符串
来源：http://hz.gogol.net.cn/gtdelzxzxl.html

Py:   s == s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtjrounvek.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtbzmmeihu.html

JS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtputrwynq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtdykupuzp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ydjk.org.cn/gtnjxfftni.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtyjwdszjk.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtmgejiunv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gtojvljjch.html

[N07] 两数之和（返回下标）
来源：http://hz.cucudq.cn/gtuznpagki.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.ehwqpu.com/gtkcuogamp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xingfuxueyuan.xyz/gtlohkthrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jyoumei.cn/gterefqkjd.html

TS:   // 手写 Map<string, number>
来源：http://hz.ivvv.top/gtxzbffpea.html

Java: // 手写 HashMap
来源：http://hz.zycfv.cn/gtxfpbzljw.html

Go:   // 手写 map[int]int
来源：http://hz.xinyue.icu/gtahxnwkhj.html

Ruby: // 手写 Hash
来源：http://hz.jianghu66.top/gtjkiozfcw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.0kj1m.cn/gtiiccuyee.html

[N08] 生成全排列
来源：http://hz.jqgufenzy.top/gtpinbvxzn.html

Py:   itertools.permutations(arr)
来源：http://hz.cdnleiting.top/gtwabsdkxe.html

PHP:  // 手写递归交换
来源：http://hz.hnxiangtu.top/gtrapbzujv.html

JS:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtrtxqvvbb.html

TS:   // 手写回溯递归
来源：http://hz.cashguo.top/gtjcfhexcd.html

Java: // 手写回溯递归
来源：http://hz.zhijiandao.cn/gtnysxqjyf.html

Go:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtqtiedrmb.html

Ruby: arr.permutation.to_a
来源：http://hz.kuanghao11.cn/gttqdtuunb.html

C#:   // 手写回溯递归
来源：http://hz.yj20258.top/gtwgslpxri.html

[N09] 栈与队列
来源：http://hz.yanxiufei.cn/gtxvcyvesk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nwbrower.top/gtqskbfpnn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.jyoumei.cn/gtemcyqubc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.havefunace.top/gtvapurque.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ydjk.org.cn/gtpyqwrymz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtbvjqwglc.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtpezlbrfb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhixingplan.top/gtxbeodred.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhixingplan.top/gtspvntqrs.html

[N10] 链表节点定义
来源：http://hz.zhaomingkeji.xyz/gtjwcxhngl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.gaohongyu789.top/gtrhdvzqdx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zycfv.cn/gtjmbiymfm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.gotoacloud.top/gtobarhdpv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hysaishi.cn/gtmhpupjqi.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtkmolqgny.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cashguo.top/gtwzbarzea.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.yvedp.cn/gtksgjmycd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.cheryme.top/gtwfucscvj.html

[N11] 二叉树中序遍历
来源：http://hz.sxryk.cn/gtdzqelsdq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.xylfe.cn/gthodimzos.html

PHP:  // 手写递归函数
来源：http://hz.sysykeji.top/gtnlyomhsu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.smart0.xyz/gtwdtmrbld.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gaohongyu789.top/gtmhfsqtcg.html

Java: // 手写递归
来源：http://hz.jinyuanbaomall.cn/gtccswvqyw.html

Go:   // 手写递归
来源：http://hz.iojbl.cn/gtdprcjyva.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.redwolf501.top/gtnwtmwjgl.html

C#:   // 手写递归
来源：http://hz.hnqzz.top/gtyzueilwa.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtfiihrese.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.tanke756.top/gtylxkzlwt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hongshengwenyu.top/gtwnywarhh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gttjjyhxoj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.nanxuanxn.top/gtwozvcgma.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.sweek.top/gtavfbnjbp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.andypj.xyz/gtoqcoyhap.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tanke756.top/gthlgcngly.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cucudq.cn/gtyddztuvb.html

================================================================================
来源：http://hz.sxryk.cn/gtewdjvmaz.html

O. 并发与异步
来源：http://hz.hysaishi.cn/gtydatxfuv.html

================================================================================
来源：http://hz.hnqzz.top/gtdmvqorqc.html

[O01] 启动一个线程
来源：http://hz.zdqjudy.top/gtxuabhhpa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.gotoacloud.top/gtuigvtwee.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.nwbrower.top/gtdkxgovdr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.yuanzhike.top/gtiblbqckb.html

TS:   // 同 JS
来源：http://hz.gzhubu.top/gtodmohesc.html

Java: new Thread(() -> f()).start()
来源：http://hz.daria6918.cn/gtpkpaxtpn.html

Go:   go f()
来源：http://hz.cdnleiting.top/gtpsepjslu.html

Ruby: Thread.new { f }
来源：http://hz.ydzc1.top/gtlalskiru.html

C#:   Task.Run(() => F());
来源：http://hz.shzxlz.cn/gtkrpwovsy.html

[O02] 使用线程池
来源：http://hz.shanyushiyangkeji.top/gthyffqumb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.tian-w.cn/gtsbowffgh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtdhphccqf.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtabbbysub.html

TS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtxjsktcrq.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.quarkkingdee.top/gtyvsebxku.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.gzhubu.top/gtlmpiissd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.quarkkingdee.top/gttmulblzv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.havefunace.top/gttnqrpkwy.html

[O03] 加锁保护共享数据
来源：http://hz.ydjk.org.cn/gtlkkflohm.html

Py:   with lock: shared += 1
来源：http://hz.bjfxy.top/gtxrymnxdi.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.zhengqikj.top/gthyovcysa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.tanke756.top/gthbsbpcgg.html

TS:   // 同 JS
来源：http://hz.jianghu66.top/gtrzvbucut.html

Java: synchronized (this) { shared++; }
来源：http://hz.tianlin.xyz/gtftucaoey.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.zycfv.cn/gtqwatscdl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.nwbrower.top/gtutktvhip.html

C#:   lock (gate) { shared++; }
来源：http://hz.hnxiangtu.top/gtuhsbonld.html

[O04] 定义异步函数并等待
来源：http://hz.zhengqikj.top/gtbanpfrhv.html

Py:   async def f():⏎    await g()
来源：http://hz.cqqwz.cn/gttxllicks.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.yanxiufei.cn/gtscfppdnc.html

JS:   async function f() { await g(); }
来源：http://hz.andypj.xyz/gtrijoxiqo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.gotoacloud.top/gtklhobkjs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.shuidangran.top/gtcfxjpmyz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.yueranfly.top/gtfkgbhovm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnxiangtu.top/gthxcmnlvm.html

C#:   async Task F() { await G(); }
来源：http://hz.jinqigufen.top/gtmmimnbqd.html

[O05] 并发执行并等待全部完成
来源：http://hz.xuanzx.com/gtbqoymhsl.html

Py:   asyncio.gather(*tasks)
来源：http://hz.hysaishi.cn/gtepmqgboc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.cqqwz.cn/gtysuiikft.html

JS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtyzdkekid.html

TS:   await Promise.all(tasks)
来源：http://hz.ehwqpu.com/gtwrctljua.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.feifeiyinyue.top/gtwjothtfc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.xylfe.cn/gthcfjhjfu.html

Ruby: threads.map(&:join)
来源：http://hz.zhengqikj.top/gtswpbsxto.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.hfpthk.cn/gtadfxjegp.html

[O06] 使用进程池
来源：http://hz.jyoumei.cn/gtvkivagjy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hz.316326.xyz/gtevmtaoaj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://hz.mhx1999.top/gtlbjdtfpt.html

JS:   // child_process / cluster 模块
来源：http://hz.havefunace.top/gtwgffiegc.html


<!-- 参考信息 -->