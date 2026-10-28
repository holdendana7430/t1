代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtvfkweqzb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtwbxsjalj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtohlbbmth.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtbmwadgib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtiakhorpe.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigfzy.top/gtdlybtrpo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtfzdhdvfq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtgreuamfr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtsfonzsxn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtrxtvfjut.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gtqpegvwht.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtdjdxtina.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtjgxevcfv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtpoikadcr.html

[K04] 读取 JSON 文件
来源：http://hz.mhx1999.top/gtevqhoupw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtibaxgpof.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtotdczqpq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtusshnnby.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtlohrbwan.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtlaezwxyl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtsahiwyst.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sysykeji.top/gtjmvphbqi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtivmkbmig.html

[K05] 深拷贝对象
来源：http://hz.52xcode.cn/gtdlhbjnoc.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtcmhnrvdn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtleeqqhkj.html

JS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtodnaidko.html

TS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtmivpwfas.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtrcddjdrq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtwhdvfirg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtkdilltap.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtyofrbzbl.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtpxbnjqeq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtdtajbijl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtfubmrlqh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtgkvkxdsc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sysykeji.top/gtavggfnly.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtyrgfgciq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtuxolgoua.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gterememdd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtaajbprje.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtqiarvyjx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtptyqpvwk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtjobvnhdn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtydeogjaf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtqoeyuyki.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtsnalqfxl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtzbtkeetw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtbtawxiwg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guannengcc.top/gternovkrk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtvgnmtqdo.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtwipgixwa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gaohongyu789.top/gtedilzwde.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtgdcwuptx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtewufetlc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtweysprxc.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtksuoyfmi.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtemeqtqbb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guannengcc.top/gtztsjczjr.html

================================================================================
来源：http://hz.zhoulong.xyz/gtwqlkyhtf.html

L. 网络请求
来源：http://hz.fengsongda.top/gtbpvdwyhm.html

================================================================================
来源：http://hz.gotoacloud.top/gttjpkfbss.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtvnmxmipj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtviuznfvc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtglkgtwqf.html

JS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtaxsnxxlc.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtryitgwfv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenjidiqi.icu/gtwcjhglji.html

Go:   resp, err := http.Get(url)
来源：http://hz.cdnleiting.top/gtrtkgxypi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yangfankeji.com/gtungfkiyi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gthiybgezk.html

[L02] 发送 POST JSON
来源：http://hz.yueranfly.top/gtlgrrdldb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtabgagdmb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gtdtvzbrrq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gthcqxooea.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtdwmgyjyg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtqwyniqld.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gteyhdqbge.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.vqdsnc.cn/gtpxuymxnj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yonumen.top/gtqgpptdui.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtuwdjbksd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtuqpxxqgd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gteoidrbei.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gtneopgeel.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtxpfacurz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jqgufenzy.top/gtcckyupzg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.9152youxi.cn/gtahfpjwwp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gtjpofxtdj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gthhvxuwxt.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gthxmyuenm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cucudq.cn/gtsnakeowf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtghxysguw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hysaishi.cn/gtvbdhksip.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtadwutyij.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zdqjudy.top/gtownxsyff.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gthvsfggiq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gtiodzxkfh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shangyingyoupin.top/gtcigbshrb.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gtgwadqdea.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jlsjyb.cn/gtyxioswvb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtazgywgoa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gtrihaqipk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yongpay.top/gtqvmdgpbn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtxpkqtwzb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtbytwmqly.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtbmfuqxdi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenjidiqi.icu/gtgpmcafoy.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtnmgqmklf.html

Py:   resp.json()
来源：http://hz.cucudq.cn/gtjqzdlkli.html

PHP:  json_decode($body, true);
来源：http://hz.cucudq.cn/gtvidtxuvt.html

JS:   await resp.json()
来源：http://hz.9152youxi.cn/gtqdbtevtk.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtbacuetcn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gtklldjkut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtsrmaajsz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.kuanghao11.cn/gteyhmmoiy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtypabxeyn.html

[L07] 处理 HTTP 状态码
来源：http://hz.iojbl.cn/gtyahjsmjk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.mhx1999.top/gtctbjjolk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtvznatmnd.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtaczwzjuw.html

TS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtumxjpzaq.html

Java: resp.statusCode()
来源：http://hz.jyoumei.cn/gtsfseetzi.html

Go:   resp.StatusCode
来源：http://hz.havefunace.top/gttcxculkg.html

Ruby: resp.code.to_i
来源：http://hz.xingfuxueyuan.xyz/gtunzqkuzk.html

C#:   (int)resp.StatusCode
来源：http://hz.hfpthk.cn/gtuhthynyx.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtvpwdplae.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangshuangyany.cn/gtpmyivjeq.html

PHP:  curl_multi_init() 系列
来源：http://hz.pengpengdd.cyou/gtfpcnoass.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yueranfly.top/gtxghcridy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtmglfzjxy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gtuamkvpci.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtlsthliqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtmlanxnbf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.daria6918.cn/gtnteoimuc.html

================================================================================
来源：http://hz.guannengcc.top/gtpyauzwfb.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gtqmxdklak.html

================================================================================
来源：http://hz.meibo888.top/gtdrhkawpa.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtmnpvswtq.html

Py:   sys.argv[1:]
来源：http://hz.zycfv.cn/gtzhlflvug.html

PHP:  $argv;  $argc;
来源：http://hz.shuidangran.top/gtzurahovf.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gttrxkrvyk.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtruenycmh.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtipwheuid.html

Go:   os.Args[1:]
来源：http://hz.aibaodan.cn/gtzsmfdblg.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtnyjvdqmt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aibaodan.cn/gtohgjixne.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtuqnvjlsa.html

Py:   os.environ.get("HOME")
来源：http://hz.yj202588.top/gtafrsrkdv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gttnhvafxs.html

JS:   process.env.HOME
来源：http://hz.gogol.net.cn/gtypjghffo.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtovmlkeet.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtwhkefzuc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aizwys.cn/gtvkhoxdcd.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258.top/gtdkwvbgxb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.redwolf501.top/gtlmxatgyo.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtgzgmwlcb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtqwdxlzek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtgkwbknei.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtbbnzegbj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtmlhanpoz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtvjcgxlun.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gttaudermu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.havefunace.top/gtwrmsotwj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtdejkciku.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gtyizkyyon.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtgqnlenyv.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gthntnmzbd.html

JS:   process.cwd()
来源：http://hz.zycfv.cn/gtakhsttdn.html

TS:   process.cwd()
来源：http://hz.jianghu66.top/gtwsxaovro.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtlstdlrog.html

Go:   os.Getwd()
来源：http://hz.tanke756.top/gtdxloanxj.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtmmjtmbfd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtdcaaeinp.html

[M05] 设置退出码
来源：http://hz.aizwys.cn/gtidjihkbe.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtgtyulgwh.html

PHP:  exit(1);
来源：http://hz.52xcode.cn/gttgdttuiz.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtnohhtiqf.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtdigaderz.html

Java: System.exit(1)
来源：http://hz.tianlin.xyz/gtnppemtvl.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtxzpmzmlz.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtqwcbbsbt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sufxvd.cn/gtovzttmkx.html

[M06] 向标准错误输出
来源：http://hz.daria6918.cn/gtuanommui.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yangfankeji.com/gtmzakrzmz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtrwhriscx.html

JS:   console.error("err")
来源：http://hz.gzhubu.top/gtfseelyve.html

TS:   console.error("err")
来源：http://hz.andypj.xyz/gtkdclijlm.html

Java: System.err.println("err")
来源：http://hz.yuanzhike.top/gtdyowdwpn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.smart0.xyz/gtjtbaakyu.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gthaeseahx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtlsdturrt.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtwvjdtkxd.html

Py:   if __name__ == "__main__":
来源：http://hz.sweek.top/gtnlwpceiy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sysykeji.top/gtddygmknm.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtrxnxcdzp.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtfarcuxxy.html

Java: public static void main(String[] args)
来源：http://hz.jinyuanbaomall.cn/gtmjjlytye.html

Go:   func main()
来源：http://hz.nwbrower.top/gtcmmomlop.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.shanyushiyangkeji.top/gtzgkbwggr.html

C#:   static void Main(string[] args)
来源：http://hz.yj202588.top/gtwapegvad.html

[M08] 获取系统与运行时信息
来源：http://hz.feifeiyinyue.top/gtsxvvdlah.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guowangkeji.top/gtmzmsbohw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnqzz.top/gtscgqphpt.html

JS:   process.platform;  process.version
来源：http://hz.hnxiangtu.top/gtytzwcmml.html

TS:   process.platform;  process.version
来源：http://hz.shzxlz.cn/gtxoeluyjf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtvzktjlpv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.wangdashe.top/gtsmebxcjc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ehwqpu.com/gtsyuccaew.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gtmozfkktl.html

================================================================================
来源：http://hz.xuanzx.com/gttzybqpom.html

N. 数据结构与算法
来源：http://hz.ywan-chungtsiang.top/gtdbtfkerf.html

================================================================================
来源：http://hz.hywenlv.cn/gttcabqwqz.html

[N01] 二分查找（有序数组）
来源：http://hz.dianchejie.cn/gtbsnqhvfi.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yuxming.cn/gtrrzrborq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtxuggsmpl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.havefunace.top/gtdpficwvn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtoxmifgha.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangkeji.top/gtjqjmnbzp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.meibo888.top/gtxtsdoqql.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtghnfntfo.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yangfankeji.com/gtthpryemd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dashuyun.cn/gttqbftghf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtwpqawawj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtilufizyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ppjwa.cn/gtylplqadw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangdashe.top/gtykzplptx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtxpbxzmcd.html

Go:   slices.Sort(arr)
来源：http://hz.zdqjudy.top/gtduqcnhmg.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtkwvccnrd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ybcxt.top/gtebsgxmaw.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtuvvvbwnz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ivvv.top/gtsketrjaz.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sxryk.cn/gtrfxxwocx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtsfeuuawi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ehwqpu.com/gtysplsyro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shzxlz.cn/gtixjlyzjz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cdnleiting.top/gtemkklicu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxuanxn.top/gtaqvmesqe.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.jqgufenzy.top/gtpdqgnpex.html

[N04] 斐波那契数列
来源：http://hz.gotoacloud.top/gtoxtxabhb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shuidangran.top/gtingmgejr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xylfe.cn/gtlnqzbwlk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cucudq.cn/gtxnhrijvi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gthrenadnl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtoggyjnnj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.snrcjt.cn/gtrzvkmsjt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtzhtkkbpt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yuanzhike.top/gthhjlctui.html

[N05] 最大公约数
来源：http://hz.yanxiufei.cn/gtopzkugbv.html

Py:   math.gcd(a, b)
来源：http://hz.dianchejie.cn/gtaqlvyzgt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.fengsongda.top/gtleujxnmj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtodbddhpk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtbtfjuitk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jyoumei.cn/gtyotkcqfj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.xingfuxueyuan.xyz/gtuxuocgvo.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtddlnsexk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.snrcjt.cn/gtoswjuabz.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtanehgupo.html

Py:   s == s[::-1]
来源：http://hz.zhijiandao.cn/gtsplnuddx.html

PHP:  $s === strrev($s);
来源：http://hz.meibo888.top/gtyfknxdmn.html

JS:   s === [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtvazihsvy.html

TS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtfahdpzvk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cashguo.top/gtvpvcdgeq.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtwflqowxv.html

Ruby: s == s.reverse
来源：http://hz.ybcxt.top/gtxwtswzju.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtekkfacmu.html

[N07] 两数之和（返回下标）
来源：http://hz.hongshengwenyu.top/gtktnevqwd.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj202588.top/gtrexlhoqe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.quarkkingdee.top/gtxfgvujdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.sxryk.cn/gtjhmdclly.html

TS:   // 手写 Map<string, number>
来源：http://hz.yuanzhike.top/gtkfteephb.html

Java: // 手写 HashMap
来源：http://hz.0kj1m.cn/gtvqtparnh.html

Go:   // 手写 map[int]int
来源：http://hz.havefunace.top/gttyytdazc.html

Ruby: // 手写 Hash
来源：http://hz.jinqigfzy.top/gtrpwvogrv.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.redwolf501.top/gtkasvirga.html

[N08] 生成全排列
来源：http://hz.hywenlv.cn/gtawtsbelt.html

Py:   itertools.permutations(arr)
来源：http://hz.shanyushiyangkeji.top/gtpqbislzn.html

PHP:  // 手写递归交换
来源：http://hz.bjfxy.top/gtehgfiwsl.html

JS:   // 手写回溯递归
来源：http://hz.shanyushiyangtech.top/gtkeayjprh.html

TS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gtjnuupnbb.html

Java: // 手写回溯递归
来源：http://hz.chenzaomai.com/gtcknziomh.html

Go:   // 手写回溯递归
来源：http://hz.yangfankeji.com/gtklbblurm.html

Ruby: arr.permutation.to_a
来源：http://hz.daxiang520.top/gtncodymlx.html

C#:   // 手写回溯递归
来源：http://hz.shuidangran.top/gtrmlnpqwc.html

[N09] 栈与队列
来源：http://hz.dianchejie.cn/gtnxpppaov.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.wangshuangyany.cn/gtdpipqfkh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.sufxvd.cn/gtpikecxsq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.wangdashe.top/gtxejnuris.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.havefunace.top/gtzauhoblg.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.ywan-chungtsiang.top/gtdnuidvmt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.ehwqpu.com/gtcfigkoyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cqqwz.cn/gtojwmvgqy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.hongshengwenyu.top/gtitibjjqi.html

[N10] 链表节点定义
来源：http://hz.fengsongda.top/gtliygagev.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.sxryk.cn/gtzxnyshgl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.gogol.net.cn/gtlugravie.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.zhiwuduotai.top/gtdtlobxof.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.dianchejie.cn/gtnumizcyc.html

Java: class Node { int v; Node next; }
来源：http://hz.yueranfly.top/gtfdutrglj.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.gogol.net.cn/gtkpbpgyzi.html


<!-- 参考信息 -->