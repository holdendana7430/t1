代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtgplwnucb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtofopkpjn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jiagoushi.top/gtfatmlsmn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtnwrrcfze.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gthdazvrda.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangtech.top/gtzhzyyiqp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtcfeglinb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.feifeiyinyue.top/gtwkmkntgh.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtuvmclfvn.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtwintcbfo.html

================================================================================
来源：http://hz.snrcjt.cn/gtprsrbymb.html

[K01] 对象转 JSON 字符串
来源：http://hz.gogol.net.cn/gteswmcsuh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtxzkzccmi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtbyqhcvom.html

JS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtuqrswvul.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtylizelyd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gthbupflhu.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangtech.top/gtystheexp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtmrkxpqvo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtllaevmpe.html

[K02] JSON 字符串转对象
来源：http://hz.jiagoushi.top/gtviguldou.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtdrndcwbw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtxwgvfocd.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtutvdzlvc.html

TS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gttsjpyccw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gtmjdmkpsx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gthbqzsotm.html

Ruby: JSON.parse(s)
来源：http://hz.haohaochexian.top/gtuznbcfyx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gtoizznnpp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.9152youxi.cn/gteushxcid.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtmdemecfa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtwzeatolg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtgpnqcayz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtcxoravmi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gteyvvlseh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtgymtxral.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtiomcndkp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.redwolf501.top/gtlnqiohff.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtcuuevumw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhaomingkeji.xyz/gtfakxexce.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtejmrpwqv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtzajnmjyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtfdtduqmt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtpejxecjp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtdrvvinsp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuanzx.com/gtumiiqsts.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gtlgwizygb.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtpoqlaays.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtzqkxuhts.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtdlqvcbre.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtgshxswla.html

TS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtuqznkvtj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtwxghicpn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yanxiufei.cn/gtdzxxddiz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tianlin.xyz/gtvrmdgqqa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ppjwa.cn/gtqvzawmhx.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtqdezthmr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtbjeopthw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtvhttqcpn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtgoiyxpeo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtvukjuyqn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258888.top/gtzjdlbewx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtodumlouu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtgfedrtjn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtxlepqmuj.html

[K07] 进制转换
来源：http://hz.zhiwuduotai.top/gtbeaysjra.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtaxbnsufu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yvedp.cn/gtxkuwfmmk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtslorlprb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtvixvzayb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtastqmbbl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtreqpkdld.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtbrzflkgs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zdqjudy.top/gtoopjajxq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258.top/gtmirgcmbv.html

Py:   pickle.dumps(obj)
来源：http://hz.tanke756.top/gtqtqngoyp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtyalqewdo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtlciovspz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtjlvdqgip.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtqlkperya.html

Go:   encoding/gob
来源：http://hz.zhongyouzk.top/gtceictfav.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtgbsxmiej.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtqwyiyazs.html

================================================================================
来源：http://hz.ydjk.org.cn/gtzbemlzsr.html

L. 网络请求
来源：http://hz.yongpay.top/gtfuotboad.html

================================================================================
来源：http://hz.sysykeji.top/gtbotvmjvq.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtustabrgg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtextfaqwl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtlglfyfug.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gtulfxtaro.html

TS:   await fetch(url)
来源：http://hz.zhiwuduotai.top/gtabfmeqxz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gterqkjyzt.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtqnmoeshi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.9152youxi.cn/gtdbfpsafj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtwsrlxafj.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtxzilgdmp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhongyouzk.top/gtxdnzjpdu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tianlin.xyz/gtydogxkzt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtdnzzjjje.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtgacdvzuo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gzhubu.top/gtrzntzsba.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtzfgmrhav.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gteopseudt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtxijyetsk.html

[L03] 设置自定义请求头
来源：http://hz.gzhubu.top/gtdxrsbxqi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yueranfly.top/gtiafsszls.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gtftalkmqj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtrykkkgpy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sweek.top/gtsxvjwxla.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pengpengdd.cyou/gtfphjkzdj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gttuweymiz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtjjyakdsc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtdsyqzwns.html

[L04] 设置超时
来源：http://hz.daria6918.cn/gtmqbwoufe.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydjk.org.cn/gtvjumkxzd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtohwpzbvy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shanyushiyangkeji.top/gtjranmmiu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtpmsxpphm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gthecpunci.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.nwbrower.top/gtkdncsins.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shzxlz.cn/gtimvoeaec.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.kuanghao11.cn/gttffspvcf.html

[L05] 上传文件（multipart）
来源：http://hz.jqgufenzy.top/gtamuhtqbw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zycfv.cn/gtmewxwbny.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtljzxmhgv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtxtvfvlzh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuxming.cn/gtquwbghdv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtthresihm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.mhx1999.top/gtvehkpwwr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gzhubu.top/gtwjkhntij.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtyqaumogb.html

[L06] 解析响应为 JSON
来源：http://hz.pengpengdd.cyou/gttphbaiyd.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtwzxijwbl.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtgtrmbtal.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtefcouyqx.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtxpyljjff.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtanpzoucp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sysykeji.top/gtitkjspnc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtoynmchng.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gtdzjogkch.html

[L07] 处理 HTTP 状态码
来源：http://hz.fzhhl.top/gtjehycltj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtihzgkxmq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hammf.cn/gtczglback.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtsbbdrqrw.html

TS:   resp.ok;  resp.status
来源：http://hz.ehwqpu.com/gtuzadcvlk.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtkyrxkjod.html

Go:   resp.StatusCode
来源：http://hz.0kj1m.cn/gthjjbqzdt.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtdsklnzyj.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gtfjggehie.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtzqiiteku.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtfzwzqzpg.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtnbrviptu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtmeexfvcl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtiynwxbuq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gthluiyvhy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shuidangran.top/gtpusupsch.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sxryk.cn/gtopelsayy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.iojbl.cn/gtldqhffap.html

================================================================================
来源：http://hz.guowangkeji.top/gtnajmkbrv.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtuixuiutf.html

================================================================================
来源：http://hz.ybcxt.top/gtsfltcznp.html

[M01] 读取命令行参数
来源：http://hz.meibo888.top/gthkxghfgr.html

Py:   sys.argv[1:]
来源：http://hz.redwolf501.top/gtuftcavsb.html

PHP:  $argv;  $argc;
来源：http://hz.yangfankeji.com/gtfvosbnxm.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtnhaoopuf.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gttbibhekn.html

Java: args 数组（main 方法参数）
来源：http://hz.chenzaomai.com/gtmgimzbpq.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gtumxsjdei.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtbfhoyqkb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinyuanbaomall.cn/gtiomlaofu.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gtvcesqxue.html

Py:   os.environ.get("HOME")
来源：http://hz.9152youxi.cn/gtkaiarrop.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258.top/gtyytxhzfc.html

JS:   process.env.HOME
来源：http://hz.yuxming.cn/gtxhgpgtsk.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtslynmdwf.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtcjtshuhm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangdashe.top/gtbprcaxvp.html

Ruby: ENV["HOME"]
来源：http://hz.xinyue.icu/gtlwrjlglb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.fzhhl.top/gtqioqtijc.html

[M03] 执行外部命令
来源：http://hz.xinyue.icu/gtwinlaxjf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cqqwz.cn/gtigzduwwl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pengpengdd.cyou/gtjvbjfgyu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtfveemfmw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtdtabgroc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yanxiufei.cn/gtxeqwacah.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cheryme.top/gthqjxdeun.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.redwolf501.top/gtnwawrgmz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.0kj1m.cn/gtjdosrutv.html

[M04] 获取当前工作目录
来源：http://hz.ybcxt.top/gtwdsnlprd.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtqvhegqyr.html

PHP:  getcwd();
来源：http://hz.c1oappe.top/gtwwvszzli.html

JS:   process.cwd()
来源：http://hz.cdnleiting.top/gtlmiohhlf.html

TS:   process.cwd()
来源：http://hz.guowangkeji.top/gtubikdiwi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ydjk.org.cn/gtcqbujyiy.html

Go:   os.Getwd()
来源：http://hz.cucudq.cn/gtkaxvfgud.html

Ruby: Dir.pwd
来源：http://hz.ppjwa.cn/gtnpnwhijx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ppjwa.cn/gttpzsxneh.html

[M05] 设置退出码
来源：http://hz.yj20258.top/gtrjzhcjgg.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtjnjpjcpx.html

PHP:  exit(1);
来源：http://hz.hywenlv.cn/gtlpxxjiec.html

JS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtjvmlosql.html

TS:   process.exit(1)
来源：http://hz.kuanghao11.cn/gtognmbaas.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtwfnrmpml.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtnxxrjhjk.html

Ruby: exit 1
来源：http://hz.tianlin.xyz/gtkttvsodf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydjk.org.cn/gtzbyzmbed.html

[M06] 向标准错误输出
来源：http://hz.andypj.xyz/gtrbjzlqwm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtohuckuuv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtablccmdo.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtwjiykury.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtvmunjqnt.html

Java: System.err.println("err")
来源：http://hz.hongshengwenyu.top/gtwbfryesc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.vqdsnc.cn/gtmkliqqbk.html

Ruby: warn "err"
来源：http://hz.sysykeji.top/gtcljzlkpm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtboxcsfdx.html

[M07] 判断是否为主入口
来源：http://hz.zhiwuduotai.top/gtnbbumqef.html

Py:   if __name__ == "__main__":
来源：http://hz.shanyushiyangkeji.top/gtbznyhviy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jiagoushi.top/gtbbxvsjbs.html

JS:   require.main === module
来源：http://hz.guannengcc.top/gtrkdecwfz.html

TS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtqcbhbxdj.html

Java: public static void main(String[] args)
来源：http://hz.gzhubu.top/gtruixdvfn.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtgzoucmku.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtqomezsfl.html

C#:   static void Main(string[] args)
来源：http://hz.zdqjudy.top/gtaigkinmx.html

[M08] 获取系统与运行时信息
来源：http://hz.jinghuilouyu.cn/gtuaesedcq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.pengpengdd.cyou/gtiwpmxkbu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hfpthk.cn/gtvmanstmu.html

JS:   process.platform;  process.version
来源：http://hz.xingfuxueyuan.xyz/gtecazruiu.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtroeabspo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.wangdashe.top/gtqtyockni.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhongyouzk.top/gtvlbnxdyy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.fengsongda.top/gtjafzbyrk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.aizwys.cn/gtcbagtshw.html

================================================================================
来源：http://hz.hnqzz.top/gtlgvcagry.html

N. 数据结构与算法
来源：http://hz.jinghuilouyu.cn/gttbmfptvo.html

================================================================================
来源：http://hz.birdmap.top/gtnmsqmaow.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gthvbtbktp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.mhx1999.top/gtngauhmkk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xuanzx.com/gtneqzmlba.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhixingplan.top/gtwglrkscb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.vqdsnc.cn/gtybrljnjk.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sweek.top/gtechcwozr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gtixpjrawa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhiwuduotai.top/gtwontrgkq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gthsianoik.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.vqdsnc.cn/gtsldoepxd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtxbspqacj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tianlin.xyz/gtzxqgeayw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zdqjudy.top/gtcchdbqhh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gtndzhobli.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.9152youxi.cn/gtnzxaspuz.html

Go:   slices.Sort(arr)
来源：http://hz.meibo888.top/gtbuoescif.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtupamknuz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.hfpthk.cn/gtqbsgewhk.html

[N03] 快速排序（分治示例）
来源：http://hz.nanxuanxn.top/gtjcmwvuqx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtoadaxlri.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yonumen.top/gtxvxfvljh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtapfthddv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guowangkeji.top/gtgpjudinf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shanyushiyangtech.top/gtwfmmylvh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.tanke756.top/gtfevydznf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yonumen.top/gtstslpvci.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ivvv.top/gtktslummd.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gteixysmcz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yvedp.cn/gtfluyzwqc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtnfuknnxg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gthorshdcz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gttvfxtyzd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shangyingyoupin.top/gtwayuoeue.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.tanke756.top/gtrbbvueev.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hysaishi.cn/gtpsgybewa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtvgrfrbop.html

[N05] 最大公约数
来源：http://hz.cashguo.top/gtliequtex.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtdqdilkre.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.gogol.net.cn/gtqaanbpxs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnxiangtu.top/gthgixvufg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yongpay.top/gtrwuqwjon.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.xuetiantiany.cn/gtbcappjev.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.shangyingyoupin.top/gtuggxwcou.html

Ruby: a.gcd(b)
来源：http://hz.nanxuanxn.top/gtsqgljyfk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tanke756.top/gtlxzcyybd.html

[N06] 判断回文字符串
来源：http://hz.hfpthk.cn/gtutxztrue.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gtbepjznzw.html

PHP:  $s === strrev($s);
来源：http://hz.gotoacloud.top/gtnplrtijg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pengpengdd.cyou/gthnwikbln.html

TS:   s === [...s].reverse().join("")
来源：http://hz.tanke756.top/gtfsalnvkd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yangfankeji.com/gtzpuyvvsj.html

Go:   // 双指针从两端比较
来源：http://hz.jinghuilouyu.cn/gtnphyjsml.html

Ruby: s == s.reverse
来源：http://hz.redwolf501.top/gtnepwfkbt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtybscdyji.html

[N07] 两数之和（返回下标）
来源：http://hz.cdnleiting.top/gtkcvbvskn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gtlwubhjsa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ydzc1.top/gtuaqzfxdh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gttznzansh.html

TS:   // 手写 Map<string, number>
来源：http://hz.nwbrower.top/gtaxpjapuf.html

Java: // 手写 HashMap
来源：http://hz.smart0.xyz/gtuwwqzjop.html

Go:   // 手写 map[int]int
来源：http://hz.wangdashe.top/gtlcwxkvek.html

Ruby: // 手写 Hash
来源：http://hz.zhoulong.xyz/gtqtkdbmfa.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.sxryk.cn/gtlqjergdj.html

[N08] 生成全排列
来源：http://hz.gogol.net.cn/gtqqvdjsbo.html


<!-- 参考信息 -->