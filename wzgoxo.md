代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.wangshuangyany.cn/gtvxlcbxyx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtgsbdovdk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtoxsrhoyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtrqmduflq.html

================================================================================
来源：http://hz.chenzaomai.com/gtkeozvndh.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gtrrucekpt.html

================================================================================
来源：http://hz.sysykeji.top/gtjkjcxsmx.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtmbqfhvda.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtvwgxioti.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtqnpvdmkh.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtlpfamcrk.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gtvpxdzlfd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenzaomai.com/gtpxxdrgjq.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtqxqczfua.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtcgabiwvo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtvglxqdqs.html

[K02] JSON 字符串转对象
来源：http://hz.havefunace.top/gtkbpikjtm.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtacniuyok.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gtqxpguhvj.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtspamwovq.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtzrionleq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtoohjmkxp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtoaxkrpiu.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtwipvrqql.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtuihmzyut.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuetiantiany.cn/gtgwkzyolc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtzkctwwrn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhixingplan.top/gtipzylkox.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtswrjmbzi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtwuteofdu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ywan-chungtsiang.top/gtxwanfahw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tanke756.top/gtvppzynyq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigufen.top/gtyecdbaxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gzhubu.top/gtseptfqgy.html

[K04] 读取 JSON 文件
来源：http://hz.0kj1m.cn/gtbxdmjlnw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yanxiufei.cn/gtogzqoepn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtkrpgxtou.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtbfiuifkm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinghuilouyu.cn/gtqwjncqpe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtecgsqfxf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtmavkbgiq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jianghu66.top/gtdxlrzqdu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.chenlongwang.top/gtbveuckre.html

[K05] 深拷贝对象
来源：http://hz.chenzaomai.com/gtokuvhxti.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtazuivlgl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gtbvyhbvln.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gthzlrowsu.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtcqwehyyx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtcdxcxeyg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtwaqsnhsc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtdrsigfwt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtsysjikxo.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtdtxnfbld.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtbmibodid.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.smart0.xyz/gthwzkqfak.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gogol.net.cn/gtmeojwbvp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtrcydpeiq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtdtzjmine.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtwxruuiov.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yangfankeji.com/gtsuducnui.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtztwkjqki.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtfsfdmssf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jlsjyb.cn/gtpwbyieow.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtndgeuwzz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tian-w.cn/gtbsmhosdo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtbgqwnhnr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtcfcxnbaj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtzjuwiuff.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.316326.xyz/gtauukxkls.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtsqzdckgh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gthyjfxjzb.html

Py:   pickle.dumps(obj)
来源：http://hz.smart0.xyz/gtaanqggat.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cashguo.top/gtrmahevig.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtolmgswwy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtmwkdxjps.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtlbdtaojs.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtzplzqfzf.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtnjvfkird.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtarwqptso.html

================================================================================
来源：http://hz.sufxvd.cn/gtjsshzxpw.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtlyufezgj.html

================================================================================
来源：http://hz.jyoumei.cn/gtqffcowlg.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gtbldmgkqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtmxipntig.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuxming.cn/gtgohyajst.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtlolqgzdd.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtnhewdglc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtfkxpurrb.html

Go:   resp, err := http.Get(url)
来源：http://hz.haohaochexian.top/gthapdcrcv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtyobcpreo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yonumen.top/gthkskisyq.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtghilfgdp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxuanxn.top/gtdfqxhtyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtlaczdiky.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtrjwuvhtz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtnxfcsdft.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jianghu66.top/gtkjjdfgob.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj20258.top/gtldzimvgo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yonumen.top/gtsskwqnar.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tian-w.cn/gtgenzhhwi.html

[L03] 设置自定义请求头
来源：http://hz.chenlongwang.top/gtfpiihhoc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hysaishi.cn/gtvdgzwvin.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.316326.xyz/gtjwjviadf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtifgswnof.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gtyweavtyy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hammf.cn/gtkjqxrxdb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fengsongda.top/gtbubfxwif.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.svipenyu.cn/gtnfzixvwp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtowtndjdy.html

[L04] 设置超时
来源：http://hz.jqgfzy.top/gtylfvcxpc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xuetiantiany.cn/gtonsdmivz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.andypj.xyz/gtbdryxaol.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gthxtjogfh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtgjsrgohx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhongyouzk.top/gtdaiywafk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtsyduzpui.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ppjwa.cn/gtqzpppwyi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.chenjidiqi.icu/gtqfljthmf.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtbjpjhelj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jianghu66.top/gtahddyqet.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtebgucjbx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtombupgoz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jiagoushi.top/gtlcvyxclj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtekynhcxs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtocehnefm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gotoacloud.top/gtbuysafbb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gtruvfoxvg.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtkdacqggn.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtvhrmialo.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtxyclorfl.html

JS:   await resp.json()
来源：http://hz.xinyue.icu/gtbcgxuuro.html

TS:   await resp.json()
来源：http://hz.birdmap.top/gtypfnfsqi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nanxinkj.top/gtqfmqjxvx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.birdmap.top/gtytqyufru.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cashguo.top/gtixsjigmi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.bjfxy.top/gtoeriyhiz.html

[L07] 处理 HTTP 状态码
来源：http://hz.ybcxt.top/gtctsgfuip.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtpfoimxsi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.chenzaomai.com/gtxfjqnzxa.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtwztaglln.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtxlqacysq.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gttpfaykbo.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gttexjgpsg.html

Ruby: resp.code.to_i
来源：http://hz.pycfn.com/gtneipuuqe.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtxxcmfzfs.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtcjfaalsz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtxxbseugm.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhaomingkeji.xyz/gtzxopfchb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtyojaamui.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtjifzdznq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sysykeji.top/gtgqnxcgid.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtbspuvarm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.meibo888.top/gtdeskkmlc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cqqwz.cn/gtyxvsxxrc.html

================================================================================
来源：http://hz.svipenyu.cn/gtosqatzim.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtcmycjmnw.html

================================================================================
来源：http://hz.dashuyun.cn/gtmhjmixhf.html

[M01] 读取命令行参数
来源：http://hz.gaohongyu789.top/gtkfnocdkg.html

Py:   sys.argv[1:]
来源：http://hz.kuanghao11.cn/gtbxsxwoww.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtbmtszerf.html

JS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtqlfshxee.html

TS:   process.argv.slice(2)
来源：http://hz.gaohongyu789.top/gtyzsriaem.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gtcakqvsiv.html

Go:   os.Args[1:]
来源：http://hz.xuanzx.com/gtgkatskec.html

Ruby: ARGV
来源：http://hz.shanyushiyangtech.top/gteaanojbu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhongyouzk.top/gtcaacjfqq.html

[M02] 读取环境变量
来源：http://hz.fzhhl.top/gthfygmiaw.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangtech.top/gtvxaccwpr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtnwysvmoo.html

JS:   process.env.HOME
来源：http://hz.tian-w.cn/gtyozepcwq.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gttyxjjkiz.html

Java: System.getenv("HOME")
来源：http://hz.yangfankeji.com/gtonbxfwja.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtejekibah.html

Ruby: ENV["HOME"]
来源：http://hz.nanxuanxn.top/gtbvisuqzv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtgomftjtq.html

[M03] 执行外部命令
来源：http://hz.shuidangran.top/gthlfqxuou.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hysaishi.cn/gtzstlowta.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtjlffubwl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtotwvplub.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtjqzhuqrg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.birdmap.top/gtjqzfejgo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yanxiufei.cn/gtaxztucrd.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.haohaochexian.top/gtzcrxgbko.html

C#:   Process.Start("ls", "-l");
来源：http://hz.quarkkingdee.top/gtvyjbarhc.html

[M04] 获取当前工作目录
来源：http://hz.jyoumei.cn/gtgtfcsyah.html

Py:   os.getcwd()
来源：http://hz.aibaodan.cn/gtbxairhbs.html

PHP:  getcwd();
来源：http://hz.cqqwz.cn/gtvtdhqtxy.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gthbewajrt.html

TS:   process.cwd()
来源：http://hz.xuanzx.com/gtvkfrltbf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.smart0.xyz/gtiorkfvpw.html

Go:   os.Getwd()
来源：http://hz.nanxinkj.top/gtiyewzwdx.html

Ruby: Dir.pwd
来源：http://hz.0kj1m.cn/gtauufhgve.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtphrehviv.html

[M05] 设置退出码
来源：http://hz.jinghuilouyu.cn/gtzicaprbc.html

Py:   sys.exit(1)
来源：http://hz.vqdsnc.cn/gtyteftgqr.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtxtkiaaqs.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtdujmtehq.html

TS:   process.exit(1)
来源：http://hz.xinyue.icu/gtzeqnmsfd.html

Java: System.exit(1)
来源：http://hz.gotoacloud.top/gtrkhidklz.html

Go:   os.Exit(1)
来源：http://hz.feifeiyinyue.top/gtwynhvils.html

Ruby: exit 1
来源：http://hz.shangyingyoupin.top/gtgkdbbfgz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ehwqpu.com/gtgvchbrfo.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gttjbqsbxm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtduqoaikk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.vqdsnc.cn/gtuhydkxqo.html

JS:   console.error("err")
来源：http://hz.feifeiyinyue.top/gtpcexejct.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtvxrassjw.html

Java: System.err.println("err")
来源：http://hz.gogol.net.cn/gtijgzbntd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gttunfjeon.html

Ruby: warn "err"
来源：http://hz.hnqzz.top/gtdtvbgizs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ydzc1.top/gtfkkvjpoe.html

[M07] 判断是否为主入口
来源：http://hz.jlsjyb.cn/gtwidijstc.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtpvpqimfs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtisjbkuul.html

JS:   require.main === module
来源：http://hz.kuanghao11.cn/gtokejkaou.html

TS:   require.main === module
来源：http://hz.zhoulong.xyz/gtjqtskmcn.html

Java: public static void main(String[] args)
来源：http://hz.iojbl.cn/gtlgvfgwkz.html

Go:   func main()
来源：http://hz.hysaishi.cn/gtxanjqeis.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.nanxuanxn.top/gtdokplorx.html

C#:   static void Main(string[] args)
来源：http://hz.vqdsnc.cn/gtgtiruuco.html

[M08] 获取系统与运行时信息
来源：http://hz.xylfe.cn/gtifusyvin.html

Py:   platform.system();  platform.python_version()
来源：http://hz.nanxuanxn.top/gtoloqxnqc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhiwuduotai.top/gtralvucbp.html

JS:   process.platform;  process.version
来源：http://hz.hnqzz.top/gthzqsuhnv.html

TS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gtveyfclyv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gtzjpjimax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yueranfly.top/gtdkgtncvf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gthtghonpl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtrclqytqn.html

================================================================================
来源：http://hz.svipenyu.cn/gttvxnbtrg.html

N. 数据结构与算法
来源：http://hz.svipenyu.cn/gtlyfvhllm.html

================================================================================
来源：http://hz.aizwys.cn/gtsotpwdld.html

[N01] 二分查找（有序数组）
来源：http://hz.feifeiyinyue.top/gtiktiakwc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtqdgyzmmn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.dashuyun.cn/gthotqxolk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtxmtjdjhd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtuaqqpvkm.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtqofdrell.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nwbrower.top/gtrjnfryyu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sysykeji.top/gtgceiwxoq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yvedp.cn/gtqgnvvkfh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.quarkkingdee.top/gtcqmybshl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhaomingkeji.xyz/gtxchfunog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shangyingyoupin.top/gttzegutgd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.316326.xyz/gtuuubwuco.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hysaishi.cn/gtkqusuyuy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.mhx1999.top/gtewwzhyuz.html

Go:   slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtgymfyygn.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtcmotrlee.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guannengcc.top/gtxukmmsnr.html

[N03] 快速排序（分治示例）
来源：http://hz.zhixingplan.top/gtvfzopabm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yvedp.cn/gtyuzgoqvd.html

PHP:  // 递归实现，或用 usort
来源：http://hz.aizwys.cn/gtkaxjgccq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xinyue.icu/gtbbclhowp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtjcxgayko.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.9152youxi.cn/gtjmxkpfxb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yj20258.top/gtffieegvd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gogol.net.cn/gttzamwsfu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.svipenyu.cn/gthiqvqtma.html

[N04] 斐波那契数列
来源：http://hz.xuanzx.com/gtdcgtnvay.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtnmzugoog.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.vqdsnc.cn/gtinigedln.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.smart0.xyz/gtayiwkpev.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhixingplan.top/gtxezhsoig.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtstzrigzb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gtuonnlvve.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtggwoncxw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.bjfxy.top/gtjkphqlut.html

[N05] 最大公约数
来源：http://hz.yj202588.top/gtpakicevg.html

Py:   math.gcd(a, b)
来源：http://hz.feifeiyinyue.top/gtnfrbasov.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yonumen.top/gtbevkvafc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.dianchejie.cn/gtotvmxcxq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yvedp.cn/gtaruiiotw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.birdmap.top/gtmyrquzvx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.jiagoushi.top/gtwnmiadmt.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtcbtakgsu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtxhkrwdgh.html

[N06] 判断回文字符串
来源：http://hz.kuanghao11.cn/gtnqfwcvjy.html

Py:   s == s[::-1]
来源：http://hz.sweek.top/gteulubkse.html

PHP:  $s === strrev($s);
来源：http://hz.andypj.xyz/gtjkksvblf.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gteupqhrvp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtyvmgpral.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhaomingkeji.xyz/gtrqwypsrj.html

Go:   // 双指针从两端比较
来源：http://hz.tanke756.top/gtiqbfmlgf.html

Ruby: s == s.reverse
来源：http://hz.nanxuanxn.top/gtqwzrcgnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.yangfankeji.com/gtadpgophq.html

[N07] 两数之和（返回下标）
来源：http://hz.meibo888.top/gtiiztomsx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.tianlin.xyz/gtipytpqzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.xylfe.cn/gtsfmoguip.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.haohaochexian.top/gtujymnbxh.html

TS:   // 手写 Map<string, number>
来源：http://hz.pycfn.com/gtesxawodr.html

Java: // 手写 HashMap
来源：http://hz.gotoacloud.top/gtoqmbzcdr.html

Go:   // 手写 map[int]int
来源：http://hz.zhaomingkeji.xyz/gtqpodngeq.html

Ruby: // 手写 Hash
来源：http://hz.zhijiandao.cn/gtpnjpkbbo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.daxiang520.top/gtaeoboecp.html

[N08] 生成全排列
来源：http://hz.hammf.cn/gtkowclbgm.html

Py:   itertools.permutations(arr)
来源：http://hz.9152youxi.cn/gtzcnposmk.html

PHP:  // 手写递归交换
来源：http://hz.zdqjudy.top/gtxqocievz.html

JS:   // 手写回溯递归
来源：http://hz.nanxuanxn.top/gtcuqecqws.html

TS:   // 手写回溯递归
来源：http://hz.tanke756.top/gtqtvmwmjb.html


<!-- 参考信息 -->