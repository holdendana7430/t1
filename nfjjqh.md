代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gttjrybdtk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtpwfmoibu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jyoumei.cn/gtohxaxgdw.html

[L02] 发送 POST JSON
来源：http://hz.9152youxi.cn/gtlgbnnuia.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtdkeefrix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgufenzy.top/gtozugbceo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtlexzewjw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtlwifyhrv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yangfankeji.com/gtkimayvro.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtmyizayjh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtkqppxfrb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gthuifgisf.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtafpnlmwr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtnzqcoxrd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangshuangyany.cn/gtxjqbtdvh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtkxkymxmm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gthdtxkxfe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.kuanghao11.cn/gttaaaksru.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtspjgnqqu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtgevmicql.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtkpxvumjc.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtrfszvkfv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtwbdrqpfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guannengcc.top/gtyfoyfctc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtkrtuihkv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtfuderomk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtwadzuoff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nanxinkj.top/gtleuzpins.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.meibo888.top/gtgvcxvjgt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtqqfnvdts.html

[L05] 上传文件（multipart）
来源：http://hz.smart0.xyz/gtpsxuouog.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.feifeiyinyue.top/gtbqxvmrtk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.kuanghao11.cn/gtkcurjtkk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtlclndhma.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtbwlsgdqf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.kuanghao11.cn/gtdvykzbft.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ivvv.top/gtsgwhrasz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.snrcjt.cn/gtujkqduhd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtcmxyqwkt.html

[L06] 解析响应为 JSON
来源：http://hz.tianlin.xyz/gtfabqnzli.html

Py:   resp.json()
来源：http://hz.xylfe.cn/gttkozqnck.html

PHP:  json_decode($body, true);
来源：http://hz.chenlongwang.top/gthfnphqpw.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtuijhihia.html

TS:   await resp.json()
来源：http://hz.yuanzhike.top/gtevivodgb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yueranfly.top/gtzmqdjdnn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.pengpengdd.cyou/gttcyvdjxf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtcgxeephj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtovyzawxk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yongpay.top/gtnwzszbxd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cashguo.top/gtkuehwfsw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xuanzx.com/gtsyoqdwia.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtvizzldad.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtkpilxial.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtrxklsfht.html

Go:   resp.StatusCode
来源：http://hz.xuanzx.com/gtqbzvwfnq.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtsnoiefad.html

C#:   (int)resp.StatusCode
来源：http://hz.316326.xyz/gtxjvtpfwf.html

[L08] 并发请求多个地址
来源：http://hz.tanke756.top/gtohefswpu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tian-w.cn/gtkkguvphe.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtjqksrwkq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtzwntcjnm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtwicvkkmn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zdqjudy.top/gthliumijl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cucudq.cn/gtxtmpebms.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.haohaochexian.top/gtalcvwsfc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtcwhnkukm.html

================================================================================
来源：http://hz.hywenlv.cn/gtbjomdrlx.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtyoyzcnpn.html

================================================================================
来源：http://hz.jinqigufen.top/gtufnrcili.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtmeqfxvjz.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtghkxhjws.html

PHP:  $argv;  $argc;
来源：http://hz.feifeiyinyue.top/gtvxhalgpf.html

JS:   process.argv.slice(2)
来源：http://hz.yonumen.top/gttzvzrvsq.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtrbqgybic.html

Java: args 数组（main 方法参数）
来源：http://hz.pengpengdd.cyou/gtmnadznlq.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtdszwjayf.html

Ruby: ARGV
来源：http://hz.zhengqikj.top/gtazhyozoc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtgyujfegi.html

[M02] 读取环境变量
来源：http://hz.yongpay.top/gthfgfqwxm.html

Py:   os.environ.get("HOME")
来源：http://hz.yuxming.cn/gteozpqwty.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtmfkgqzjx.html

JS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtecszvrpv.html

TS:   process.env.HOME
来源：http://hz.chenzaomai.com/gtxnrluvan.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtohqcegju.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtmglovxha.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gttvnasvoi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yvedp.cn/gtsfvdjfcg.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtwenethph.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hywenlv.cn/gtcdntueus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hfpthk.cn/gtijfrzdev.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtxluxwexd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cheryme.top/gtcovdehxx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhixingplan.top/gtzzodrnoa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtamiivpce.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangkeji.top/gtwimwgoaf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.aizwys.cn/gtswzexqgh.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gttdojummd.html

Py:   os.getcwd()
来源：http://hz.52xcode.cn/gtiruybqrj.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtlvhnilko.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtmpybrqkh.html

TS:   process.cwd()
来源：http://hz.ehwqpu.com/gtxeoptaoh.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtyypyovyl.html

Go:   os.Getwd()
来源：http://hz.svipenyu.cn/gtbzargudy.html

Ruby: Dir.pwd
来源：http://hz.yj202588.top/gtojjoddsr.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtiabaewob.html

[M05] 设置退出码
来源：http://hz.ppjwa.cn/gtplvgcbci.html

Py:   sys.exit(1)
来源：http://hz.nanxuanxn.top/gtodvyxdnq.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtrmaiieyc.html

JS:   process.exit(1)
来源：http://hz.andypj.xyz/gtfsmpmxnh.html

TS:   process.exit(1)
来源：http://hz.chenzaomai.com/gthgyyfxmh.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtruuhqpnp.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gtdjurmuxw.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtdfeddkqb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtozychrux.html

[M06] 向标准错误输出
来源：http://hz.cdnleiting.top/gtxpgkareg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gttbhettqk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ppjwa.cn/gtgkwufgwk.html

JS:   console.error("err")
来源：http://hz.sufxvd.cn/gttjeiqxtl.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtwxeojshf.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gthamswace.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtyvdqrufe.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gttzjymnis.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jlsjyb.cn/gtaohrehqh.html

[M07] 判断是否为主入口
来源：http://hz.zhengqikj.top/gtcbmgmjoc.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gtgshqnflg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yonumen.top/gthgkinjrz.html

JS:   require.main === module
来源：http://hz.jlsjyb.cn/gtwirjxbqg.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtzvhfaujm.html

Java: public static void main(String[] args)
来源：http://hz.jqgufenzy.top/gtfmwysvym.html

Go:   func main()
来源：http://hz.9152youxi.cn/gtxzpupoch.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtpmpgslbn.html

C#:   static void Main(string[] args)
来源：http://hz.daxiang520.top/gtzhcryznf.html

[M08] 获取系统与运行时信息
来源：http://hz.mhx1999.top/gtgucntqpj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtgtkewijd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gttdvotuxy.html

JS:   process.platform;  process.version
来源：http://hz.shuidangran.top/gtuvpxbiji.html

TS:   process.platform;  process.version
来源：http://hz.hongshengwenyu.top/gtskkxgafs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtovvwptrt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.hywenlv.cn/gtwwieleop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtixjqozkm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shangyingyoupin.top/gtjfihgsnv.html

================================================================================
来源：http://hz.guannengcc.top/gtvexvfzby.html

N. 数据结构与算法
来源：http://hz.hongshengwenyu.top/gtmjrusnvj.html

================================================================================
来源：http://hz.52xcode.cn/gteihwifmx.html

[N01] 二分查找（有序数组）
来源：http://hz.jinqigfzy.top/gtdwkxfeaf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xylfe.cn/gtxhznsusg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yvedp.cn/gtoncidpyj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nwbrower.top/gtxcoxpenk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhongyouzk.top/gttwalblqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtnnkszzwd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xziqi.cn/gttqtcdurj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtrfkdvrmq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yuanzhike.top/gtfdnocaqr.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xingfuxueyuan.xyz/gtnokwlhkg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ppjwa.cn/gteiqcctuw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hammf.cn/gtgamxwurs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhijiandao.cn/gtnbswniwl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtacfoabwh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.0kj1m.cn/gtpumtizgf.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtpvbbszog.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtkxmzkmey.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhixingplan.top/gtnqozvtuh.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtnbehwvbw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.quarkkingdee.top/gthljeqmgf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jyoumei.cn/gtpezydhqh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.mhx1999.top/gttazfqwju.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigufen.top/gtuxkpjlow.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtmiyiiunj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hysaishi.cn/gtxnbopkbv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.jqgfzy.top/gtarnnnsts.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.wangdashe.top/gtogpigmwk.html

[N04] 斐波那契数列
来源：http://hz.yangfankeji.com/gtcwowdewu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxinkj.top/gtenafsopi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xinyue.icu/gtkhdfewmg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangtech.top/gtalkiqagj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nanxinkj.top/gtotjszsdg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtvmukcmne.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jyoumei.cn/gtsfgbbxlf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xingfuxueyuan.xyz/gtyzykziti.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gticudndvh.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gtznkstbqq.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtxcfsdvft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.mhx1999.top/gtqmhqkdzw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yanxiufei.cn/gtcpevhxpw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtwzkdyvbw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tanke756.top/gtzdhtxthx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.wangshuangyany.cn/gtesmtqhlc.html

Ruby: a.gcd(b)
来源：http://hz.chenjidiqi.icu/gtjzsovcbd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jlsjyb.cn/gtqgfbbmnz.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtohgwqkdk.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtnolquygx.html

PHP:  $s === strrev($s);
来源：http://hz.zhiwuduotai.top/gtoeqjaicj.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gthqjywcju.html

TS:   s === [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtkfkmpwzw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.9152youxi.cn/gtoafmedvq.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gtzetyyqse.html

Ruby: s == s.reverse
来源：http://hz.guannengcc.top/gtvnohrlnm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtcfunvwoo.html

[N07] 两数之和（返回下标）
来源：http://hz.sweek.top/gtbwnctxfr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hnqzz.top/gtywhvkamp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.pycfn.com/gtqzlgzqst.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nwbrower.top/gtamhlsfdj.html

TS:   // 手写 Map<string, number>
来源：http://hz.shanyushiyangkeji.top/gtziyupprr.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gthmltzbbe.html

Go:   // 手写 map[int]int
来源：http://hz.zdqjudy.top/gtzmtgccxb.html

Ruby: // 手写 Hash
来源：http://hz.yj20258888.top/gtfxczpsix.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.pengpengdd.cyou/gtmxhvnvnn.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtntbfizpb.html

Py:   itertools.permutations(arr)
来源：http://hz.jlsjyb.cn/gthhllotta.html

PHP:  // 手写递归交换
来源：http://hz.xuanzx.com/gtjxvnmgew.html

JS:   // 手写回溯递归
来源：http://hz.9152youxi.cn/gtolpuajja.html

TS:   // 手写回溯递归
来源：http://hz.chenzaomai.com/gtkirsdkvs.html

Java: // 手写回溯递归
来源：http://hz.ybcxt.top/gtpjwcpbza.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtlzmqfgsm.html

Ruby: arr.permutation.to_a
来源：http://hz.0kj1m.cn/gtncpmadcp.html

C#:   // 手写回溯递归
来源：http://hz.xingfuxueyuan.xyz/gtudvrpiva.html

[N09] 栈与队列
来源：http://hz.xinyue.icu/gtkeascnle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.gaohongyu789.top/gtkzlftufw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sxryk.cn/gtudoxgjwq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.redwolf501.top/gtnaykkcua.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhoulong.xyz/gtjtmldylk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.tanke756.top/gtuyazdocd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.daxiang520.top/gtnrgummuo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.xinyue.icu/gtxsbalwvs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gaohongyu789.top/gtepvllpru.html

[N10] 链表节点定义
来源：http://hz.52xcode.cn/gtqxwklnhi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.pycfn.com/gtewuxwtfn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cucudq.cn/gterqpuybd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.andypj.xyz/gtqenpkfzt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.guowangkeji.top/gtidupstue.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gtidsbmdwx.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.mhx1999.top/gtogkfrkrk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.cashguo.top/gtsyoslgzz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhongyouzk.top/gtcvhysuiv.html

[N11] 二叉树中序遍历
来源：http://hz.ppjwa.cn/gtoiqjziql.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.nwbrower.top/gtksicoxys.html

PHP:  // 手写递归函数
来源：http://hz.jinqigufen.top/gtkbrfqjxj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.cashguo.top/gtlkwwqggo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sxryk.cn/gtajrghhex.html

Java: // 手写递归
来源：http://hz.yanxiufei.cn/gtakgtshbf.html

Go:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtnjbujogs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.yangfankeji.com/gtlryhkric.html

C#:   // 手写递归
来源：http://hz.hongshengwenyu.top/gtlukiisgz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gotoacloud.top/gtpzwhevev.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.xuetiantiany.cn/gtrjziwkkd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.havefunace.top/gtvyjntqpj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yj20258.top/gtzqyojdfm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.kuanghao11.cn/gteremvbgm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtlbbrtuwo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.hammf.cn/gtxntookym.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.iojbl.cn/gtijlhxlet.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.gotoacloud.top/gtqskpthmr.html

================================================================================
来源：http://hz.jqgufenzy.top/gttjrwlguu.html

O. 并发与异步
来源：http://hz.bjfxy.top/gtpsfwcwgs.html

================================================================================
来源：http://hz.svipenyu.cn/gtdqjgmrcs.html

[O01] 启动一个线程
来源：http://hz.yonumen.top/gthclivgws.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.fengsongda.top/gtiaiyanpt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.52xcode.cn/gtnhxovvbb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.zhaomingkeji.xyz/gttohqgiwd.html

TS:   // 同 JS
来源：http://hz.316326.xyz/gtsdwxodma.html

Java: new Thread(() -> f()).start()
来源：http://hz.smart0.xyz/gtousexfpu.html

Go:   go f()
来源：http://hz.tian-w.cn/gtcoppvvsh.html

Ruby: Thread.new { f }
来源：http://hz.meibo888.top/gthvbnekbn.html

C#:   Task.Run(() => F());
来源：http://hz.guannengcc.top/gtzpskntoy.html

[O02] 使用线程池
来源：http://hz.snrcjt.cn/gtqchrnegm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.wangshuangyany.cn/gtxiukcbdp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.pengpengdd.cyou/gtdjmbsoxs.html

JS:   // worker_threads 线程池
来源：http://hz.havefunace.top/gtbyxgoknu.html

TS:   // worker_threads 线程池
来源：http://hz.fzhhl.top/gtxogqfpoj.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ehwqpu.com/gtydexjgxp.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.hywenlv.cn/gtpeqnaqqu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.tianlin.xyz/gtehymdliv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.daxiang520.top/gthyistpjg.html

[O03] 加锁保护共享数据
来源：http://hz.shuidangran.top/gtyoquvmfb.html

Py:   with lock: shared += 1
来源：http://hz.iojbl.cn/gtnimzjkgk.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.hnqzz.top/gtiwxsizzk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.ydjk.org.cn/gtrdzwbdbp.html

TS:   // 同 JS
来源：http://hz.quarkkingdee.top/gtyrvqtimf.html

Java: synchronized (this) { shared++; }
来源：http://hz.dashuyun.cn/gthcxvtypy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.smart0.xyz/gtapmazvxt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.guowangkeji.top/gtsitseumz.html

C#:   lock (gate) { shared++; }
来源：http://hz.ehwqpu.com/gtdnhgjwim.html

[O04] 定义异步函数并等待
来源：http://hz.quarkkingdee.top/gteyzbqymp.html

Py:   async def f():⏎    await g()
来源：http://hz.daxiang520.top/gtgnricoge.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hz.wangshuangyany.cn/gtvxmcuufl.html

JS:   async function f() { await g(); }
来源：http://hz.cucudq.cn/gtgpgucgmy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://hz.ybcxt.top/gtzsazonxr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hz.9152youxi.cn/gtbkylpjse.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hz.daxiang520.top/gtgvbdkqke.html

Ruby: # 用 Fiber 或 async gem
来源：http://hz.hnqzz.top/gttxnprxpo.html

C#:   async Task F() { await G(); }
来源：http://hz.vqdsnc.cn/gtuqgwzmnr.html

[O05] 并发执行并等待全部完成
来源：http://hz.ydjk.org.cn/gtlfprjuey.html

Py:   asyncio.gather(*tasks)
来源：http://hz.pengpengdd.cyou/gtljvycoec.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hz.yueranfly.top/gthfdlokov.html

JS:   await Promise.all(tasks)
来源：http://hz.shzxlz.cn/gtbohgrozn.html

TS:   await Promise.all(tasks)
来源：http://hz.chenjidiqi.icu/gtullcqimf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hz.xinyue.icu/gtqhrmdosj.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hz.aibaodan.cn/gtymucwqhk.html

Ruby: threads.map(&:join)
来源：http://hz.hfpthk.cn/gtsajmlrrz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://hz.iojbl.cn/gtzprzolam.html


<!-- 参考信息 -->