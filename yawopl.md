代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.chenjidiqi.icu/gtqanvfbyk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daria6918.cn/gtlguntbfn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gtoeclhzio.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtpzxgukmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtvfmxbszx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtzbxpbetj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtazmozoiv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtihyuksyr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtbupffalb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yanxiufei.cn/gtjcrrseds.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinqigufen.top/gtofmryuxg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhongyouzk.top/gtceddwhns.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gttabbkhaj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtbvdqyxai.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhoulong.xyz/gtxjzjvoma.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhengqikj.top/gtalcpxibp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aibaodan.cn/gtogyrlmeg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.andypj.xyz/gtfwulbbqh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gttwpyocmg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtkwvyqzug.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtorqpxjnh.html

[L04] 设置超时
来源：http://hz.zhaomingkeji.xyz/gtkljcugjz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtogdwjhnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtyvzwyqsw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gttiocenmr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtsstpkyjr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtwzwlylsq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtirqyaboc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yanxiufei.cn/gtwsydnbgy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtbygzqgqt.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtrqalqzed.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.316326.xyz/gtjglxnwhn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgfzy.top/gtrzzspmva.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtjoiktvcw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.kuanghao11.cn/gtzypvdgle.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtmfslztcu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gtzyazuwyn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtmpsjhegz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtftbqevwp.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtgouulbtn.html

Py:   resp.json()
来源：http://hz.yonumen.top/gtntshptkw.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258.top/gtprzmbvry.html

JS:   await resp.json()
来源：http://hz.ehwqpu.com/gtlbcssutn.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtgeopwfgh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.andypj.xyz/gtbrqghzuc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtbitxrzvo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtqkmzhmsf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gtciqcwqto.html

[L07] 处理 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtcswgtucg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.guowangkeji.top/gtpqwlssmq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.shanyushiyangkeji.top/gtixjoyfjv.html

JS:   resp.ok;  resp.status
来源：http://hz.yueranfly.top/gtslazzqpg.html

TS:   resp.ok;  resp.status
来源：http://hz.zhixingplan.top/gtpczpegmg.html

Java: resp.statusCode()
来源：http://hz.xuanzx.com/gtrmpkxhrk.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gtmupstpie.html

Ruby: resp.code.to_i
来源：http://hz.ybcxt.top/gtscsjfqnr.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtzzwkajae.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtxypzohza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hywenlv.cn/gttopuozir.html

PHP:  curl_multi_init() 系列
来源：http://hz.jyoumei.cn/gtkqwhsfwl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtiworuqkx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtwyjnxtls.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenlongwang.top/gtuipaxqfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gthvimfaty.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.fzhhl.top/gtmgaagknq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.quarkkingdee.top/gtoweodidv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtnwjhtplc.html

M. 命令行 / 进程 / 环境
来源：http://hz.ehwqpu.com/gtzcckfyds.html

================================================================================
来源：http://hz.guowangkeji.top/gtqqcxxwed.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtmyrikdqm.html

Py:   sys.argv[1:]
来源：http://hz.zhaomingkeji.xyz/gtppqlvbmf.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtmnrlhyta.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtylvksaeu.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtnppighwu.html

Java: args 数组（main 方法参数）
来源：http://hz.sysykeji.top/gtrxxhjaei.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtlvfqducf.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gtynspprsc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.andypj.xyz/gtqnxduwlt.html

[M02] 读取环境变量
来源：http://hz.yuanzhike.top/gtbqqkbonf.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtbikbfywo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtkxisuiyd.html

JS:   process.env.HOME
来源：http://hz.shanyushiyangtech.top/gtumnsszuu.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtnhtxqxna.html

Java: System.getenv("HOME")
来源：http://hz.zhongyouzk.top/gthdbopeym.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuanzhike.top/gtepsytzud.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtsntwumfp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zycfv.cn/gtxdcrgrwu.html

[M03] 执行外部命令
来源：http://hz.0kj1m.cn/gtidqmqhat.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtzwehckxo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtznengntf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtyhkzeclp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tian-w.cn/gtqckmleby.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtpyrekarw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtkwmijsyu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhengqikj.top/gtumlwcmuy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangkeji.top/gtcmdsgfcz.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtjwvbyava.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtkzbwnvxw.html

PHP:  getcwd();
来源：http://hz.shangyingyoupin.top/gthxatzjhj.html

JS:   process.cwd()
来源：http://hz.zhixingplan.top/gtgjffmlxv.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gtjxxpjyti.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gtknnzsrmc.html

Go:   os.Getwd()
来源：http://hz.chenzaomai.com/gtwsctgbks.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtgdjutajo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtvksdxcgi.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtmoatpkls.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtkcxmjuox.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtrclxkfrx.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtfzqrkazr.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtfqrrvtpq.html

Java: System.exit(1)
来源：http://hz.cdnleiting.top/gtljfnsfyq.html

Go:   os.Exit(1)
来源：http://hz.xziqi.cn/gttfzepzli.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtosxwnwdp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yanxiufei.cn/gtehpesxlm.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtnehrnfhd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtktymvows.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtujeychnf.html

JS:   console.error("err")
来源：http://hz.tianlin.xyz/gtuxouqjil.html

TS:   console.error("err")
来源：http://hz.zycfv.cn/gtvyfnzwht.html

Java: System.err.println("err")
来源：http://hz.ivvv.top/gtywyojxcc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sxryk.cn/gtukudtmew.html

Ruby: warn "err"
来源：http://hz.hongshengwenyu.top/gtnriipstk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.iojbl.cn/gtzkvdqvtt.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtpilprcfg.html

Py:   if __name__ == "__main__":
来源：http://hz.ppjwa.cn/gtcibhhpks.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenzaomai.com/gtrthdirek.html

JS:   require.main === module
来源：http://hz.tanke756.top/gtgixtqrkb.html

TS:   require.main === module
来源：http://hz.ybcxt.top/gtyncupexz.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtpglssysl.html

Go:   func main()
来源：http://hz.fzhhl.top/gtzvrhqyhx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fzhhl.top/gtkwdckgcx.html

C#:   static void Main(string[] args)
来源：http://hz.sxryk.cn/gtudwttcqb.html

[M08] 获取系统与运行时信息
来源：http://hz.gzhubu.top/gtlmplhkwq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cashguo.top/gtvpqidiwy.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.gotoacloud.top/gtzcvsahcx.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtoaqxolgu.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtvncpjkxi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhijiandao.cn/gtdfqpkqmf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gogol.net.cn/gtwylfoodh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gthfxphdit.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pycfn.com/gtpbgwkwsl.html

================================================================================
来源：http://hz.birdmap.top/gtrimmsopk.html

N. 数据结构与算法
来源：http://hz.cqqwz.cn/gtkujzcsdr.html

================================================================================
来源：http://hz.jyoumei.cn/gtqhrjbgke.html

[N01] 二分查找（有序数组）
来源：http://hz.jqgufenzy.top/gtaixtvlbh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtsboowvkg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gtskaiwiax.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gthprbmoek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gttxdcvkpk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sxryk.cn/gtwfvmraaq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jqgufenzy.top/gtcybnyvqr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtgxznhzhr.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hnxiangtu.top/gtvbybopwo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.kuanghao11.cn/gtlsoxwuwt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gtxqmbfofs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtmejblarz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.tianlin.xyz/gtiqywzdry.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cucudq.cn/gtlsbbjtvj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtvhwepjsi.html

Go:   slices.Sort(arr)
来源：http://hz.tanke756.top/gtztbfsilm.html

Ruby: arr.sort
来源：http://hz.guowangkeji.top/gtmuwefrcn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.9152youxi.cn/gtejafcnwi.html

[N03] 快速排序（分治示例）
来源：http://hz.pycfn.com/gtbrkjbwmk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtaxfahvlk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtuhjtgbeq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtsegkybii.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yj20258.top/gtihiolbst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.xingfuxueyuan.xyz/gtkmmatqxh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hnxiangtu.top/gthcdtkhxm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.iojbl.cn/gtfeyhrhva.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtqmwrrlmu.html

[N04] 斐波那契数列
来源：http://hz.hnxiangtu.top/gteczitdxx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gthyfpwlmu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jianghu66.top/gtnuyvdkyv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtkzlbvhyr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtkkaynjja.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtfyidiket.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtjiiscvxm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.svipenyu.cn/gtzxiheozi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtxwkpkvtz.html

[N05] 最大公约数
来源：http://hz.316326.xyz/gtaufbswoo.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtgoqelrct.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tanke756.top/gttzvxhhqg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.birdmap.top/gtdvbpfdav.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtmpddddba.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shangyingyoupin.top/gtvdwujxhz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.chenzaomai.com/gtocgsabrb.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtttpvvinq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnxiangtu.top/gthizobypl.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtovapfpyx.html

Py:   s == s[::-1]
来源：http://hz.yj20258888.top/gtcvqjnboi.html

PHP:  $s === strrev($s);
来源：http://hz.shuidangran.top/gtlygpbxcz.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtoxxrbavj.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtcjcwrrmo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.tianlin.xyz/gtkknecmzz.html

Go:   // 双指针从两端比较
来源：http://hz.aibaodan.cn/gtszfhjzyf.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtxokvfdpv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhijiandao.cn/gtomvszalb.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtozyuuxpa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cucudq.cn/gtyzhpczcr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.zhoulong.xyz/gtmodmqzrt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tanke756.top/gtlxmncsty.html

TS:   // 手写 Map<string, number>
来源：http://hz.zhijiandao.cn/gtprerulri.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtqitmvgir.html

Go:   // 手写 map[int]int
来源：http://hz.xinyue.icu/gtajtykycc.html

Ruby: // 手写 Hash
来源：http://hz.zhaomingkeji.xyz/gtbmcgnevm.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sysykeji.top/gtolijxuzc.html

[N08] 生成全排列
来源：http://hz.pycfn.com/gtqsbzmwjf.html

Py:   itertools.permutations(arr)
来源：http://hz.ydzc1.top/gtljarvdhc.html

PHP:  // 手写递归交换
来源：http://hz.yonumen.top/gtcqedczhg.html

JS:   // 手写回溯递归
来源：http://hz.ydjk.org.cn/gtlhunnelt.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gthpsoekiq.html

Java: // 手写回溯递归
来源：http://hz.yuanzhike.top/gtwahgsnur.html

Go:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtjpblibvq.html

Ruby: arr.permutation.to_a
来源：http://hz.redwolf501.top/gtyhanadye.html

C#:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtjixwnhne.html

[N09] 栈与队列
来源：http://hz.hywenlv.cn/gtnzlpwptx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.redwolf501.top/gtavepsvha.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.redwolf501.top/gtcjthyjys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtsoeuaufi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.kuanghao11.cn/gtwwthsxsu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ivvv.top/gtkrbitygu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.jqgufenzy.top/gthmjlnpji.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.andypj.xyz/gtatftjywb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.daxiang520.top/gtvguhrwgs.html

[N10] 链表节点定义
来源：http://hz.shangyingyoupin.top/gtvadeetut.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtqlzpqghj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xingfuxueyuan.xyz/gtlfujwlmi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.birdmap.top/gtdcavuukz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.meibo888.top/gtdzavwakb.html

Java: class Node { int v; Node next; }
来源：http://hz.zhijiandao.cn/gtuxngfydl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.vqdsnc.cn/gtjnqlnkau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtdhrdufgp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gaohongyu789.top/gtjrbsjnlv.html

[N11] 二叉树中序遍历
来源：http://hz.shuidangran.top/gtcftsrjfp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.jinqigufen.top/gtfqxosyzi.html

PHP:  // 手写递归函数
来源：http://hz.pengpengdd.cyou/gttfvmvcod.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yuxming.cn/gtyfyozlpe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtbahvnwml.html

Java: // 手写递归
来源：http://hz.c1oappe.top/gtnrmalxvv.html

Go:   // 手写递归
来源：http://hz.52xcode.cn/gtxwvztxwc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhixingplan.top/gttanikhws.html

C#:   // 手写递归
来源：http://hz.c1oappe.top/gtrggiyolh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jqgfzy.top/gtluznbzlo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.snrcjt.cn/gtjxttbqbf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gtujlitnan.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtzhwgltnh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.wangshuangyany.cn/gtolsxozdp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinyuanbaomall.cn/gtgqyonmuu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.dianchejie.cn/gtgfuarikh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.meibo888.top/gtixuwnfdb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.aizwys.cn/gtfmigllav.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtfrkklddi.html

O. 并发与异步
来源：http://hz.guannengcc.top/gtljutiler.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbjuxzqun.html

[O01] 启动一个线程
来源：http://hz.jinqigufen.top/gttzhfmwet.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.haohaochexian.top/gtyrnpfwuc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhaomingkeji.xyz/gtzlwbdxbf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.sufxvd.cn/gtnusxkobr.html

TS:   // 同 JS
来源：http://hz.0kj1m.cn/gtuusdoftd.html

Java: new Thread(() -> f()).start()
来源：http://hz.xuetiantiany.cn/gtpdpejryf.html

Go:   go f()
来源：http://hz.kuanghao11.cn/gtzdofqmmc.html

Ruby: Thread.new { f }
来源：http://hz.iojbl.cn/gtmwbakdkr.html

C#:   Task.Run(() => F());
来源：http://hz.tianlin.xyz/gtaszgvvvi.html

[O02] 使用线程池
来源：http://hz.fzhhl.top/gtxwcxjivc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.kuanghao11.cn/gtvepjpcmm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.hnqzz.top/gtzjeymvoe.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangtech.top/gtygfgfmec.html

TS:   // worker_threads 线程池
来源：http://hz.ywan-chungtsiang.top/gtfmrclvnt.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.feifeiyinyue.top/gtxvwtkjsf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.yuxming.cn/gtevgcivdk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.yj20258.top/gtigtgmljf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.gotoacloud.top/gtiomurowk.html

[O03] 加锁保护共享数据
来源：http://hz.dashuyun.cn/gtyuvsarlf.html

Py:   with lock: shared += 1
来源：http://hz.svipenyu.cn/gteykdoars.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.birdmap.top/gtadrcqkqp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ivvv.top/gtxexvxqli.html

TS:   // 同 JS
来源：http://hz.9152youxi.cn/gtbqdsrhyh.html

Java: synchronized (this) { shared++; }
来源：http://hz.yj20258888.top/gtldtmvxnv.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hnqzz.top/gtkappphjx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.52xcode.cn/gtwzaxmeed.html

C#:   lock (gate) { shared++; }
来源：http://hz.shangyingyoupin.top/gtsjqcskjg.html

[O04] 定义异步函数并等待
来源：http://hz.yuxming.cn/gtdekkjdnn.html

Py:   async def f():⏎    await g()
来源：http://hz.c1oappe.top/gtzyqtdaoq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.birdmap.top/gtvfokoqlw.html

JS:   async function f() { await g(); }
来源：http://hz.jqgfzy.top/gtkebazbry.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.xziqi.cn/gtdmucfrnb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.nwbrower.top/gtpmgcrfyf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.sufxvd.cn/gtchrgurmm.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.tianlin.xyz/gtzartneqx.html

C#:   async Task F() { await G(); }
来源：http://hz.jlsjyb.cn/gtaanltppb.html

[O05] 并发执行并等待全部完成
来源：http://hz.wangdashe.top/gtrosizhoe.html

Py:   asyncio.gather(*tasks)
来源：http://hz.shzxlz.cn/gtashsyvrd.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.fengsongda.top/gtxdwuaiam.html

JS:   await Promise.all(tasks)
来源：http://hz.52xcode.cn/gtgjksffsj.html

TS:   await Promise.all(tasks)
来源：http://hz.jinqigfzy.top/gtvojnnzyn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.hywenlv.cn/gtndesejjo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.gotoacloud.top/gtqciuyyab.html

Ruby: threads.map(&:join)
来源：http://hz.jinqigfzy.top/gtjazlgilv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.tian-w.cn/gtfuinyxjf.html


<!-- 参考信息 -->