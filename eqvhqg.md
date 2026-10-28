代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtqxlvbwuk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fzhhl.top/gtinqogfjp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtnfacmcpe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtpjgfnrxu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shuidangran.top/gtcmajyxqx.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtefrkfxhs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigfzy.top/gtfynrejrb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gogol.net.cn/gttjwvrkiu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtnvuerrtj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtuywbtlgg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtnrsnregy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sxryk.cn/gtrhpwequy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gttgoetlni.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gaohongyu789.top/gtooozfelk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yvedp.cn/gtnemuaska.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtnxqhfvqq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtmwjbyvlz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtljoqkpin.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtpotkwdvv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtasjmyljf.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gtgfptmzwu.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtbbjbqfmg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtefpyrdrd.html

================================================================================
来源：http://hz.dashuyun.cn/gtovozxzzl.html

L. 网络请求
来源：http://hz.guowangkeji.top/gtkjozhukg.html

================================================================================
来源：http://hz.guowangkeji.top/gtruwacniu.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtetkuhctg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtwzwqtpjq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtfgxaudru.html

JS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtbktdvwij.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtvqcoeqpu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtsfugisuy.html

Go:   resp, err := http.Get(url)
来源：http://hz.shuidangran.top/gtygyjudhw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fzhhl.top/gtwhkmjahq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtssbwkqss.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangtech.top/gtfdvztmxz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtaucvtuyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhiwuduotai.top/gtmvdghodj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtijtmuzzo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtausmvpvb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.316326.xyz/gtuonvvsmh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.birdmap.top/gtizoslmhk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hongshengwenyu.top/gtfumcajvx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtaitmxhha.html

[L03] 设置自定义请求头
来源：http://hz.jinqigufen.top/gtoyelnrcf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtlitczhrc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gtwqhtcaic.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtibtfpqni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenlongwang.top/gtrqldszmk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtmrikilnv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtrfmuoufo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgufenzy.top/gtihrqhota.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cqqwz.cn/gtkqphfkjk.html

[L04] 设置超时
来源：http://hz.hysaishi.cn/gtkyeyxtjz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hysaishi.cn/gtctsrpxbt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.meibo888.top/gtyvmagjhd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dashuyun.cn/gtzqmaraax.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtnioahrov.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.birdmap.top/gtejurneqt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shangyingyoupin.top/gtsdwbysrr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtsvthdlhx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtdzgnwljh.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtppprhuje.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuetiantiany.cn/gthfxfgrpl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtgqyrrzlr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gthygomcua.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gttwuksvim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.iojbl.cn/gtqdmwoqco.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daria6918.cn/gthfxuqjyl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtgmaelbei.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgufenzy.top/gtzwkuxacz.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtzhonjgoh.html

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gtxjputxhb.html

PHP:  json_decode($body, true);
来源：http://hz.svipenyu.cn/gtuimlarps.html

JS:   await resp.json()
来源：http://hz.fengsongda.top/gteretrgxx.html

TS:   await resp.json()
来源：http://hz.cdnleiting.top/gthdvvpqqb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtjqvfcjji.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtenefmxec.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydjk.org.cn/gtdldnivih.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cucudq.cn/gtzmvburgs.html

[L07] 处理 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtfwivdmun.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtpspyoqbp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtugsrydip.html

JS:   resp.ok;  resp.status
来源：http://hz.wangdashe.top/gtqokudhwx.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtcankeksx.html

Java: resp.statusCode()
来源：http://hz.yj202588.top/gtfrffsnjq.html

Go:   resp.StatusCode
来源：http://hz.shangyingyoupin.top/gtoiqnpekb.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtzfwhelju.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtgzzkdojt.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtfynocxcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cashguo.top/gtissiayef.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtkttnwzho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gtkyvyzdaw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gtebrorbry.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.haohaochexian.top/gtrcqbwhir.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jiagoushi.top/gtriykwbma.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.aibaodan.cn/gtxltilvqh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.smart0.xyz/gtpalzaqqc.html

================================================================================
来源：http://hz.chenzaomai.com/gtblxlvuzj.html

M. 命令行 / 进程 / 环境
来源：http://hz.tanke756.top/gtseydazxy.html

================================================================================
来源：http://hz.xylfe.cn/gthyshyvkp.html

[M01] 读取命令行参数
来源：http://hz.smart0.xyz/gtnnutazdh.html

Py:   sys.argv[1:]
来源：http://hz.daxiang520.top/gtfburgobs.html

PHP:  $argv;  $argc;
来源：http://hz.guannengcc.top/gtnqxzakej.html

JS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtmipfxoev.html

TS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtptdclhxf.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtfqpinsmt.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtaworrqfm.html

Ruby: ARGV
来源：http://hz.shangyingyoupin.top/gtgsjmbibr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258.top/gtnehxvwaw.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gtvjmmccrx.html

Py:   os.environ.get("HOME")
来源：http://hz.jianghu66.top/gtunqykefn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yuanzhike.top/gtcffxbfbe.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gtnnyyubbg.html

TS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtgqgnovqp.html

Java: System.getenv("HOME")
来源：http://hz.9152youxi.cn/gtcvicbjcg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fengsongda.top/gtyirrgxkn.html

Ruby: ENV["HOME"]
来源：http://hz.chenzaomai.com/gtjxluqygh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtskadcclz.html

[M03] 执行外部命令
来源：http://hz.zhixingplan.top/gtjavmejbh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtddhgwmgt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gteclamivg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtexlawwxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtflortdam.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nwbrower.top/gthlrwxnao.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhoulong.xyz/gtmzrqzljp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.nanxinkj.top/gtmyspoaur.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zycfv.cn/gtdreiedad.html

[M04] 获取当前工作目录
来源：http://hz.redwolf501.top/gthahplupk.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtjcdkakfa.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtpcrbfwph.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtsnqlwokj.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gthefwvxjx.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtogqxceey.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gtizudxjea.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gtekkmgusx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtjwicedaz.html

[M05] 设置退出码
来源：http://hz.yj20258.top/gtvpqxzgtl.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtmcyjzmlr.html

PHP:  exit(1);
来源：http://hz.xziqi.cn/gthyeqzrdl.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtdncxcalp.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gtozwnabpg.html

Java: System.exit(1)
来源：http://hz.jianghu66.top/gtaureeval.html

Go:   os.Exit(1)
来源：http://hz.xuanzx.com/gtpxhuijxe.html

Ruby: exit 1
来源：http://hz.hywenlv.cn/gtuuchqsne.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xylfe.cn/gtwxqjvzbd.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gthmyclyaa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhaomingkeji.xyz/gtmqvpbgda.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gotoacloud.top/gtbqpdzhqn.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtedkbpnvk.html

TS:   console.error("err")
来源：http://hz.pycfn.com/gttakpcnjv.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtdsdiqjbg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.havefunace.top/gtpnbiyyqy.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtqyouchkp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtfodkquzm.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtofavtcst.html

Py:   if __name__ == "__main__":
来源：http://hz.zhengqikj.top/gtdqhcckfo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.guannengcc.top/gtvvoxfubk.html

JS:   require.main === module
来源：http://hz.yongpay.top/gtgkqfftih.html

TS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gtnbdzoymx.html

Java: public static void main(String[] args)
来源：http://hz.bjfxy.top/gtyfysuyid.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtdeknybsb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.fengsongda.top/gtqplxfweh.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtsuactgan.html

[M08] 获取系统与运行时信息
来源：http://hz.zhongyouzk.top/gtccmeyzod.html

Py:   platform.system();  platform.python_version()
来源：http://hz.bjfxy.top/gtdklgbvxt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtreydqvop.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtxesryoet.html

TS:   process.platform;  process.version
来源：http://hz.ywan-chungtsiang.top/gtpbrodgkq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtwnsdmpcd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ivvv.top/gtfxtmspzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtbknlbhjn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hywenlv.cn/gttdqqegod.html

================================================================================
来源：http://hz.mhx1999.top/gtahqscgcd.html

N. 数据结构与算法
来源：http://hz.haohaochexian.top/gtkuaahysq.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtchhriiha.html

[N01] 二分查找（有序数组）
来源：http://hz.hammf.cn/gtxlamkgxt.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.cashguo.top/gtnufoazkt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dianchejie.cn/gtgniwtejy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ivvv.top/gtlmzechnk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.dianchejie.cn/gtpppilxom.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtlesxbdeh.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtiqgiouyq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.andypj.xyz/gtyxhphzdx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.svipenyu.cn/gtlynmlcdz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sysykeji.top/gtnhrfbvix.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gtqpkmjeun.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigfzy.top/gtijjfghjc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hammf.cn/gtaxvajreo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtfyvdzjwk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yanxiufei.cn/gtbnouosfn.html

Go:   slices.Sort(arr)
来源：http://hz.zhijiandao.cn/gtxkdptmsr.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtemiyimmv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtvpzerkng.html

[N03] 快速排序（分治示例）
来源：http://hz.hywenlv.cn/gtzwefgnmf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydzc1.top/gtfdsvmicc.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jinqigufen.top/gtzadbcuev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gtjuequdjd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.sweek.top/gtpiciaxzd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtlvmduxdu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtdkribbnk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shangyingyoupin.top/gtovjkghqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tianlin.xyz/gtyzwttodb.html

[N04] 斐波那契数列
来源：http://hz.jyoumei.cn/gthyqstlmb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xuanzx.com/gtwmxbkcwk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gttjbeczht.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtfsnzotjc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.mhx1999.top/gttcyiijcj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.gogol.net.cn/gtqncontzn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.mhx1999.top/gtemoxlcah.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yangfankeji.com/gtnrylpnpe.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.sweek.top/gtgizuduhp.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gthbxsjtfp.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtqonldpnq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangshuangyany.cn/gtveierfug.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hammf.cn/gtvjrczfxg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gttwbdqpmq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.kuanghao11.cn/gtqttouajj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fengsongda.top/gtmqtivbui.html

Ruby: a.gcd(b)
来源：http://hz.cucudq.cn/gtmboabiug.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.c1oappe.top/gtqxtxorvt.html

[N06] 判断回文字符串
来源：http://hz.zhijiandao.cn/gtjftophbc.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtpofkjvhy.html

PHP:  $s === strrev($s);
来源：http://hz.jqgufenzy.top/gtemqejmbk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtxjfqwaer.html

TS:   s === [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtsapzyejc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gtagzqbnlh.html

Go:   // 双指针从两端比较
来源：http://hz.iojbl.cn/gtvcvefkba.html

Ruby: s == s.reverse
来源：http://hz.fengsongda.top/gtleuyehzf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtkwezkkns.html

[N07] 两数之和（返回下标）
来源：http://hz.9152youxi.cn/gtnpqzyjll.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xziqi.cn/gtywicsvry.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shzxlz.cn/gtlhfijipg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxuanxn.top/gtolqpsanj.html

TS:   // 手写 Map<string, number>
来源：http://hz.fengsongda.top/gtzkfcufcz.html

Java: // 手写 HashMap
来源：http://hz.dianchejie.cn/gtbrolrebl.html

Go:   // 手写 map[int]int
来源：http://hz.jyoumei.cn/gtkbesxbvg.html

Ruby: // 手写 Hash
来源：http://hz.shzxlz.cn/gtqjmoqbdi.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yvedp.cn/gtxrkrhxnn.html

[N08] 生成全排列
来源：http://hz.dianchejie.cn/gtrpyfqplz.html

Py:   itertools.permutations(arr)
来源：http://hz.quarkkingdee.top/gtiqwpurbt.html

PHP:  // 手写递归交换
来源：http://hz.mhx1999.top/gtohnybqzb.html

JS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtrakoguul.html

TS:   // 手写回溯递归
来源：http://hz.zhixingplan.top/gtdxsqajfo.html

Java: // 手写回溯递归
来源：http://hz.sweek.top/gtjqqvgfre.html

Go:   // 手写回溯递归
来源：http://hz.zhiwuduotai.top/gtvbnnzega.html

Ruby: arr.permutation.to_a
来源：http://hz.daria6918.cn/gtarpgkioq.html

C#:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtqchojxyh.html

[N09] 栈与队列
来源：http://hz.xuetiantiany.cn/gtukavoyor.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hnxiangtu.top/gtmnxxzmdm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtfteiquqe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.sweek.top/gtcxbxoovq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daxiang520.top/gtfkgqpcrb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.zhixingplan.top/gtpvfxnqzt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhaomingkeji.xyz/gtxrmdqvfg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jqgufenzy.top/gtjenuznxp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtedeveidk.html

[N10] 链表节点定义
来源：http://hz.yonumen.top/gtlqgodhsz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.yj20258.top/gtzubqnpbb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xziqi.cn/gtxmfolxdk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhongyouzk.top/gtjskcuygf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.xuetiantiany.cn/gtuloqizrw.html

Java: class Node { int v; Node next; }
来源：http://hz.316326.xyz/gtpfskbgxb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yuanzhike.top/gtyvwwheqw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zdqjudy.top/gtmcpdasww.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.chenjidiqi.icu/gtadslqszq.html

[N11] 二叉树中序遍历
来源：http://hz.aizwys.cn/gtnokymtbh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.shanyushiyangkeji.top/gtukemgmao.html

PHP:  // 手写递归函数
来源：http://hz.zhengqikj.top/gtleiovuck.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.iojbl.cn/gtmqjqewhv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.gotoacloud.top/gtcwdzjnvg.html

Java: // 手写递归
来源：http://hz.316326.xyz/gtjhuyexuw.html

Go:   // 手写递归
来源：http://hz.fengsongda.top/gtnsfhbjsf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.gogol.net.cn/gtgauspbit.html

C#:   // 手写递归
来源：http://hz.jianghu66.top/gtbngbjsce.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.xinyue.icu/gtfbgutdxz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.quarkkingdee.top/gtuxuffnpr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhengqikj.top/gtoyevgbel.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.redwolf501.top/gtdvpmvjna.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.hnqzz.top/gtkgsevmtd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yueranfly.top/gtenpxqikm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.nwbrower.top/gtfpqkqwei.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jinqigufen.top/gtvwkhsnlw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.daria6918.cn/gtogdeoayr.html

================================================================================
来源：http://hz.guowangkeji.top/gtpwgsprdo.html

O. 并发与异步
来源：http://hz.jqgufenzy.top/gtoxukzzrt.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsmguwntw.html

[O01] 启动一个线程
来源：http://hz.yj20258888.top/gtgvjkapll.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.jinyuanbaomall.cn/gthrrhdwpf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.yangfankeji.com/gtdjxmflti.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.gogol.net.cn/gtejkactee.html

TS:   // 同 JS
来源：http://hz.yangfankeji.com/gtplitfbno.html

Java: new Thread(() -> f()).start()
来源：http://hz.xziqi.cn/gtiiosaruv.html

Go:   go f()
来源：http://hz.gaohongyu789.top/gtpdzskyoq.html

Ruby: Thread.new { f }
来源：http://hz.sysykeji.top/gtkncetpjk.html

C#:   Task.Run(() => F());
来源：http://hz.sxryk.cn/gtqhhechzm.html

[O02] 使用线程池
来源：http://hz.zdqjudy.top/gtbvsajufu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.guannengcc.top/gtyrbrnaqy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.nanxinkj.top/gtrooyybod.html

JS:   // worker_threads 线程池
来源：http://hz.jqgfzy.top/gtfstkixia.html


<!-- 参考信息 -->