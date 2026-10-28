代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtkomdrlci.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtevojksqr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtkpkdweui.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtpqedjajn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hnxiangtu.top/gtuqymnumc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtmzwnrrab.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtfxfqnddq.html

Py:   pickle.dumps(obj)
来源：http://hz.vqdsnc.cn/gtsilkjtkk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtpvxqxoym.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtgpdwolbt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtiadlriew.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtksgjmrfm.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtaealrnxv.html

Ruby: Marshal.dump(obj)
来源：http://hz.52xcode.cn/gtmmsqfcgt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtaoajruat.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcdwkrpul.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtlneevwtg.html

================================================================================
来源：http://hz.hfpthk.cn/gtfdcagwmc.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtlodrdamc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gthygesaog.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtwsdbiyer.html

JS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtygsqxwpc.html

TS:   await fetch(url)
来源：http://hz.tian-w.cn/gtcwqpvsrz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gturrwozoq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yanxiufei.cn/gtnmdseuuz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtnhdbodpv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhijiandao.cn/gtwdstuxyl.html

[L02] 发送 POST JSON
来源：http://hz.fzhhl.top/gtokzaswsp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gtexaafgzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtfgpjqxga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtmmneuwpo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtjablshsc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sxryk.cn/gtjgdunamz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgfzy.top/gtxrxdfoab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtuwmteahs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.havefunace.top/gthlivwioo.html

[L03] 设置自定义请求头
来源：http://hz.yj202588.top/gtnrrgimnj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sxryk.cn/gthlcrdyuw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sweek.top/gtzcynmrmd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtwwnwrsyi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtnqybdkis.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xylfe.cn/gtajerneiq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtdlpsnswj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ybcxt.top/gttijfbraj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jianghu66.top/gtetqsyubm.html

[L04] 设置超时
来源：http://hz.gaohongyu789.top/gtazokmxpl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.guannengcc.top/gtzcgvgcak.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.0kj1m.cn/gtpllxpavb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtxrvywtnc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtthtfdqgx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtcdeoavov.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.pycfn.com/gtrfnsjjbj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtzaaipdmo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigfzy.top/gtvmbgmhqk.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtqqqvbull.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pycfn.com/gtcyycinhb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yonumen.top/gtakxakemp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtldmjszrs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gterdngsrx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.andypj.xyz/gtdwexrrzy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gttkbzodzo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jyoumei.cn/gttakveoin.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gtnloizmcq.html

[L06] 解析响应为 JSON
来源：http://hz.guannengcc.top/gtacawmiqc.html

Py:   resp.json()
来源：http://hz.xingfuxueyuan.xyz/gttffilpuw.html

PHP:  json_decode($body, true);
来源：http://hz.ybcxt.top/gtupkwudjr.html

JS:   await resp.json()
来源：http://hz.zhengqikj.top/gtmiyptvdr.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtyeeqbrgb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangdashe.top/gtahiayrps.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtntdsjceb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tian-w.cn/gtlaxqefqc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.redwolf501.top/gtvnkccosr.html

[L07] 处理 HTTP 状态码
来源：http://hz.xziqi.cn/gtbagarotc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuetiantiany.cn/gtqbbpvwia.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sysykeji.top/gtqlcharkd.html

JS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gthhodxylm.html

TS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtpjztqbpe.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gthqthsbcq.html

Go:   resp.StatusCode
来源：http://hz.gzhubu.top/gtxognvany.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtvsjyutxj.html

C#:   (int)resp.StatusCode
来源：http://hz.gogol.net.cn/gtnvhdxecz.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gteeixqyka.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtzefgrzdt.html

PHP:  curl_multi_init() 系列
来源：http://hz.yj20258888.top/gtmkrndofa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtcetbitwb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtzuiksezt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtqsrcpdvl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtbwzofpfb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtrkrvsafk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtfkifzxza.html

================================================================================
来源：http://hz.yongpay.top/gtsyrjelth.html

M. 命令行 / 进程 / 环境
来源：http://hz.mhx1999.top/gtlgbrdcpo.html

================================================================================
来源：http://hz.redwolf501.top/gtapqcowmi.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtlblngiet.html

Py:   sys.argv[1:]
来源：http://hz.sufxvd.cn/gtzykrhheu.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtcgfoserj.html

JS:   process.argv.slice(2)
来源：http://hz.nwbrower.top/gtykxzzgef.html

TS:   process.argv.slice(2)
来源：http://hz.daria6918.cn/gtggadvabo.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gttfisyfgm.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtfmblgwow.html

Ruby: ARGV
来源：http://hz.yongpay.top/gthvnlcajp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinqigufen.top/gthqdsdjrh.html

[M02] 读取环境变量
来源：http://hz.yueranfly.top/gtfxxrbcqd.html

Py:   os.environ.get("HOME")
来源：http://hz.daria6918.cn/gttlpaobtn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shangyingyoupin.top/gtynzdghgx.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtsqzcsdrg.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gthrexpmvd.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtihjznuwv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.quarkkingdee.top/gtkehplwko.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtjxulekut.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtyhkpjzhw.html

[M03] 执行外部命令
来源：http://hz.shangyingyoupin.top/gtuanyhexa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.fengsongda.top/gtoymqvewu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gttbauccxf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtuwavpdvf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtnuwhtfgr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xylfe.cn/gtloqtpevm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ppjwa.cn/gthvlmglsh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtsfskvzlc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gtokstzfhr.html

[M04] 获取当前工作目录
来源：http://hz.sxryk.cn/gtibcgyrmy.html

Py:   os.getcwd()
来源：http://hz.nanxinkj.top/gtimdinuao.html

PHP:  getcwd();
来源：http://hz.zhijiandao.cn/gtginrziyo.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtxycoczlw.html

TS:   process.cwd()
来源：http://hz.52xcode.cn/gtmtoicgab.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydzc1.top/gtnbziinie.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtqkvwfdcv.html

Ruby: Dir.pwd
来源：http://hz.hammf.cn/gtcfzuznzq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gotoacloud.top/gtisfjjqid.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gthhdbstxl.html

Py:   sys.exit(1)
来源：http://hz.bjfxy.top/gtkjumnxsb.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gtgprldwpf.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtjvxmovbq.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtmxxwmcti.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtvioqtumh.html

Go:   os.Exit(1)
来源：http://hz.sufxvd.cn/gtkkgwugnw.html

Ruby: exit 1
来源：http://hz.zhoulong.xyz/gtegubactf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtqcfxieqj.html

[M06] 向标准错误输出
来源：http://hz.nanxinkj.top/gtmfotpiza.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtsamgbbvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.daria6918.cn/gtbaeahwqt.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gthyxjbpuq.html

TS:   console.error("err")
来源：http://hz.ppjwa.cn/gtdpvcclan.html

Java: System.err.println("err")
来源：http://hz.svipenyu.cn/gtwrvapzyk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258888.top/gteictlnat.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtxhiccwdc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhoulong.xyz/gtacsqnual.html

[M07] 判断是否为主入口
来源：http://hz.jlsjyb.cn/gtiplvuean.html

Py:   if __name__ == "__main__":
来源：http://hz.yangfankeji.com/gtucrgpcfh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ivvv.top/gttgjjvskq.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtxuhtevem.html

TS:   require.main === module
来源：http://hz.haohaochexian.top/gtxqhqevbf.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtptnrhykr.html

Go:   func main()
来源：http://hz.sufxvd.cn/gtztkqewdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.bjfxy.top/gtjlcqxocn.html

C#:   static void Main(string[] args)
来源：http://hz.zhaomingkeji.xyz/gtrmmjucxb.html

[M08] 获取系统与运行时信息
来源：http://hz.redwolf501.top/gtlwbhhkpz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.9152youxi.cn/gtiekwokww.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sxryk.cn/gtrictlcqm.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtmpicrghv.html

TS:   process.platform;  process.version
来源：http://hz.chenjidiqi.icu/gtxuylgrek.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gtcuawjppo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtekltampv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.9152youxi.cn/gtzyetzdyv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtdfdyxnjb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtkixpjmbn.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtvjoetcdr.html

================================================================================
来源：http://hz.tanke756.top/gtybqlygwe.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtilgnehns.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jianghu66.top/gtcpvmvmle.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jianghu66.top/gtmajbqdkg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.nanxuanxn.top/gtypoxfmkc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jlsjyb.cn/gtacjviarz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtxqokjvpx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jianghu66.top/gtlhrhlamm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.gogol.net.cn/gtcsqoepfs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gzhubu.top/gtcyjiycec.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258.top/gtydmggqjr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gteqdiqhux.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gttvobjhss.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yonumen.top/gtpfrolidj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhiwuduotai.top/gtaugowvqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtulxttxvp.html

Go:   slices.Sort(arr)
来源：http://hz.yueranfly.top/gtxgyhvkcf.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtqfcddlqd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtljqqulrq.html

[N03] 快速排序（分治示例）
来源：http://hz.kuanghao11.cn/gtbaxnntqo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.9152youxi.cn/gtcflrkwwx.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtaqjhmjgl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.bjfxy.top/gtjyimxvil.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtmsegadro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtqjxqyxuv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.haohaochexian.top/gtmbxkjrvx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.hnqzz.top/gtfwjjeubj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.gzhubu.top/gtvsjpwfak.html

[N04] 斐波那契数列
来源：http://hz.zhaomingkeji.xyz/gtnjdstslv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtcnchnere.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xuanzx.com/gtsglvpdxv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gtnwkqhhgf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.redwolf501.top/gtxgubjjay.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgufenzy.top/gtggxanxam.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yangfankeji.com/gtsyykamtt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.316326.xyz/gtjllfpzel.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtyrmjeauq.html

[N05] 最大公约数
来源：http://hz.hnxiangtu.top/gtjibaqiqh.html

Py:   math.gcd(a, b)
来源：http://hz.tianlin.xyz/gtjpfjeirz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgufenzy.top/gtsqmyhsqa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtcqprdkbx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtxfjopzca.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.chenzaomai.com/gtxhxvkhoi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.daxiang520.top/gtsnzifxdu.html

Ruby: a.gcd(b)
来源：http://hz.xingfuxueyuan.xyz/gtyrxrckpd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtksovfeli.html

[N06] 判断回文字符串
来源：http://hz.xuanzx.com/gtydwwxjfv.html

Py:   s == s[::-1]
来源：http://hz.jinghuilouyu.cn/gtyjyuaiaq.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtwogsrvtq.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtecjrzstz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtanafarrr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.snrcjt.cn/gtxrcbtmuk.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtwkklvubu.html

Ruby: s == s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtouqpqlej.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gteuknqqxa.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtjgnltfed.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.hysaishi.cn/gtyagnwuor.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtdalzylmc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtbwzmkhiw.html

TS:   // 手写 Map<string, number>
来源：http://hz.hfpthk.cn/gttkevzagb.html

Java: // 手写 HashMap
来源：http://hz.yj20258.top/gtynbbqcen.html

Go:   // 手写 map[int]int
来源：http://hz.smart0.xyz/gtzplgsgau.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtnakzfsqj.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.tianlin.xyz/gtimrpkzbb.html

[N08] 生成全排列
来源：http://hz.jinghuilouyu.cn/gtdfhjghru.html

Py:   itertools.permutations(arr)
来源：http://hz.nanxinkj.top/gtmuaijowq.html

PHP:  // 手写递归交换
来源：http://hz.cdnleiting.top/gtmxetayrq.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtpnilzpve.html

TS:   // 手写回溯递归
来源：http://hz.dashuyun.cn/gtfjunvvnf.html

Java: // 手写回溯递归
来源：http://hz.ppjwa.cn/gtukrvsdmv.html

Go:   // 手写回溯递归
来源：http://hz.havefunace.top/gtbvzkqfid.html

Ruby: arr.permutation.to_a
来源：http://hz.zhongyouzk.top/gtzjzynjhg.html

C#:   // 手写回溯递归
来源：http://hz.yanxiufei.cn/gtkymzfblm.html

[N09] 栈与队列
来源：http://hz.ivvv.top/gtttwkhxcx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.bjfxy.top/gtkmonxxdo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.nanxuanxn.top/gtwwuytfgr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jinqigufen.top/gtbuihgfah.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jinyuanbaomall.cn/gtgkgdchpt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.shuidangran.top/gtowccqdax.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.hysaishi.cn/gtgmtwcycu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cucudq.cn/gtffdsamiq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.aibaodan.cn/gtcdvkewsd.html

[N10] 链表节点定义
来源：http://hz.52xcode.cn/gtehmdjmkp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtgcmxmuem.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.iojbl.cn/gthlsletpb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.yj20258888.top/gthfuhwnyx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zdqjudy.top/gtqletnhdr.html

Java: class Node { int v; Node next; }
来源：http://hz.pengpengdd.cyou/gtkbiuqxds.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.52xcode.cn/gtcoavbcgv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xylfe.cn/gtzlnakbol.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.jqgufenzy.top/gtthdsxtfa.html

[N11] 二叉树中序遍历
来源：http://hz.hnxiangtu.top/gtzyzyxsiq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.tanke756.top/gtzhygyhej.html

PHP:  // 手写递归函数
来源：http://hz.andypj.xyz/gtofnyrgkr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tianlin.xyz/gtbswjbjyq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.chenjidiqi.icu/gtndoohjbz.html

Java: // 手写递归
来源：http://hz.shzxlz.cn/gtmqshhalm.html

Go:   // 手写递归
来源：http://hz.xylfe.cn/gtilkgidwk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.xuetiantiany.cn/gtgcbymyai.html

C#:   // 手写递归
来源：http://hz.shanyushiyangkeji.top/gtbzjxgsbh.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.daxiang520.top/gtprsmtbjs.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zycfv.cn/gtttnyawpc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.jianghu66.top/gteygrefdp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.aizwys.cn/gtesjlkiel.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenlongwang.top/gtjkyivmsr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yuxming.cn/gtcmbrgsfe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.jqgfzy.top/gtcrshnflf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.xuetiantiany.cn/gtztyjbhyr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.jinqigufen.top/gtwpvimzvx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtiiitlkvv.html

O. 并发与异步
来源：http://hz.xylfe.cn/gttfbxbagu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgcppvfeo.html

[O01] 启动一个线程
来源：http://hz.xylfe.cn/gtjzkbxjwl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.havefunace.top/gtmudsjulk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.zhongyouzk.top/gtkzvjcabx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.hnqzz.top/gtlwzjjmbn.html

TS:   // 同 JS
来源：http://hz.hnxiangtu.top/gtzzopmihs.html

Java: new Thread(() -> f()).start()
来源：http://hz.vqdsnc.cn/gtxxxpvgae.html

Go:   go f()
来源：http://hz.wangshuangyany.cn/gtrnitxodq.html

Ruby: Thread.new { f }
来源：http://hz.yangfankeji.com/gtjlcwjghk.html

C#:   Task.Run(() => F());
来源：http://hz.xuetiantiany.cn/gtlxsaouxu.html

[O02] 使用线程池
来源：http://hz.0kj1m.cn/gtcwvmiujl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ydzc1.top/gtwkmumebo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.feifeiyinyue.top/gtcpckswrb.html

JS:   // worker_threads 线程池
来源：http://hz.kuanghao11.cn/gtmvykolae.html

TS:   // worker_threads 线程池
来源：http://hz.shuidangran.top/gtivvavwpc.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.gzhubu.top/gtzdjprprh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.fengsongda.top/gtqlkotynn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.wangdashe.top/gtgdgnzgxf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.sufxvd.cn/gtxghqluqs.html

[O03] 加锁保护共享数据
来源：http://hz.52xcode.cn/gtxhgdfdes.html

Py:   with lock: shared += 1
来源：http://hz.yanxiufei.cn/gtvhrcflpu.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.jqgfzy.top/gtdwhifvix.html


<!-- 参考信息 -->