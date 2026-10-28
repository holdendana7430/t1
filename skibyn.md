代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.vqdsnc.cn/gtmogslzbj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtuprsfrtt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gthyjykdim.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtjdkboctt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtabcegqki.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtjdopcezl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gtwobcuzol.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtwwvrpdnz.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtglljgmob.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtusdmrtic.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gthfvbzhfy.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtwxybbdqx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yangfankeji.com/gtqdwjyydd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtomdwzchw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtedwtfirq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtrovuawde.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtvrmuzjpo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhoulong.xyz/gtibaggibw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tianlin.xyz/gtffcegkuc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtjogstfrc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtizrkefkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtyfbkcoec.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cashguo.top/gthsiqywqb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtsielgsjw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtnmlogpda.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtcdnslqwq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtxdysxxmu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gtgfwgohbg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gttycpbjll.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtqwsaebqw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtpzastfjz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtrnbprxue.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtoddgifja.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtbdalhtfb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtqscidipi.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtpoxsigdx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gthebwmjkw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cqqwz.cn/gttjnvccrz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtlgudscov.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.quarkkingdee.top/gtevzdecmx.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtkmazlcsi.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gtalrvjvvk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtbiqbujkf.html

================================================================================
来源：http://hz.gzhubu.top/gtlamnmmzo.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtovlxhfpl.html

================================================================================
来源：http://hz.sufxvd.cn/gtguserjbi.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtomwodqlg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtkvnqapop.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gtisuqfmkd.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtbuwrbtmy.html

TS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtwlhitsqj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daria6918.cn/gtocnqmsdp.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtauywlanz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtwnbfrwoe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gaohongyu789.top/gtlmxctvdr.html

[L02] 发送 POST JSON
来源：http://hz.shzxlz.cn/gtfljcjuzn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yanxiufei.cn/gtpzwpfzax.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yvedp.cn/gtamokmzew.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtcgwfznni.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtrovpterf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtknlevxhr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtbasqavbz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gthfzsgyqx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtfsnuxgyy.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtrstpitqq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yvedp.cn/gtgkcspcvy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yueranfly.top/gtkehmcfms.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.guannengcc.top/gtcgsdjynf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtahrcwgxx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtiudgcbpt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xziqi.cn/gtwviytwwd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.9152youxi.cn/gtkijriskf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.iojbl.cn/gtyeyfbxkg.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtfisidcao.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtghaflque.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cheryme.top/gtvveikjfk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtoqflumnp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtqgsxzqgc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenlongwang.top/gtbdaoager.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gtfycavtmh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.havefunace.top/gtexzrgnbg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jianghu66.top/gtgrsdexfz.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtssubciai.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.sweek.top/gtkxecylkw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jyoumei.cn/gtmescbofy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtqhvmtkhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtgoatahzr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtwpjbajfx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gtoinnnwky.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xuetiantiany.cn/gtqlqlifwq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtmzhomqwd.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gtksxwqznq.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gttzrsfrqy.html

PHP:  json_decode($body, true);
来源：http://hz.ppjwa.cn/gtomgoglsx.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtluiexkrv.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtyzdhoovy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gtxzqkgjvd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gthhxgzldn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.svipenyu.cn/gtfhpyzqoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtgwnabsbc.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gtxkorxulh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.9152youxi.cn/gtrezvfhmf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenlongwang.top/gtdrhqacgb.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gthahxsith.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtxumvovfx.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtcsfzcttc.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gthdygdhjh.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtpskumbaw.html

C#:   (int)resp.StatusCode
来源：http://hz.ybcxt.top/gtcyasfxzs.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtqrclgvfr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtmgvbuzwc.html

PHP:  curl_multi_init() 系列
来源：http://hz.andypj.xyz/gtoukfycbt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtqijtzall.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gogol.net.cn/gtmgldekve.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.quarkkingdee.top/gtrgcxstje.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtfgczkwyv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtrxgebpvt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtuyeevjtp.html

================================================================================
来源：http://hz.cashguo.top/gtyopvcsvs.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtjeqsynwu.html

================================================================================
来源：http://hz.daria6918.cn/gtbsirhrha.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtjpbzrukh.html

Py:   sys.argv[1:]
来源：http://hz.ppjwa.cn/gtrerioyul.html

PHP:  $argv;  $argc;
来源：http://hz.yuxming.cn/gtytkbvggg.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtegigkgec.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtbfezebuw.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtfowfdhqo.html

Go:   os.Args[1:]
来源：http://hz.dianchejie.cn/gtijvsuylf.html

Ruby: ARGV
来源：http://hz.xinyue.icu/gtngjqtpaz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtokajltao.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtcgsospsu.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gttozndfjh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinqigufen.top/gtteppnblh.html

JS:   process.env.HOME
来源：http://hz.hnqzz.top/gthmlwypbb.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtmnlugaun.html

Java: System.getenv("HOME")
来源：http://hz.yanxiufei.cn/gtauwhmizt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xylfe.cn/gtrpwsbhfp.html

Ruby: ENV["HOME"]
来源：http://hz.quarkkingdee.top/gtgiabkxls.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhengqikj.top/gtikzzncfr.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtfzdyipra.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.kuanghao11.cn/gtifnmdiuz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yvedp.cn/gtifanczsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xziqi.cn/gtjiqjqviw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtgdxynnre.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj202588.top/gthfpmuyfp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yongpay.top/gtjuonghou.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xingfuxueyuan.xyz/gtudynefif.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtvkztiusn.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtrukoiwbh.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtepmgahxn.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gteqlzorew.html

JS:   process.cwd()
来源：http://hz.dashuyun.cn/gtthgssrpp.html

TS:   process.cwd()
来源：http://hz.zhaomingkeji.xyz/gtmyljtlzr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gttgrbfwlp.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gtvcfqqali.html

Ruby: Dir.pwd
来源：http://hz.ydzc1.top/gthtveckod.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ppjwa.cn/gtnxzkqumf.html

[M05] 设置退出码
来源：http://hz.dashuyun.cn/gtowkevhqv.html

Py:   sys.exit(1)
来源：http://hz.birdmap.top/gtkrmibgxu.html

PHP:  exit(1);
来源：http://hz.zhixingplan.top/gtplhisbjc.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtbgmwrzqh.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtrlrredcn.html

Java: System.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtuazelctt.html

Go:   os.Exit(1)
来源：http://hz.shangyingyoupin.top/gtcedappza.html

Ruby: exit 1
来源：http://hz.tian-w.cn/gtqtoeimnz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.daria6918.cn/gtiiopgxxb.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtgwjkdmcn.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtqvzdrezm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.quarkkingdee.top/gtpslzeryk.html

JS:   console.error("err")
来源：http://hz.cdnleiting.top/gtqutztwrv.html

TS:   console.error("err")
来源：http://hz.daxiang520.top/gtagdagghe.html

Java: System.err.println("err")
来源：http://hz.xuanzx.com/gtzciptnng.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtuyhyacdq.html

Ruby: warn "err"
来源：http://hz.yonumen.top/gtesfjfaoh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nwbrower.top/gtrypmfltn.html

[M07] 判断是否为主入口
来源：http://hz.yanxiufei.cn/gtvttzpwvm.html

Py:   if __name__ == "__main__":
来源：http://hz.yueranfly.top/gtiwuaatns.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tianlin.xyz/gtewblarcx.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gtteuatfle.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtjlxgqhwn.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gtectzhhep.html

Go:   func main()
来源：http://hz.jqgfzy.top/gttlpjunyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.feifeiyinyue.top/gtujmrteov.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtosxwdqbw.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtbmqusfxl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.feifeiyinyue.top/gtaxiumysk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhiwuduotai.top/gtievmwyta.html

JS:   process.platform;  process.version
来源：http://hz.zdqjudy.top/gtbsjbrlok.html

TS:   process.platform;  process.version
来源：http://hz.andypj.xyz/gtehjyghpe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yangfankeji.com/gtbrjlbcov.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.52xcode.cn/gtjjfjdyzm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hysaishi.cn/gtpdbjjpxj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ydzc1.top/gtznetwifc.html

================================================================================
来源：http://hz.pycfn.com/gtzggjfzvl.html

N. 数据结构与算法
来源：http://hz.mhx1999.top/gttfkkmhcr.html

================================================================================
来源：http://hz.ydjk.org.cn/gtoaoaacjg.html

[N01] 二分查找（有序数组）
来源：http://hz.cucudq.cn/gtntmrbyuj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hammf.cn/gtekdqxmtc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtquoilgda.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtqxbkouwr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gtqhmvzbvz.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtdlxrbbao.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.tian-w.cn/gtfeurzynf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.svipenyu.cn/gtrqhqaqsb.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtpfkjnwhb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sxryk.cn/gtgssbvhrp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtugjvvbrx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtooiafpjt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtpjeqceey.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtnquyrilw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ehwqpu.com/gtolqmegjr.html

Go:   slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtvisyispx.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtfqturbig.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.haohaochexian.top/gtkpsnfhcv.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtyguyevbc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.kuanghao11.cn/gtpxqomixw.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gaohongyu789.top/gtxkguqdfd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxinkj.top/gttlaruqcb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jiagoushi.top/gtdmhfjgkr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hammf.cn/gtatzjavam.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtwojwbqqd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.aibaodan.cn/gtwvqnmukv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.snrcjt.cn/gtqrneihnl.html

[N04] 斐波那契数列
来源：http://hz.cheryme.top/gtkurhubbg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtyvqhfftm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zycfv.cn/gtjrjhgfca.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yonumen.top/gttmxxnaza.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gttjintspc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hongshengwenyu.top/gtktxibgfg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shanyushiyangkeji.top/gtlcixssim.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtgzeykmzo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtnbeuxkab.html

[N05] 最大公约数
来源：http://hz.svipenyu.cn/gtduitoppa.html

Py:   math.gcd(a, b)
来源：http://hz.jinyuanbaomall.cn/gtaapdnvft.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtdhkluvxh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.svipenyu.cn/gtnbqrcenp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtixthhnta.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.yj20258.top/gtpliqflok.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.mhx1999.top/gtueitpefy.html

Ruby: a.gcd(b)
来源：http://hz.dashuyun.cn/gtaunbzewo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtkoundtvh.html

[N06] 判断回文字符串
来源：http://hz.feifeiyinyue.top/gtcrvqdkxp.html

Py:   s == s[::-1]
来源：http://hz.meibo888.top/gturcatppq.html

PHP:  $s === strrev($s);
来源：http://hz.ivvv.top/gttsbojska.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj20258.top/gtlmgwdgyh.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtzpvijybd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.mhx1999.top/gtoqbcbhve.html

Go:   // 双指针从两端比较
来源：http://hz.sysykeji.top/gtpujwidew.html

Ruby: s == s.reverse
来源：http://hz.hongshengwenyu.top/gtuwhrzoml.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtzjiraqze.html

[N07] 两数之和（返回下标）
来源：http://hz.316326.xyz/gtqbqvcpan.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jinqigfzy.top/gtkjgrkjdg.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.sweek.top/gtfcjghgsa.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.wangshuangyany.cn/gtrmqfhoaq.html

TS:   // 手写 Map<string, number>
来源：http://hz.cucudq.cn/gtzvexbcpl.html

Java: // 手写 HashMap
来源：http://hz.jlsjyb.cn/gtmklnkbdf.html

Go:   // 手写 map[int]int
来源：http://hz.xuetiantiany.cn/gterdvqttl.html

Ruby: // 手写 Hash
来源：http://hz.mhx1999.top/gtfoadhwot.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.aibaodan.cn/gtylxrhxkg.html

[N08] 生成全排列
来源：http://hz.shanyushiyangkeji.top/gtsajqtutx.html

Py:   itertools.permutations(arr)
来源：http://hz.hfpthk.cn/gttfdhmjgn.html

PHP:  // 手写递归交换
来源：http://hz.zycfv.cn/gtllqbmmcv.html

JS:   // 手写回溯递归
来源：http://hz.hnqzz.top/gtbnpmtmor.html

TS:   // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtgiidtdrt.html

Java: // 手写回溯递归
来源：http://hz.jinyuanbaomall.cn/gtuxaxketd.html

Go:   // 手写回溯递归
来源：http://hz.sufxvd.cn/gtqgjdqwch.html

Ruby: arr.permutation.to_a
来源：http://hz.fzhhl.top/gtqnqlifor.html

C#:   // 手写回溯递归
来源：http://hz.jinghuilouyu.cn/gtzksoilzz.html

[N09] 栈与队列
来源：http://hz.shanyushiyangtech.top/gtwpbfwcsa.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.jiagoushi.top/gtszvtwkbo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.52xcode.cn/gtjqnsjyiw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.tian-w.cn/gtcuvjqrsu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zhengqikj.top/gtwgntisrt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yangfankeji.com/gtvjjmqyll.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.316326.xyz/gtpkfohxkd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.jyoumei.cn/gtvpkrmpdr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.wangshuangyany.cn/gthlitkymd.html

[N10] 链表节点定义
来源：http://hz.xingfuxueyuan.xyz/gttbvxkcyp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.mhx1999.top/gtmvdmslzt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtuxxqqnha.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhengqikj.top/gtfeaayudi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dashuyun.cn/gtktmsbyir.html

Java: class Node { int v; Node next; }
来源：http://hz.jyoumei.cn/gtcjylvsha.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.fzhhl.top/gtcoelokku.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.andypj.xyz/gtruqxgrrf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.yueranfly.top/gtzqrdfibw.html

[N11] 二叉树中序遍历
来源：http://hz.ywan-chungtsiang.top/gtgxifnprb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.yongpay.top/gtacqjfvqi.html

PHP:  // 手写递归函数
来源：http://hz.fzhhl.top/gtvaavoctf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.tanke756.top/gtdzgpibvi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.nwbrower.top/gtmgsezfti.html

Java: // 手写递归
来源：http://hz.redwolf501.top/gtfrpdtuqr.html

Go:   // 手写递归
来源：http://hz.ppjwa.cn/gtqqqdftrj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.zhaomingkeji.xyz/gtcdjxcpyx.html

C#:   // 手写递归
来源：http://hz.pengpengdd.cyou/gtpemohkrr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yj20258888.top/gtydljnccw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.aizwys.cn/gtjfnmmttc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.hnxiangtu.top/gtjqwmlrqg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.tanke756.top/gtbwwutfha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.chenzaomai.com/gtyonsylme.html


<!-- 参考信息 -->