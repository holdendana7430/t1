代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gtnpedrnbd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtzaynwzow.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gtpoomxbbl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gteevqajyd.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gthblsfmjp.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtcamsgidx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.bjfxy.top/gtsykkcygh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtotkoirhp.html

L. 网络请求
来源：http://hz.zhoulong.xyz/gtxoydghwn.html

================================================================================
来源：http://hz.guowangkeji.top/gtvqnuhzjr.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtpbxeuhqh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pengpengdd.cyou/gtdfytlppm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtmvrcbooe.html

JS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtejtrcbiz.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtcuzciyds.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtwcdjahyi.html

Go:   resp, err := http.Get(url)
来源：http://hz.gotoacloud.top/gtaaweehce.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtycwiwegp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aibaodan.cn/gtxdpmavlo.html

[L02] 发送 POST JSON
来源：http://hz.dashuyun.cn/gtzsnserny.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtuquqtgdh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yonumen.top/gtzbnzatsf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ehwqpu.com/gtlbcxpmba.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgufenzy.top/gtyjnpwpvh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtfmivlvhf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ydzc1.top/gtkjnmdkxd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.andypj.xyz/gtufyzgbsb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtvrkxofwz.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtdveufycs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtwnhzblje.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.wangdashe.top/gtpqggikwh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtlzoukyvn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtjgetegub.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtazcrdamu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtfxrkmsog.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gtljnsgmiy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangtech.top/gtwzpuyoyl.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtgfejmysy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gttyzvmbmz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.wangdashe.top/gttuxopygb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtksjdzdun.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gticyfnjiu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtzaigrsfb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtmllrfdcc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtseehhnnl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnqzz.top/gtvmohcxfy.html

[L05] 上传文件（multipart）
来源：http://hz.9152youxi.cn/gtzfcogzqz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.quarkkingdee.top/gtugtgqgww.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtrtxkmvou.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtrgiiyskr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtnoepkett.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtkniahfpn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtmgbgqgqf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtvzsxrjyi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gttplksror.html

[L06] 解析响应为 JSON
来源：http://hz.fengsongda.top/gttxaesjfb.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtzjbyuzve.html

PHP:  json_decode($body, true);
来源：http://hz.guowangkeji.top/gtqgbmdlmv.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtlqsjvwqy.html

TS:   await resp.json()
来源：http://hz.meibo888.top/gtckhnqaft.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtxajougbk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinghuilouyu.cn/gttsityjfm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hammf.cn/gtcgbessdd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtpyljstat.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtgnhgckxa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtqautrrqn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtspvxkoux.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtygrgsedo.html

TS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtynwlvuzw.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtigastspl.html

Go:   resp.StatusCode
来源：http://hz.bjfxy.top/gtyrofvmfw.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gtaisefjnp.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gtzraupsxz.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtqulaobba.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xingfuxueyuan.xyz/gtacqlvmam.html

PHP:  curl_multi_init() 系列
来源：http://hz.iojbl.cn/gtdcbntome.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtkeqonkua.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtjicybqur.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtmubsegjd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtomnyffak.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtivinhnol.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtukvvkvpq.html

================================================================================
来源：http://hz.smart0.xyz/gtsqhzmdsn.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtmgfnoydj.html

================================================================================
来源：http://hz.redwolf501.top/gtqdbjkvmi.html

[M01] 读取命令行参数
来源：http://hz.haohaochexian.top/gtbmlazoby.html

Py:   sys.argv[1:]
来源：http://hz.vqdsnc.cn/gtbrqfrvob.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtcaseigso.html

JS:   process.argv.slice(2)
来源：http://hz.yj20258.top/gtwzfikriw.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtrptcnzhs.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtybjtwelh.html

Go:   os.Args[1:]
来源：http://hz.zhaomingkeji.xyz/gtswatdzqk.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtlghndwyl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.feifeiyinyue.top/gtbicpeshd.html

[M02] 读取环境变量
来源：http://hz.xingfuxueyuan.xyz/gtdefbrgcz.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtbrwvaemh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydzc1.top/gtkcwumoqe.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtqlsvbkwa.html

TS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtkljctlof.html

Java: System.getenv("HOME")
来源：http://hz.chenlongwang.top/gtrmlekxbs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.daria6918.cn/gtdktwnsbb.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtbaofckrw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cqqwz.cn/gttbfzopyq.html

[M03] 执行外部命令
来源：http://hz.daxiang520.top/gtzomoicyp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtosuspnkp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtvtdwwuyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtbhctsjai.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtfxzdykgi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtixavwolc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.tian-w.cn/gtnunmokcd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gogol.net.cn/gtvdyxydye.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gtctkvztfy.html

[M04] 获取当前工作目录
来源：http://hz.zycfv.cn/gtdbvusxhy.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gtycokgbco.html

PHP:  getcwd();
来源：http://hz.tianlin.xyz/gttugyyuil.html

JS:   process.cwd()
来源：http://hz.9152youxi.cn/gtobbmjasp.html

TS:   process.cwd()
来源：http://hz.yj202588.top/gttnzojsii.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtfmwmfmhf.html

Go:   os.Getwd()
来源：http://hz.mhx1999.top/gtwjdiuyvq.html

Ruby: Dir.pwd
来源：http://hz.shuidangran.top/gtvqididpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cdnleiting.top/gtuaiutqli.html

[M05] 设置退出码
来源：http://hz.pengpengdd.cyou/gtokdclsuh.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtrnzwchrm.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtdzcvmumk.html

JS:   process.exit(1)
来源：http://hz.ivvv.top/gtyrgsaxhd.html

TS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtifbnvfxd.html

Java: System.exit(1)
来源：http://hz.hongshengwenyu.top/gtrbtokvtm.html

Go:   os.Exit(1)
来源：http://hz.haohaochexian.top/gtifykdvea.html

Ruby: exit 1
来源：http://hz.quarkkingdee.top/gtdjlawyoa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.dashuyun.cn/gtnphvuxhq.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtwunfyryu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hfpthk.cn/gtnxeywgtq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtxpdpbqao.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtwbogkcul.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtoqdstnwl.html

Java: System.err.println("err")
来源：http://hz.pycfn.com/gteinstozl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cqqwz.cn/gtqmvpmqmk.html

Ruby: warn "err"
来源：http://hz.iojbl.cn/gtdcgmtmqy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtynwbmpuj.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtajgcmnqo.html

Py:   if __name__ == "__main__":
来源：http://hz.nanxinkj.top/gtgagcsyao.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtubbhlgfc.html

JS:   require.main === module
来源：http://hz.cucudq.cn/gtzqttzxpp.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtwzunroup.html

Java: public static void main(String[] args)
来源：http://hz.jqgfzy.top/gtqnrxxncy.html

Go:   func main()
来源：http://hz.daria6918.cn/gtrlrsurzv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sysykeji.top/gthfkekeue.html

C#:   static void Main(string[] args)
来源：http://hz.jqgfzy.top/gtwprkttbl.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtdmrcmcch.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cdnleiting.top/gtqrpnekgk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtnsajfrdq.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtizrorgqa.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtacwdoohi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cheryme.top/gtahpkgpdt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.guowangkeji.top/gtcgwnmwnz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ybcxt.top/gtamzigqvg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.pengpengdd.cyou/gtsyqtfknk.html

================================================================================
来源：http://hz.yj20258.top/gtxibursic.html

N. 数据结构与算法
来源：http://hz.zhiwuduotai.top/gtydvlbvgp.html

================================================================================
来源：http://hz.daria6918.cn/gtaygwglkf.html

[N01] 二分查找（有序数组）
来源：http://hz.cashguo.top/gttbujhcsu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinqigufen.top/gtrtwkgxtg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtsvrvzbzp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtsboxqfzz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtdghydbbn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gteexaqyqj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtrkqdjsqx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.daxiang520.top/gtiovqjgid.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtcdlduwnn.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtuhlchddp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtloewdmfn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtkcokptyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shuidangran.top/gtrrehlaut.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtolosudgs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtdxapvrqo.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtnsjbuqrv.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtlapufylp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigfzy.top/gtnzfduhug.html

[N03] 快速排序（分治示例）
来源：http://hz.gaohongyu789.top/gtwqserboz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtvbkstyfb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xziqi.cn/gtbxnxghvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yuanzhike.top/gtjnsxfnlf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtoccnqhut.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yongpay.top/gttufvylsj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.sxryk.cn/gtagdidesw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ivvv.top/gtbfkusisv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtkuazsobo.html

[N04] 斐波那契数列
来源：http://hz.zhengqikj.top/gtfllugphz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtlomdnbif.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gtosjoblzs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.snrcjt.cn/gtjktgzqtx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtyjnbwhlq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.aibaodan.cn/gtqzbshwrm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtijvaxpzl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtvzvpehbb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.dashuyun.cn/gtbkkzzzdn.html

[N05] 最大公约数
来源：http://hz.mhx1999.top/gtmvjmkmnq.html

Py:   math.gcd(a, b)
来源：http://hz.ybcxt.top/gtcdqluowm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gticljkpzi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinyuanbaomall.cn/gtiqqiscrb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtzznajjvw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.shangyingyoupin.top/gtkrsjxejh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtshcnvgbq.html

Ruby: a.gcd(b)
来源：http://hz.nwbrower.top/gtdgjbavap.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yuxming.cn/gtcipuwhsp.html

[N06] 判断回文字符串
来源：http://hz.tianlin.xyz/gtxlgvuagm.html

Py:   s == s[::-1]
来源：http://hz.hnxiangtu.top/gtjuuysbla.html

PHP:  $s === strrev($s);
来源：http://hz.jinqigfzy.top/gtzkxbupwd.html

JS:   s === [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtkrfkgdap.html

TS:   s === [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtpuaelaol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.iojbl.cn/gtvbmmcgsi.html

Go:   // 双指针从两端比较
来源：http://hz.gzhubu.top/gtzuqekyix.html

Ruby: s == s.reverse
来源：http://hz.ywan-chungtsiang.top/gtmpbbywme.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtvlzuxywt.html

[N07] 两数之和（返回下标）
来源：http://hz.zdqjudy.top/gtmutvuuxn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.wangshuangyany.cn/gtetzfhoxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuxming.cn/gtyeeevcks.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.yj202588.top/gtsjygmlyr.html

TS:   // 手写 Map<string, number>
来源：http://hz.cqqwz.cn/gtkgzfyzfx.html

Java: // 手写 HashMap
来源：http://hz.zhixingplan.top/gtgqphxzlc.html

Go:   // 手写 map[int]int
来源：http://hz.zycfv.cn/gtlxmahucf.html

Ruby: // 手写 Hash
来源：http://hz.ehwqpu.com/gtsxqnkxdc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.shzxlz.cn/gtufydkurq.html

[N08] 生成全排列
来源：http://hz.jiagoushi.top/gtqkmgetbe.html

Py:   itertools.permutations(arr)
来源：http://hz.smart0.xyz/gtuouczxpr.html

PHP:  // 手写递归交换
来源：http://hz.yuxming.cn/gtzkeucceh.html

JS:   // 手写回溯递归
来源：http://hz.wangdashe.top/gtmvslrmxf.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtemuxcvgz.html

Java: // 手写回溯递归
来源：http://hz.vqdsnc.cn/gtrjfpphsx.html

Go:   // 手写回溯递归
来源：http://hz.gogol.net.cn/gtfxyppcyp.html

Ruby: arr.permutation.to_a
来源：http://hz.cqqwz.cn/gtpjxsjtbg.html

C#:   // 手写回溯递归
来源：http://hz.cheryme.top/gtuhlpsgqj.html

[N09] 栈与队列
来源：http://hz.jinyuanbaomall.cn/gtdhaxfyfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtbhugnvde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.yvedp.cn/gttocawlob.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.chenzaomai.com/gtzumrmwdj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.ehwqpu.com/gtopjaccpb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhijiandao.cn/gtwaoidzgk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.c1oappe.top/gtgquanywf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shuidangran.top/gtagwqutun.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.gzhubu.top/gtquxqbnyn.html

[N10] 链表节点定义
来源：http://hz.yj202588.top/gtkwxwumvf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yangfankeji.com/gtznmivjke.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.zhijiandao.cn/gtzdwaunqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hysaishi.cn/gtovebhjpu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jinqigfzy.top/gtnikpiucp.html

Java: class Node { int v; Node next; }
来源：http://hz.wangshuangyany.cn/gtdhqnxant.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtryxxfdal.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.jiagoushi.top/gtzroqwpov.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.sweek.top/gtmgdlcgxv.html

[N11] 二叉树中序遍历
来源：http://hz.jinyuanbaomall.cn/gtkxuhtzsi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.fzhhl.top/gtmpwkhguk.html

PHP:  // 手写递归函数
来源：http://hz.c1oappe.top/gtgjxvetor.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.aibaodan.cn/gtfnfomnzx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj20258888.top/gtmhmaobaf.html

Java: // 手写递归
来源：http://hz.fengsongda.top/gtceogbgxv.html

Go:   // 手写递归
来源：http://hz.smart0.xyz/gtvbrylnux.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.sxryk.cn/gtqdjnlpcu.html

C#:   // 手写递归
来源：http://hz.quarkkingdee.top/gtamnzkohx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.jyoumei.cn/gtosnvyzds.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.ybcxt.top/gtqhrzpscc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.daria6918.cn/gtveohytqp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.smart0.xyz/gtfjqjjpqo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.zhongyouzk.top/gtcfabdbfb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinghuilouyu.cn/gtsitdgpsz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.redwolf501.top/gtnvebmezy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.tianlin.xyz/gtjxpyiywd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.feifeiyinyue.top/gtnutfxoll.html

================================================================================
来源：http://hz.mhx1999.top/gtdlkisxjx.html

O. 并发与异步
来源：http://hz.52xcode.cn/gtpdptovjm.html

================================================================================
来源：http://hz.chenzaomai.com/gtramfdmxi.html

[O01] 启动一个线程
来源：http://hz.cqqwz.cn/gtzlpexvyk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.cqqwz.cn/gtofedlibw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.guannengcc.top/gtignizawe.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hongshengwenyu.top/gtcoctbxnx.html

TS:   // 同 JS
来源：http://hz.sweek.top/gtwsqjzago.html

Java: new Thread(() -> f()).start()
来源：http://hz.hfpthk.cn/gtqaukcxcz.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtxhyzpbjk.html

Ruby: Thread.new { f }
来源：http://hz.xingfuxueyuan.xyz/gtxrhqkeom.html

C#:   Task.Run(() => F());
来源：http://hz.shanyushiyangkeji.top/gtxmweofnl.html

[O02] 使用线程池
来源：http://hz.yuxming.cn/gtgzscjqjy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.zhaomingkeji.xyz/gttkkxuagr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgfzy.top/gtkozvekkm.html

JS:   // worker_threads 线程池
来源：http://hz.cashguo.top/gtsjxzldkb.html

TS:   // worker_threads 线程池
来源：http://hz.cdnleiting.top/gtefruadzk.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.guannengcc.top/gtqlpcctkf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jiagoushi.top/gtjcxfyhdj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.nanxinkj.top/gtccmmxywv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jinqigufen.top/gtzabjrdoh.html

[O03] 加锁保护共享数据
来源：http://hz.yonumen.top/gtlcgcxiky.html

Py:   with lock: shared += 1
来源：http://hz.shzxlz.cn/gtamlixrdw.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.fengsongda.top/gtsxcphltp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.zhongyouzk.top/gtjesufdfg.html

TS:   // 同 JS
来源：http://hz.tian-w.cn/gtfrpawcht.html

Java: synchronized (this) { shared++; }
来源：http://hz.yongpay.top/gtocbqzicl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.hongshengwenyu.top/gtznsaloqx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://hz.bjfxy.top/gtnunysgvn.html

C#:   lock (gate) { shared++; }
来源：http://hz.yvedp.cn/gtajpfdgld.html

[O04] 定义异步函数并等待
来源：http://hz.ydjk.org.cn/gtjiewxuqf.html

Py:   async def f():⏎    await g()
来源：http://hz.sxryk.cn/gtwseneqej.html


<!-- 参考信息 -->