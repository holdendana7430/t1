代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtaxxiidbt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtslqzhsxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtavrkvfpp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.svipenyu.cn/gtwkcqpoef.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hysaishi.cn/gtshhftvob.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtrshtceqm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gtfnptwezq.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtyedfcmyh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtczghbwli.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtmbkzghbw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gttqbwgmrm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtswctzcay.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtajiveskl.html

Ruby: Marshal.dump(obj)
来源：http://hz.xylfe.cn/gtrfaxjyyd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtowsvidbr.html

================================================================================
来源：http://hz.xinyue.icu/gtrpekfuca.html

L. 网络请求
来源：http://hz.ydzc1.top/gtayqslzvh.html

================================================================================
来源：http://hz.svipenyu.cn/gtfsdjfesu.html

[L01] 发送 GET 请求
来源：http://hz.sysykeji.top/gtsyegdblv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhiwuduotai.top/gtpjgzfied.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cashguo.top/gtqxhxyxsi.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtsthzzuxm.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtxiwfajod.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guannengcc.top/gtjlffrgyk.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtlnxemwuw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtgmczkrcq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gttlxhjvnv.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtrdncsxch.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258888.top/gtartqahtn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hysaishi.cn/gtugcaohza.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gttvziyqki.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtkjmjqosp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtyzmfwsvr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sxryk.cn/gtnymniajk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.9152youxi.cn/gtjozbgdoq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gtgiklapqg.html

[L03] 设置自定义请求头
来源：http://hz.jinghuilouyu.cn/gtqofkhcss.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtapkescij.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtmcmuecxz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtgqwcvoic.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtxrtfigwt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xziqi.cn/gtfnpuerri.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtkyidvarq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yueranfly.top/gtasbzarrx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtpybqaalr.html

[L04] 设置超时
来源：http://hz.nanxuanxn.top/gtyytibrci.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtyohytjln.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtoaaszlos.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtumjfnzgn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtitihwmsr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cqqwz.cn/gtelpqfrhu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtrgavohfd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgufenzy.top/gtaziaphni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhengqikj.top/gtefqvcnjb.html

[L05] 上传文件（multipart）
来源：http://hz.zhixingplan.top/gtffrdovyk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gtnjdeutco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtnebpqyjb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pycfn.com/gtmqcgtgfz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtuvjlupor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtbvojlgcw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cdnleiting.top/gtaufridzi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangshuangyany.cn/gtmqswnxxn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gtoxerjoma.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258.top/gtgyotmkyr.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtydfoielj.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gtndgugayc.html

JS:   await resp.json()
来源：http://hz.guowangkeji.top/gtypbkknft.html

TS:   await resp.json()
来源：http://hz.xuetiantiany.cn/gtiwfgsejd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gthwcybjlt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtzugfjjnq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gtdetdbsqs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gtglwcyowp.html

[L07] 处理 HTTP 状态码
来源：http://hz.yuanzhike.top/gtwyjdsvcj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gaohongyu789.top/gtxxsmnafs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.mhx1999.top/gtcwzxnfhu.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtjljzawst.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtglovvfit.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtwvzuigbh.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtfimpsxbp.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtoymnbqsr.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtipjvvhsx.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtrexqoihm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenlongwang.top/gtqudtnlof.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtqnyaxoxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gttwggzdpo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtefxiliuj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gtmthsuuml.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ppjwa.cn/gtuvsecdht.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gotoacloud.top/gtmzxawayz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.316326.xyz/gtxipmgymb.html

================================================================================
来源：http://hz.redwolf501.top/gtlhopastg.html

M. 命令行 / 进程 / 环境
来源：http://hz.shuidangran.top/gtmvvmzmbb.html

================================================================================
来源：http://hz.nwbrower.top/gtnphagsmn.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gthwwipgsq.html

Py:   sys.argv[1:]
来源：http://hz.zhongyouzk.top/gtdzkhcxgr.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtyodbcuer.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtmfchmuqs.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtkbtaaxxy.html

Java: args 数组（main 方法参数）
来源：http://hz.sufxvd.cn/gtvnmsqcdz.html

Go:   os.Args[1:]
来源：http://hz.fzhhl.top/gtypakbhte.html

Ruby: ARGV
来源：http://hz.ydjk.org.cn/gtktgtndma.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtujmwwptp.html

[M02] 读取环境变量
来源：http://hz.xuetiantiany.cn/gtxvdvrmzb.html

Py:   os.environ.get("HOME")
来源：http://hz.ywan-chungtsiang.top/gtmkjcsrtk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtmdlwvwpa.html

JS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtikfpnmdx.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtkctjwjac.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtvtafenov.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yueranfly.top/gtnxkhvfcd.html

Ruby: ENV["HOME"]
来源：http://hz.wangdashe.top/gtdoiqugqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtmnbsimrz.html

[M03] 执行外部命令
来源：http://hz.cqqwz.cn/gtsjjaoxzf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtelknuxlx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yanxiufei.cn/gtaglxyyvo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.sweek.top/gtisojjwci.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtyrnmgnlf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtwugsoxly.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxinkj.top/gtfcssasyk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gttxxnlmix.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yvedp.cn/gthyazryoi.html

[M04] 获取当前工作目录
来源：http://hz.9152youxi.cn/gtqdhpjifb.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtqirblcrp.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtvechuwzc.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtykgaeinv.html

TS:   process.cwd()
来源：http://hz.cashguo.top/gtaawpskob.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dashuyun.cn/gtdgypcxyc.html

Go:   os.Getwd()
来源：http://hz.xingfuxueyuan.xyz/gthsjjrcie.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtdpexzkwu.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.haohaochexian.top/gtutndamye.html

[M05] 设置退出码
来源：http://hz.jinqigufen.top/gtkpshaird.html

Py:   sys.exit(1)
来源：http://hz.wangdashe.top/gtlmerbeok.html

PHP:  exit(1);
来源：http://hz.sysykeji.top/gtljvuxksq.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtzvwpkykt.html

TS:   process.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtbbupkffr.html

Java: System.exit(1)
来源：http://hz.daxiang520.top/gtzswicmko.html

Go:   os.Exit(1)
来源：http://hz.cheryme.top/gthyfiarmd.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtfygvuwlg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj202588.top/gtdgnsjhhb.html

[M06] 向标准错误输出
来源：http://hz.hfpthk.cn/gtjwgycihg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.fengsongda.top/gtigicmqxe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.tian-w.cn/gtinrywuii.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtgacvnlrd.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtpfkkiswv.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtrwuouexk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtcjxutchx.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtvcrsfqlk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtuafzcwuo.html

[M07] 判断是否为主入口
来源：http://hz.svipenyu.cn/gtmafghfky.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtahujwdfi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gtugylihxt.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtxvcojdxo.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gtwpfjskns.html

Java: public static void main(String[] args)
来源：http://hz.tian-w.cn/gtogqyhoor.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtmauwdkge.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtdszqchyp.html

C#:   static void Main(string[] args)
来源：http://hz.yonumen.top/gthoyojqou.html

[M08] 获取系统与运行时信息
来源：http://hz.yvedp.cn/gtvkwhioqx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtenoinhmi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.redwolf501.top/gtoqylkccx.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtesfopyxj.html

TS:   process.platform;  process.version
来源：http://hz.daxiang520.top/gtjigokovz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gtlzaddmdp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtrkxeybyf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtgoijyeze.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hysaishi.cn/gtfpzvdkzi.html

================================================================================
来源：http://hz.316326.xyz/gtmnxxabsv.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtacewykmq.html

================================================================================
来源：http://hz.hnqzz.top/gtilgahohf.html

[N01] 二分查找（有序数组）
来源：http://hz.zhaomingkeji.xyz/gtkucopbey.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gttwcqoakm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shuidangran.top/gtyoiiysek.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtzaresksu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtifogqifr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtrxvwjmkq.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtvebdrkiy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pengpengdd.cyou/gtweabbhaz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gtnvjyashw.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.havefunace.top/gtxvqjfvft.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtmygxqsqv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtluhgqhuz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jiagoushi.top/gtdzcubwjn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtnjfstbcd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.birdmap.top/gtftutxlzv.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtpwdacszw.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtslemhrma.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zdqjudy.top/gtvsvxubfj.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gtcoernibl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.shzxlz.cn/gtixsgvpdb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yvedp.cn/gtftsnjvbq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtitsompau.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtxxpthkpz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtvxzkgksp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtsvlcrehx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.bjfxy.top/gtszfkgxro.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jyoumei.cn/gtgpojaolx.html

[N04] 斐波那契数列
来源：http://hz.fzhhl.top/gtdibdgejk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtxzqodcau.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aizwys.cn/gtqeqfqmdb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xingfuxueyuan.xyz/gtsvvclaec.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jyoumei.cn/gtigjtetyb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtiodhgqya.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xziqi.cn/gtkjkhiqck.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtcjrxgngx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.feifeiyinyue.top/gthdualign.html

[N05] 最大公约数
来源：http://hz.gogol.net.cn/gtgfnmbvrv.html

Py:   math.gcd(a, b)
来源：http://hz.ivvv.top/gtzbbxyeug.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sufxvd.cn/gtsntgvgve.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tanke756.top/gtnuihjgrr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gttrbgvijr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yuanzhike.top/gtgaiepgdx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.svipenyu.cn/gtylqaqtnp.html

Ruby: a.gcd(b)
来源：http://hz.havefunace.top/gtlttmcpxj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ppjwa.cn/gtergspvaa.html

[N06] 判断回文字符串
来源：http://hz.zhaomingkeji.xyz/gtdijmacii.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtdugxwpxn.html

PHP:  $s === strrev($s);
来源：http://hz.havefunace.top/gtvcacvegh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtukgkkcpg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtdsrcajpa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jinqigufen.top/gtavbmntqr.html

Go:   // 双指针从两端比较
来源：http://hz.zycfv.cn/gtdninrmnl.html

Ruby: s == s.reverse
来源：http://hz.haohaochexian.top/gtyjohpbxd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtjnxongru.html

[N07] 两数之和（返回下标）
来源：http://hz.hongshengwenyu.top/gtcheehefb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.quarkkingdee.top/gtmvhbimlw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtrkwoqnuc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.smart0.xyz/gteryocarz.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinqigfzy.top/gtelvgisbt.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtxamcbhzz.html

Go:   // 手写 map[int]int
来源：http://hz.tianlin.xyz/gtnkfquniw.html

Ruby: // 手写 Hash
来源：http://hz.feifeiyinyue.top/gtdkfxsqvw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jianghu66.top/gtonikldex.html

[N08] 生成全排列
来源：http://hz.tianlin.xyz/gtgfjksczy.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtlnynojvn.html

PHP:  // 手写递归交换
来源：http://hz.aibaodan.cn/gtwohqohcc.html

JS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtvoyercmf.html

TS:   // 手写回溯递归
来源：http://hz.fzhhl.top/gttsuuqgsp.html

Java: // 手写回溯递归
来源：http://hz.meibo888.top/gtihqijkwj.html

Go:   // 手写回溯递归
来源：http://hz.fzhhl.top/gthydokdez.html

Ruby: arr.permutation.to_a
来源：http://hz.haohaochexian.top/gtfzwolfoh.html

C#:   // 手写回溯递归
来源：http://hz.zhaomingkeji.xyz/gthxvxbmpy.html

[N09] 栈与队列
来源：http://hz.gotoacloud.top/gttqicjazl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jyoumei.cn/gtpguwldiz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnqzz.top/gtkyrpvuev.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.guannengcc.top/gtcmltjcvm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.wangdashe.top/gteeddneao.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yj20258888.top/gtjdngmvwm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.svipenyu.cn/gtiuosjufk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.ehwqpu.com/gtepomykoh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.feifeiyinyue.top/gtbmxjofzd.html

[N10] 链表节点定义
来源：http://hz.meibo888.top/gtgrnhvquw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.chenlongwang.top/gtoxmagjru.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.fzhhl.top/gtcfhcpjsa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.ydzc1.top/gtmnvegziw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhengqikj.top/gtpexnqsvp.html

Java: class Node { int v; Node next; }
来源：http://hz.yonumen.top/gtsqipqtwe.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.jqgufenzy.top/gtxaxnzmop.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.xuetiantiany.cn/gtfvfynpsd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zdqjudy.top/gtetmbrdzr.html

[N11] 二叉树中序遍历
来源：http://hz.yj20258888.top/gtlgmzxwyy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.kuanghao11.cn/gtirckppak.html

PHP:  // 手写递归函数
来源：http://hz.aizwys.cn/gtsgodjtqz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.jlsjyb.cn/gtakvnauvj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.sysykeji.top/gtwibfvbex.html

Java: // 手写递归
来源：http://hz.gzhubu.top/gtmlgamcyf.html

Go:   // 手写递归
来源：http://hz.gzhubu.top/gtadvkcotg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.jyoumei.cn/gtbhfmyunn.html

C#:   // 手写递归
来源：http://hz.xingfuxueyuan.xyz/gtnawzdohs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.ehwqpu.com/gtcbjtvyco.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.zhaomingkeji.xyz/gtxvhadfma.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.svipenyu.cn/gtzclgexwj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tian-w.cn/gtezsbwwek.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.haohaochexian.top/gteqysfqbg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.iojbl.cn/gtycosnnlp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daxiang520.top/gtqscvsrgs.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.guowangkeji.top/gtutufdfyg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.fengsongda.top/gtkjluding.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnumhnned.html

O. 并发与异步
来源：http://hz.tanke756.top/gtchviiazq.html

================================================================================
来源：http://hz.hysaishi.cn/gtvfivcqnl.html

[O01] 启动一个线程
来源：http://hz.yuanzhike.top/gtmfywokcj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.yonumen.top/gtnbagqdaz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.birdmap.top/gtljsqxqzy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.fzhhl.top/gtmuogalzk.html

TS:   // 同 JS
来源：http://hz.jyoumei.cn/gtajjmctic.html

Java: new Thread(() -> f()).start()
来源：http://hz.daxiang520.top/gthezdnxzx.html

Go:   go f()
来源：http://hz.xziqi.cn/gtyxfywfdw.html

Ruby: Thread.new { f }
来源：http://hz.zhaomingkeji.xyz/gtjooxafpi.html

C#:   Task.Run(() => F());
来源：http://hz.wangshuangyany.cn/gtuxqrssyo.html

[O02] 使用线程池
来源：http://hz.svipenyu.cn/gtacwoncoy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.ehwqpu.com/gtyzaffdow.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.ybcxt.top/gtqdfebgfl.html

JS:   // worker_threads 线程池
来源：http://hz.yangfankeji.com/gtnaduqadm.html

TS:   // worker_threads 线程池
来源：http://hz.hnxiangtu.top/gtnhxwthms.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.nwbrower.top/gtgyxmybgt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.zhengqikj.top/gtptbthgww.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.shuidangran.top/gtdhdfpjfr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jqgfzy.top/gttfqqjdcf.html

[O03] 加锁保护共享数据
来源：http://hz.zhiwuduotai.top/gtujqkxpuo.html

Py:   with lock: shared += 1
来源：http://hz.pengpengdd.cyou/gtyrsbjgnc.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.smart0.xyz/gtkemistdz.html


<!-- 参考信息 -->