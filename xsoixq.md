代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gticjnehbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtofpvczbu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtlcgtgbuu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.smart0.xyz/gtirgfiyyw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtllyuknlt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.aizwys.cn/gtbvznehpn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtuddlbsco.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtwqlfowji.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtfcqvvbgk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtlisgpbva.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.birdmap.top/gtlmtjmkdu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtfumgjrap.html

Go:   encoding/gob
来源：http://hz.gzhubu.top/gtibuxgtfs.html

Ruby: Marshal.dump(obj)
来源：http://hz.52xcode.cn/gtiyyivnyu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zycfv.cn/gtmteluvyk.html

================================================================================
来源：http://hz.yueranfly.top/gtxtdbqmsn.html

L. 网络请求
来源：http://hz.xuanzx.com/gtzoyxvsdy.html

================================================================================
来源：http://hz.zdqjudy.top/gthqmzbvnz.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtfsaljxfb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtvoqtdwih.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gtnnfwcngy.html

JS:   await fetch(url)
来源：http://hz.zhijiandao.cn/gtiytdhwdq.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gtzqdqukou.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtdhobmven.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtbthoziup.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gtdiovoprd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gtqifbjtqg.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtalyiiluf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gtzbbtpizv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtkqcpkcwc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hysaishi.cn/gtmgowpywc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtfvucfmws.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cqqwz.cn/gtgekhurnv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtlrcpyvwy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cheryme.top/gtvkmbfpgs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtbctqrkph.html

[L03] 设置自定义请求头
来源：http://hz.vqdsnc.cn/gtmaexkejv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gtzgaguzss.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yanxiufei.cn/gtbnzmxofi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtzywpazlf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guowangkeji.top/gtuvgavzbh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtbccuwslb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtnaqnrvjv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.havefunace.top/gtjwplwqvx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtfljsynuo.html

[L04] 设置超时
来源：http://hz.xuanzx.com/gtcqgxizic.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtwvxgvddg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pengpengdd.cyou/gtiqczzlyy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtesmxahsf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtkontlzkm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aizwys.cn/gtgqpdatxv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtwpjgtuap.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xingfuxueyuan.xyz/gtzuwpoboz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ydzc1.top/gtubfhtmsd.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtnbldarcg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhoulong.xyz/gtwfbpqrsn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtuowrbeur.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtjcpbxqzx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cdnleiting.top/gtotdrfxsc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtbiejlesc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtyapramaa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dashuyun.cn/gtnoeootwb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtdqgcoeun.html

[L06] 解析响应为 JSON
来源：http://hz.meibo888.top/gtlrcjqfcc.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtcwudrcqr.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtmuvbszcv.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtxbsazkdp.html

TS:   await resp.json()
来源：http://hz.hywenlv.cn/gtubtvkgvc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jqgufenzy.top/gtxiwuhltd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtaarmywyh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yongpay.top/gtkkogzffe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuetiantiany.cn/gtecewsemg.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtyhmvynlx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinghuilouyu.cn/gtvovtzjmw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtsgkgufvm.html

JS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtyjfgdsdi.html

TS:   resp.ok;  resp.status
来源：http://hz.dashuyun.cn/gtlojgrvvg.html

Java: resp.statusCode()
来源：http://hz.yangfankeji.com/gtbnhxynld.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtdezbqhpy.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gttuqtegoe.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtzhrtmkvu.html

[L08] 并发请求多个地址
来源：http://hz.hywenlv.cn/gtkmctlayj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtazksxdjb.html

PHP:  curl_multi_init() 系列
来源：http://hz.52xcode.cn/gtixvrorqx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtekpwvlgi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtztajqymd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtuwdmrckg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yueranfly.top/gtjmcgwtzq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtgnyfubrk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xingfuxueyuan.xyz/gtngnflkuq.html

================================================================================
来源：http://hz.shzxlz.cn/gtivzoeewm.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtjifvpnyo.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtttvsmsny.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtglmbxqwv.html

Py:   sys.argv[1:]
来源：http://hz.gzhubu.top/gtkqskshsy.html

PHP:  $argv;  $argc;
来源：http://hz.xinyue.icu/gtvalcykbl.html

JS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtnreiboou.html

TS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtgxsmniep.html

Java: args 数组（main 方法参数）
来源：http://hz.svipenyu.cn/gtpxrgqbzn.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtyrcynyfw.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtfgylnadz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shuidangran.top/gtkoisnvva.html

[M02] 读取环境变量
来源：http://hz.kuanghao11.cn/gthnyrlxwb.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtaraqhivg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.bjfxy.top/gtygvsgbal.html

JS:   process.env.HOME
来源：http://hz.cheryme.top/gtsheelfib.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtegzpyaqf.html

Java: System.getenv("HOME")
来源：http://hz.tanke756.top/gttreixibh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtfiwaivhb.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangkeji.top/gteczvvfwq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhongyouzk.top/gtivcpnpty.html

[M03] 执行外部命令
来源：http://hz.sysykeji.top/gttudsnfrz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ydzc1.top/gtbeutixnk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtsnejxmmt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtkzfepchw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pengpengdd.cyou/gtmkyipblt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.havefunace.top/gtbrnzmoza.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xuetiantiany.cn/gtmbkonugd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtmvtxqdyn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jlsjyb.cn/gtvomycsnd.html

[M04] 获取当前工作目录
来源：http://hz.sweek.top/gtplzritzg.html

Py:   os.getcwd()
来源：http://hz.xingfuxueyuan.xyz/gthxhkbqhc.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtullthsys.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtjvbjzyhs.html

TS:   process.cwd()
来源：http://hz.andypj.xyz/gtgsucbcmd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtxskdmrvt.html

Go:   os.Getwd()
来源：http://hz.jinyuanbaomall.cn/gtrislueof.html

Ruby: Dir.pwd
来源：http://hz.zhaomingkeji.xyz/gtuiaqsxvt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtuzotdzjz.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtlzwojcak.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtlsvrawuc.html

PHP:  exit(1);
来源：http://hz.nwbrower.top/gtaqwlekqt.html

JS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtjvkzgaqq.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtrzuwvcuv.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtaeszdppm.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtwychcnlk.html

Ruby: exit 1
来源：http://hz.shanyushiyangkeji.top/gttqmtjwwj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinyuanbaomall.cn/gtqxrhnhsg.html

[M06] 向标准错误输出
来源：http://hz.cashguo.top/gtgdweofvw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gthgcxncfz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fengsongda.top/gtsklgptub.html

JS:   console.error("err")
来源：http://hz.gogol.net.cn/gtaknblmlf.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtcleyfdok.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtxlnjsrsh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.9152youxi.cn/gtywrtrjse.html

Ruby: warn "err"
来源：http://hz.wangshuangyany.cn/gtmtkbdusc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinghuilouyu.cn/gtngjpzejo.html

[M07] 判断是否为主入口
来源：http://hz.ivvv.top/gtotayfjlv.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtrzmlqwab.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.pycfn.com/gtzujmurkc.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gtlvpqizdw.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtudnvgxne.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtibyhxdeu.html

Go:   func main()
来源：http://hz.jyoumei.cn/gtdysymkss.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhixingplan.top/gtqqzatwrb.html

C#:   static void Main(string[] args)
来源：http://hz.guowangkeji.top/gtxkxerazk.html

[M08] 获取系统与运行时信息
来源：http://hz.tanke756.top/gthzkuaaot.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhijiandao.cn/gtzocgiuut.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.birdmap.top/gtxtmmsnfs.html

JS:   process.platform;  process.version
来源：http://hz.c1oappe.top/gtnxwxhddi.html

TS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtxbuwgewl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtvyearlgd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fengsongda.top/gtiohoavbi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhongyouzk.top/gtjpsescou.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xingfuxueyuan.xyz/gthmlvndep.html

================================================================================
来源：http://hz.pycfn.com/gtppnnarmn.html

N. 数据结构与算法
来源：http://hz.zdqjudy.top/gtaxunzdyy.html

================================================================================
来源：http://hz.316326.xyz/gtzjheiwpq.html

[N01] 二分查找（有序数组）
来源：http://hz.nanxuanxn.top/gtcvrmezpo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.smart0.xyz/gtllnyxnem.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenzaomai.com/gtujakdmab.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtkbcmpdck.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtzmetgrbs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtawdlewrb.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.daxiang520.top/gtifqjszqs.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xylfe.cn/gtyizrevzh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtjvhovtgs.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.daxiang520.top/gtapicgrse.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tanke756.top/gtmlvpbvcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.vqdsnc.cn/gtakflhfpq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtmdiprnen.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gotoacloud.top/gtcnvatfft.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.fzhhl.top/gttiatlwoh.html

Go:   slices.Sort(arr)
来源：http://hz.fzhhl.top/gtybxktsxc.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtwxphnhea.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtnihonoej.html

[N03] 快速排序（分治示例）
来源：http://hz.ydjk.org.cn/gtngipuuaq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.gogol.net.cn/gtvsidgdty.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtwmjrrepv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangdashe.top/gtcuqcosra.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.pycfn.com/gtksgxflbu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sweek.top/gtkruvyddg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hywenlv.cn/gtakcvoioo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.quarkkingdee.top/gtdjafjdck.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtnqmvbbpt.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtosdqhlxv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yonumen.top/gtkprzjovg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.dianchejie.cn/gttnhzsisj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gthawfmfaj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtlxdvoabs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jiagoushi.top/gtutkrmksa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.c1oappe.top/gtmwicentp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gtihqojnfm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.c1oappe.top/gtsocgntrp.html

[N05] 最大公约数
来源：http://hz.zhoulong.xyz/gtgvcvvwpk.html

Py:   math.gcd(a, b)
来源：http://hz.vqdsnc.cn/gtofwvspjc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yangfankeji.com/gtgeqrsrfb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuetiantiany.cn/gtbkaeawwm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtnrjwhjml.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jianghu66.top/gtsbqvrfra.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.c1oappe.top/gtwudyqivu.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtqbmlimtr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigufen.top/gtapwldtwg.html

[N06] 判断回文字符串
来源：http://hz.nwbrower.top/gtpykfossb.html

Py:   s == s[::-1]
来源：http://hz.hysaishi.cn/gtdwnuobmh.html

PHP:  $s === strrev($s);
来源：http://hz.yanxiufei.cn/gtpdhaevti.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtevnyexya.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtntieqhol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.xziqi.cn/gtnbojeygb.html

Go:   // 双指针从两端比较
来源：http://hz.wangdashe.top/gtawxvvvwp.html

Ruby: s == s.reverse
来源：http://hz.guowangkeji.top/gtgxwzabyc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtgkrahkqo.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtpoizobhh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.cheryme.top/gtexdhzfhv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yj20258.top/gtiwcuuxyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.haohaochexian.top/gtxngwaiqu.html

TS:   // 手写 Map<string, number>
来源：http://hz.gaohongyu789.top/gtrjawjpei.html

Java: // 手写 HashMap
来源：http://hz.vqdsnc.cn/gtpculxldx.html

Go:   // 手写 map[int]int
来源：http://hz.sufxvd.cn/gtrplmwdsz.html

Ruby: // 手写 Hash
来源：http://hz.pycfn.com/gtvydqagra.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj202588.top/gtavngaqje.html

[N08] 生成全排列
来源：http://hz.zhixingplan.top/gtjvgjedzc.html

Py:   itertools.permutations(arr)
来源：http://hz.guannengcc.top/gtdklcjmsy.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtaolmkfjt.html

JS:   // 手写回溯递归
来源：http://hz.ydzc1.top/gtjkybscwc.html

TS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtfzgttpdc.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtestvvgck.html

Go:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtgomdcyme.html

Ruby: arr.permutation.to_a
来源：http://hz.nanxuanxn.top/gtepydkxua.html

C#:   // 手写回溯递归
来源：http://hz.gaohongyu789.top/gtmtezjjyt.html

[N09] 栈与队列
来源：http://hz.zhongyouzk.top/gtvladkwhi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xylfe.cn/gtpupzwftv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.chenlongwang.top/gtprmpnttk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yanxiufei.cn/gtcenvween.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.dashuyun.cn/gtoxsnxrae.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yonumen.top/gtyfmdjckq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.dianchejie.cn/gtuxqsikxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.gzhubu.top/gtflkxsqxa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinghuilouyu.cn/gtbeuxspuc.html

[N10] 链表节点定义
来源：http://hz.wangdashe.top/gthsvzjiyf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.jlsjyb.cn/gthzbxuzmk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.cqqwz.cn/gtajdtzjvo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.hongshengwenyu.top/gtoucooork.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.jlsjyb.cn/gtqtsuprkj.html

Java: class Node { int v; Node next; }
来源：http://hz.9152youxi.cn/gtpbgpkljg.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nwbrower.top/gtwwbhpmen.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.birdmap.top/gtovymiovn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.zhengqikj.top/gtzjpnxloe.html

[N11] 二叉树中序遍历
来源：http://hz.cucudq.cn/gtyvrtkqlc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.andypj.xyz/gtlwmzssta.html

PHP:  // 手写递归函数
来源：http://hz.guowangkeji.top/gtposczzcs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.daxiang520.top/gtvmjhejsb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.wangshuangyany.cn/gtifjiqpxw.html

Java: // 手写递归
来源：http://hz.aibaodan.cn/gtlkvkpymy.html

Go:   // 手写递归
来源：http://hz.0kj1m.cn/gtllmaiztg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.vqdsnc.cn/gtdsnhswgk.html

C#:   // 手写递归
来源：http://hz.dianchejie.cn/gthhdttymi.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.haohaochexian.top/gtgdpxzwvx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.chenlongwang.top/gtqnlkepef.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.dashuyun.cn/gttcromkgs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.guowangkeji.top/gteaftuhei.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.dianchejie.cn/gtkrlbincg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.wangdashe.top/gtjnqinqox.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.chenjidiqi.icu/gttdjhmyie.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.aizwys.cn/gtxiruhxbg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ehwqpu.com/gteqmiankr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbzabangz.html

O. 并发与异步
来源：http://hz.zhengqikj.top/gtfgstrqfc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnurxchok.html

[O01] 启动一个线程
来源：http://hz.gzhubu.top/gtwbmdnmtk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.ydjk.org.cn/gtumzwucsz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.shangyingyoupin.top/gtcvwjuywv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.chenlongwang.top/gtzvrvbkvk.html

TS:   // 同 JS
来源：http://hz.zhoulong.xyz/gtkeqlyjxw.html

Java: new Thread(() -> f()).start()
来源：http://hz.havefunace.top/gtqyylbhyb.html

Go:   go f()
来源：http://hz.tianlin.xyz/gtkuwxlkfb.html

Ruby: Thread.new { f }
来源：http://hz.52xcode.cn/gtimvsosso.html

C#:   Task.Run(() => F());
来源：http://hz.cheryme.top/gtgvdyckfx.html

[O02] 使用线程池
来源：http://hz.hysaishi.cn/gtuvpxgxbs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.yvedp.cn/gtfabbyzjn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.birdmap.top/gtrtwkxsly.html

JS:   // worker_threads 线程池
来源：http://hz.shanyushiyangkeji.top/gtfnvycahy.html

TS:   // worker_threads 线程池
来源：http://hz.xuetiantiany.cn/gtwfocsfmz.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.jinghuilouyu.cn/gtmmheecpa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.haohaochexian.top/gthlwdgcjt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.jinqigufen.top/gtsvnfjeou.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.ydzc1.top/gtypdwmcyq.html

[O03] 加锁保护共享数据
来源：http://hz.316326.xyz/gtcjvsoyxc.html

Py:   with lock: shared += 1
来源：http://hz.tian-w.cn/gtgtxdielb.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.nwbrower.top/gtttujeisq.html


<!-- 参考信息 -->