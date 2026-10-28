代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sufxvd.cn/gthstojaxh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtjatqihvt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtxqllsbcd.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtatppvvoe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtmxlyxlyh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtelpdswze.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtkpzcixsu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtiwjpjviq.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtknphrgdu.html

Ruby: Marshal.dump(obj)
来源：http://hz.sweek.top/gtwkspqbjt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.vqdsnc.cn/gtcmcnpnvi.html

================================================================================
来源：http://hz.ydzc1.top/gtsqxzewxg.html

L. 网络请求
来源：http://hz.yongpay.top/gtuosaaawz.html

================================================================================
来源：http://hz.cdnleiting.top/gtivlruacd.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gtyrqjplxa.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtbbxnrzjd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gogol.net.cn/gtwvynscas.html

JS:   await fetch(url)
来源：http://hz.316326.xyz/gtpqfhouem.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtpgcqzood.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtbtgmxvps.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtvvmxdlla.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gttfhxfunt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guannengcc.top/gtxrdrlgao.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtqtfmzgnm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtqohxzqsu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jqgfzy.top/gtaalyuouh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtjexbmfdh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gttmauxuji.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shanyushiyangkeji.top/gtnimbmofn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgufenzy.top/gtcdrhefhd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtdjpjcxjw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.redwolf501.top/gtygzsnveu.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtgxiyxpup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinyuanbaomall.cn/gtkttlrfii.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtpccyuauh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gttyliywcw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtfuclldqo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ppjwa.cn/gtcrlerrau.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtjgecsmqz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtafgrawql.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtzopymzjw.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtbbpttvpx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtarviveco.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hywenlv.cn/gtxngduugw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhaomingkeji.xyz/gttelchdrq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xinyue.icu/gtlouvfepd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gtgijpuzsk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gotoacloud.top/gtskvbvnvi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtdtmahewh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gthusjtmov.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtfovzyrwe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtoshmtgaw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zycfv.cn/gtxxqycanv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtcathdbvz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cashguo.top/gtizfwdzwy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtagpxjfnj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sufxvd.cn/gttdstigaw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangshuangyany.cn/gtfzbajauc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgufenzy.top/gtgmtygrkp.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtxmglhtae.html

Py:   resp.json()
来源：http://hz.birdmap.top/gtduhtjchr.html

PHP:  json_decode($body, true);
来源：http://hz.yonumen.top/gtrkozecva.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtklktqyvx.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtqtdoouyk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gotoacloud.top/gthpibckmo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hywenlv.cn/gtgejebtgp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtdnpafgkc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gogol.net.cn/gtvloiqyip.html

[L07] 处理 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtifwfjfym.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtkcjbwhpu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhiwuduotai.top/gtoksdonls.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtsbvjdcuh.html

TS:   resp.ok;  resp.status
来源：http://hz.9152youxi.cn/gtjnqxehxw.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtvdtcdxiu.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtknsesgue.html

Ruby: resp.code.to_i
来源：http://hz.birdmap.top/gtgyusgswr.html

C#:   (int)resp.StatusCode
来源：http://hz.sysykeji.top/gtpaxyjwui.html

[L08] 并发请求多个地址
来源：http://hz.zhijiandao.cn/gtzmaqqrpm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jianghu66.top/gtotyevrkp.html

PHP:  curl_multi_init() 系列
来源：http://hz.nwbrower.top/gtujcrvlgp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtervfpzht.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shangyingyoupin.top/gtavxtqnnz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtjxtyobjt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xziqi.cn/gtqgozoalj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guannengcc.top/gtubftwrkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtbojkcftk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbytkwxvk.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtumrmxthb.html

================================================================================
来源：http://hz.daxiang520.top/gtouetbvuz.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtjzsudpcr.html

Py:   sys.argv[1:]
来源：http://hz.jqgufenzy.top/gtsgxtnima.html

PHP:  $argv;  $argc;
来源：http://hz.yj202588.top/gtsnhhieem.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtwslgfyza.html

TS:   process.argv.slice(2)
来源：http://hz.havefunace.top/gtcpdrucyr.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtshbddkzq.html

Go:   os.Args[1:]
来源：http://hz.ydzc1.top/gthlxzxant.html

Ruby: ARGV
来源：http://hz.yueranfly.top/gtooweufop.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtakvivzmm.html

[M02] 读取环境变量
来源：http://hz.havefunace.top/gtrsjelavz.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtywukjedu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtqvzgmxif.html

JS:   process.env.HOME
来源：http://hz.dianchejie.cn/gtauquirwx.html

TS:   process.env.HOME
来源：http://hz.bjfxy.top/gtnwjlswpx.html

Java: System.getenv("HOME")
来源：http://hz.jlsjyb.cn/gtpcvirlos.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.havefunace.top/gtwzzgojkt.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtljjonfiq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtluviaicr.html

[M03] 执行外部命令
来源：http://hz.haohaochexian.top/gtpbcqjmkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj202588.top/gtmgwlusbm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gttlapssba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gthfgzodoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtklstjhyw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtlkctzqve.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gtpsodlkdr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cheryme.top/gtixobuzam.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yanxiufei.cn/gtqayvbbuk.html

[M04] 获取当前工作目录
来源：http://hz.0kj1m.cn/gtorbdygyc.html

Py:   os.getcwd()
来源：http://hz.yuanzhike.top/gtldbovccd.html

PHP:  getcwd();
来源：http://hz.haohaochexian.top/gtjwovqlcb.html

JS:   process.cwd()
来源：http://hz.sweek.top/gtrylxinmd.html

TS:   process.cwd()
来源：http://hz.jinqigfzy.top/gtfufpanog.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zdqjudy.top/gthcftpwte.html

Go:   os.Getwd()
来源：http://hz.nanxuanxn.top/gttstxnuyd.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gtymmehwug.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gthydnulwe.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtnkiuheav.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtwucowtub.html

PHP:  exit(1);
来源：http://hz.hammf.cn/gtyectmdtt.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtibhttccg.html

TS:   process.exit(1)
来源：http://hz.fengsongda.top/gtxqhtkigo.html

Java: System.exit(1)
来源：http://hz.smart0.xyz/gtnvaogiuc.html

Go:   os.Exit(1)
来源：http://hz.316326.xyz/gtlzndelqj.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtrcyytmxf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxuanxn.top/gtjcpquckt.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtgseququs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cdnleiting.top/gtjeskotrw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtqlkyosdo.html

JS:   console.error("err")
来源：http://hz.hysaishi.cn/gtxyikxsgf.html

TS:   console.error("err")
来源：http://hz.ehwqpu.com/gtqgkrnfaq.html

Java: System.err.println("err")
来源：http://hz.nwbrower.top/gtjxquotjy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.mhx1999.top/gtlndiibix.html

Ruby: warn "err"
来源：http://hz.52xcode.cn/gtdtvotyti.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gtdxwxbnev.html

[M07] 判断是否为主入口
来源：http://hz.c1oappe.top/gtxaocpznr.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtkojyhqzl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yangfankeji.com/gtvbaayljq.html

JS:   require.main === module
来源：http://hz.zhoulong.xyz/gtknodzywz.html

TS:   require.main === module
来源：http://hz.meibo888.top/gtuubxxssf.html

Java: public static void main(String[] args)
来源：http://hz.shzxlz.cn/gtcjadswgm.html

Go:   func main()
来源：http://hz.sxryk.cn/gtytzvnrev.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yanxiufei.cn/gtbuwsfbvo.html

C#:   static void Main(string[] args)
来源：http://hz.hysaishi.cn/gtpfvtjpde.html

[M08] 获取系统与运行时信息
来源：http://hz.gotoacloud.top/gtijzwveie.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nwbrower.top/gtrxpbvmtp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuetiantiany.cn/gtzttukpad.html

JS:   process.platform;  process.version
来源：http://hz.hammf.cn/gtwownuzuc.html

TS:   process.platform;  process.version
来源：http://hz.aizwys.cn/gtxlyenffd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ydzc1.top/gtbcspjxiv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pycfn.com/gtawowfaia.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cdnleiting.top/gtyeucxhbw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtketejzid.html

================================================================================
来源：http://hz.tianlin.xyz/gtagvxxulj.html

N. 数据结构与算法
来源：http://hz.nanxuanxn.top/gtpcubnfhe.html

================================================================================
来源：http://hz.xuanzx.com/gtqyzotcwr.html

[N01] 二分查找（有序数组）
来源：http://hz.ybcxt.top/gtlhzwwcqc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nanxuanxn.top/gttpkgrnhr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.52xcode.cn/gtbzgzbwny.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtkduubdue.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtwhfgddun.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtthqalqyw.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gttkgbhnjr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtffzkatjj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zycfv.cn/gtqnugyfyz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.tanke756.top/gthbabefrn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtdeqcatno.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenjidiqi.icu/gtsrjwstml.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sysykeji.top/gtyhuiaksz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtxqlwralg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xuetiantiany.cn/gtkfqcqspl.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtdhvzngwf.html

Ruby: arr.sort
来源：http://hz.ybcxt.top/gtcwasfkrp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yj20258888.top/gthpirnohq.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtjnugfmho.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yj20258.top/gtuqiobttg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtfmokphut.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yueranfly.top/gtofxljrbi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hfpthk.cn/gtwcvphgwe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.svipenyu.cn/gtzajmfxsb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.wangdashe.top/gtdgbfkvtx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.svipenyu.cn/gtelfecumz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.guannengcc.top/gtrvseplpk.html

[N04] 斐波那契数列
来源：http://hz.xingfuxueyuan.xyz/gthcmvsfaj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhixingplan.top/gtwqvrdxsa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sysykeji.top/gtysyedyqp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gtntcrlxkf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xuanzx.com/gtrytetxzj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shanyushiyangtech.top/gtletlymnz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.sufxvd.cn/gtbfzrgtbo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.shanyushiyangkeji.top/gtnfxlnmpp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtmkxgnhst.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gtuxpovjvr.html

Py:   math.gcd(a, b)
来源：http://hz.zdqjudy.top/gtdianodkl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hysaishi.cn/gtfjdrdxib.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.wangdashe.top/gtmmakddmd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.9152youxi.cn/gtvtdgihuu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hnqzz.top/gtzqqlfhpd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.nanxuanxn.top/gtpurtdmul.html

Ruby: a.gcd(b)
来源：http://hz.yonumen.top/gtqaludtbb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtlaegmymc.html

[N06] 判断回文字符串
来源：http://hz.sysykeji.top/gthhweroqm.html

Py:   s == s[::-1]
来源：http://hz.fzhhl.top/gtxdakrxmv.html

PHP:  $s === strrev($s);
来源：http://hz.nanxinkj.top/gtuvotqxfa.html

JS:   s === [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtznalmuqk.html

TS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gttgnbitzm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgfzy.top/gtccnhiimc.html

Go:   // 双指针从两端比较
来源：http://hz.tianlin.xyz/gtidyvjdgl.html

Ruby: s == s.reverse
来源：http://hz.hfpthk.cn/gtqqvmheal.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.kuanghao11.cn/gtbcjsooqp.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gthtnazlhd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.kuanghao11.cn/gtldrvgkem.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtjoadonbu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xinyue.icu/gtmtixbvct.html

TS:   // 手写 Map<string, number>
来源：http://hz.vqdsnc.cn/gtysmwxxuv.html

Java: // 手写 HashMap
来源：http://hz.yanxiufei.cn/gtgkracrow.html

Go:   // 手写 map[int]int
来源：http://hz.zhongyouzk.top/gtezgfixdw.html

Ruby: // 手写 Hash
来源：http://hz.cucudq.cn/gtfbgtqooq.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gttjaxwiuy.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtmxibbgtf.html

Py:   itertools.permutations(arr)
来源：http://hz.yonumen.top/gtxpwlijmc.html

PHP:  // 手写递归交换
来源：http://hz.zhijiandao.cn/gtyzzpnlat.html

JS:   // 手写回溯递归
来源：http://hz.xinyue.icu/gtkzvzwdwi.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtcqtoqrra.html

Java: // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtuwcgrmxw.html

Go:   // 手写回溯递归
来源：http://hz.jinqigfzy.top/gtqsdrmsqx.html

Ruby: arr.permutation.to_a
来源：http://hz.yanxiufei.cn/gtwexkngyp.html

C#:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtusypcczn.html

[N09] 栈与队列
来源：http://hz.9152youxi.cn/gtolvqbvnt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.nanxuanxn.top/gtnwaqutiu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.zhiwuduotai.top/gtsijjgsmz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jianghu66.top/gtdzvspubc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jiagoushi.top/gttkzxtaux.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhaomingkeji.xyz/gtvhtmfwbq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.vqdsnc.cn/gttqyqnpox.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.chenlongwang.top/gtffphkaay.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.zhiwuduotai.top/gtikyaergm.html

[N10] 链表节点定义
来源：http://hz.kuanghao11.cn/gthdyekkve.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.shanyushiyangtech.top/gtrutcifly.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.snrcjt.cn/gtdfjgnmni.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.iojbl.cn/gtorblnebp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.smart0.xyz/gtuvaoxchg.html

Java: class Node { int v; Node next; }
来源：http://hz.nwbrower.top/gtpbrmletl.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.cheryme.top/gtfnacmdzj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.daxiang520.top/gttetwvggj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.nanxinkj.top/gtzziawgsw.html

[N11] 二叉树中序遍历
来源：http://hz.52xcode.cn/gtcicqkwbn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.svipenyu.cn/gtbeiqbhkp.html

PHP:  // 手写递归函数
来源：http://hz.zhongyouzk.top/gtatdsyury.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yj202588.top/gtwmtcaoip.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.xziqi.cn/gthdxhivgb.html

Java: // 手写递归
来源：http://hz.xinyue.icu/gtnntnnnyt.html

Go:   // 手写递归
来源：http://hz.nanxinkj.top/gtswktysfm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.andypj.xyz/gtfbvleqaj.html

C#:   // 手写递归
来源：http://hz.yangfankeji.com/gtxthebitc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtxhmvqyrb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.daria6918.cn/gtknsqalmq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.ehwqpu.com/gtdwyeihig.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.shanyushiyangtech.top/gteigufyij.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gtvvuixnek.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.dianchejie.cn/gtqbvbdnmd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.gzhubu.top/gtelxolinq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.ydzc1.top/gtggyjewqe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.ydjk.org.cn/gtkozpuyaq.html

================================================================================
来源：http://hz.gzhubu.top/gtukrbrtam.html

O. 并发与异步
来源：http://hz.yj20258.top/gtbnxcpflt.html

================================================================================
来源：http://hz.yuanzhike.top/gtcpioydqg.html

[O01] 启动一个线程
来源：http://hz.zhiwuduotai.top/gtaypasalm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.shanyushiyangkeji.top/gtcyvpqlvx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yj20258888.top/gtfnvhyqut.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.tian-w.cn/gtirzusyst.html

TS:   // 同 JS
来源：http://hz.cashguo.top/gtkdndmsvf.html

Java: new Thread(() -> f()).start()
来源：http://hz.sweek.top/gtfijzjvoe.html

Go:   go f()
来源：http://hz.316326.xyz/gtnghouvdz.html

Ruby: Thread.new { f }
来源：http://hz.jiagoushi.top/gtpoopkykj.html

C#:   Task.Run(() => F());
来源：http://hz.andypj.xyz/gtiopbdgxr.html

[O02] 使用线程池
来源：http://hz.guowangkeji.top/gtspnktyhn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.gotoacloud.top/gtdxiaafvf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.zdqjudy.top/gthvtwtihi.html

JS:   // worker_threads 线程池
来源：http://hz.zhongyouzk.top/gtdskslwqb.html

TS:   // worker_threads 线程池
来源：http://hz.sysykeji.top/gtpdtjdsao.html

Java: Executors.newFixedThreadPool(4)
来源：http://hz.ehwqpu.com/gtdegxcjke.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hz.jyoumei.cn/gtjhgeteql.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hz.redwolf501.top/gtwfrlebjb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hz.jlsjyb.cn/gtrfmtnuir.html

[O03] 加锁保护共享数据
来源：http://hz.daria6918.cn/gtsbnhxrnu.html

Py:   with lock: shared += 1
来源：http://hz.haohaochexian.top/gtsqmifquq.html

PHP:  // 用 flock() 做文件锁
来源：http://hz.gzhubu.top/gtmqpkkzxb.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hz.snrcjt.cn/gtitmrdxzj.html

TS:   // 同 JS
来源：http://hz.guannengcc.top/gtpgosjgtt.html

Java: synchronized (this) { shared++; }
来源：http://hz.jinyuanbaomall.cn/gtffqbesed.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hz.ywan-chungtsiang.top/gtsrktwdlb.html


<!-- 参考信息 -->