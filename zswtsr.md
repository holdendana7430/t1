代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtwextucjm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gtruipmwom.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtdibojuyz.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtwczuizvb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtiwzetaej.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtqwphbfkc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtipbqxpgo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtkaatrcxa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtiuocchmh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtgxgkknvj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtuctlgjvc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gtnebqypjb.html

================================================================================
来源：http://hz.yuxming.cn/gtcaorcuko.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtcjxtgkcq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtetcjmcep.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtwfzmgrnh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtrjfbhnxt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtqpccotpx.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtbqmqgpad.html

TS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtwfqnrkcm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtnyzbldym.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtozwlystw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zycfv.cn/gtviwmyajc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtyqubemyd.html

[K02] JSON 字符串转对象
来源：http://hz.cheryme.top/gtihossndi.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gtljozotrz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtvseavdkm.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtvarzitxs.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtldlkfcog.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtishfzlri.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtksqpnzts.html

Ruby: JSON.parse(s)
来源：http://hz.yongpay.top/gtioldfesc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtwvuskdtm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtjqjjxwvq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtvlautttw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtqdjhledr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtyzhbqnlj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtejnfucyk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guannengcc.top/gtuxmzbvjz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtbgzzsyvx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yueranfly.top/gtqknxbeul.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtrywtduqv.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gttyltxxna.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtenagzifs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhijiandao.cn/gtfpizzksm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtnysfdbrk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtvcbjaixh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtzeknxbco.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gteuivcqsx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtkdiafcyi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtpltbaecv.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtedvrplpb.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtngxqjuou.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtmzontwrd.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtlvwrwjzr.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtosaceluk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtqlyaqofe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtlsgtpnff.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtlboxssfu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtjoqhhjul.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtpouaumru.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtndyuvelf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gtezsvaogx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtaxevcrlv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtpazmvniv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtqxbldwsm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtpyvsxtxr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtvbmtpkyn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.iojbl.cn/gtvyyohtel.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtturtgbkl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gthgcqyicr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gthuijlrbo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtwwtljvok.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtykqarrit.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258.top/gtytpylxzz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydzc1.top/gtiefkufbe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gttocyvyxk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtprdrkzgm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtxinlitgz.html

Py:   pickle.dumps(obj)
来源：http://hz.hnqzz.top/gtwrohlkqi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.iojbl.cn/gtzcwjsefg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtjzkahnod.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtzgdsehwg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtqkuevzsa.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtcnlrztuz.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtoxnhpryi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtdjedcubd.html

================================================================================
来源：http://hz.pycfn.com/gtbwmvoern.html

L. 网络请求
来源：http://hz.jinghuilouyu.cn/gttxczllps.html

================================================================================
来源：http://hz.bjfxy.top/gtnusbobnw.html

[L01] 发送 GET 请求
来源：http://hz.yanxiufei.cn/gtbxsmfubm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtkmofqdnp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gtrtbgooch.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtfzebqdit.html

TS:   await fetch(url)
来源：http://hz.fengsongda.top/gtekupvakn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.c1oappe.top/gttezdcdxu.html

Go:   resp, err := http.Get(url)
来源：http://hz.quarkkingdee.top/gtmjxuaqdi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtiwitqwkv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gtdbedjwkc.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtrzcijbsy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtdfvvhlux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenlongwang.top/gtmoaujyew.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gtcdvlmdcg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtnhxxuowm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtqqjpbeiu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtbnqwhdic.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cdnleiting.top/gtkdgffyel.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtelkqnbyh.html

[L03] 设置自定义请求头
来源：http://hz.yj20258888.top/gtjgsenoau.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.dashuyun.cn/gtwngqcxwl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtfzyongsv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtsnnaeoum.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtvtyantei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuxming.cn/gtgaaqktla.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtwgspbdle.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nwbrower.top/gtjurfxaml.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gthrmhxajf.html

[L04] 设置超时
来源：http://hz.meibo888.top/gtpuwatuts.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gteimtehan.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.gzhubu.top/gteujenhrg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtclbccgcz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtojvlvsyw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtjdrblyku.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuxming.cn/gtdowkefie.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgufenzy.top/gtapkwovjg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gttgytyjuw.html

[L05] 上传文件（multipart）
来源：http://hz.daria6918.cn/gtemnyhsak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhengqikj.top/gtkzicrxod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.guowangkeji.top/gthrvxzkkv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.meibo888.top/gtuxbiehgf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtzftcuemr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ppjwa.cn/gtoxutzdnt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenzaomai.com/gtnzgydehq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.smart0.xyz/gtanzvawzl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gtvumlpzof.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtmbvpqltl.html

Py:   resp.json()
来源：http://hz.mhx1999.top/gthnvsexps.html

PHP:  json_decode($body, true);
来源：http://hz.daria6918.cn/gthsqxijhh.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtykdppeer.html

TS:   await resp.json()
来源：http://hz.tian-w.cn/gtybvgqvjw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.wangshuangyany.cn/gtvrmxahfr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhaomingkeji.xyz/gtmxccwttt.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hysaishi.cn/gtfbkycqkp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xingfuxueyuan.xyz/gtrvfzsugt.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtpatykwxl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtxkeywsgz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jlsjyb.cn/gtizfaentw.html

JS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtyxvicafn.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtwuemidiz.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtniaxeumm.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtcaluiyna.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtucxgjsow.html

C#:   (int)resp.StatusCode
来源：http://hz.jqgufenzy.top/gtzssdjnga.html

[L08] 并发请求多个地址
来源：http://hz.ivvv.top/gtfpohbfcj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtezqimnfr.html

PHP:  curl_multi_init() 系列
来源：http://hz.snrcjt.cn/gthlpskxnd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.tianlin.xyz/gtdzcomfuo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtegldexnu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daxiang520.top/gtmygfcfwl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gotoacloud.top/gtgsxwgxwj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gthqbqvjtd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.pycfn.com/gtrfdhhrty.html

================================================================================
来源：http://hz.hywenlv.cn/gtjublfpum.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtczlmhekb.html

================================================================================
来源：http://hz.aibaodan.cn/gtimlqsemh.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtsgjxzvfg.html

Py:   sys.argv[1:]
来源：http://hz.nwbrower.top/gtxkxkitaw.html

PHP:  $argv;  $argc;
来源：http://hz.cucudq.cn/gtijybwipz.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtbxidilud.html

TS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gthjfumgdl.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtvvdkdnmd.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtatdgkatu.html

Ruby: ARGV
来源：http://hz.nanxuanxn.top/gtfjikgeqg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtlilrqqap.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtxkfqiirn.html

Py:   os.environ.get("HOME")
来源：http://hz.jinyuanbaomall.cn/gthfbyhrvg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtwyijlqdx.html

JS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtnqxsknai.html

TS:   process.env.HOME
来源：http://hz.cdnleiting.top/gttvbloyde.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtkjxxtnxf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtqfdlcigz.html

Ruby: ENV["HOME"]
来源：http://hz.yuanzhike.top/gtygkzjdbm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hongshengwenyu.top/gtfysyzlyx.html

[M03] 执行外部命令
来源：http://hz.jinyuanbaomall.cn/gturjsmmag.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinyuanbaomall.cn/gtdvsnpnbs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gtbvqvojjj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtnbbzhens.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ybcxt.top/gtjqtvulsm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.svipenyu.cn/gtqzdxrvcq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtmkttxrgy.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yonumen.top/gtuxoxkltb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtluyidfxq.html

[M04] 获取当前工作目录
来源：http://hz.nanxinkj.top/gttlhpcnja.html

Py:   os.getcwd()
来源：http://hz.nwbrower.top/gtxjhcthhq.html

PHP:  getcwd();
来源：http://hz.gogol.net.cn/gtvfvyvtuj.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtqbwgktwd.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtlqbneffg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yangfankeji.com/gtvdqptxcd.html

Go:   os.Getwd()
来源：http://hz.andypj.xyz/gtzqlalmjt.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtwfqwctlg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jqgfzy.top/gtiktaeqpy.html

[M05] 设置退出码
来源：http://hz.bjfxy.top/gtgwnqnqlo.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtrbpshdab.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtxqndeylk.html

JS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtbqtdmwih.html

TS:   process.exit(1)
来源：http://hz.andypj.xyz/gtocfwuqbq.html

Java: System.exit(1)
来源：http://hz.havefunace.top/gtyczaggxh.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtnpljnjuu.html

Ruby: exit 1
来源：http://hz.shanyushiyangtech.top/gtktzstjqk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shzxlz.cn/gtvvthyots.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtmnjlnixa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtkutxcazv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fzhhl.top/gtnnmtipzb.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtuvjxbvcm.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gthyelqqnv.html

Java: System.err.println("err")
来源：http://hz.bjfxy.top/gtyiapmaek.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gaohongyu789.top/gtiwcfwiec.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gtgwvyllwd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.havefunace.top/gtwibrwldw.html

[M07] 判断是否为主入口
来源：http://hz.ydzc1.top/gtpycycpqt.html

Py:   if __name__ == "__main__":
来源：http://hz.yj202588.top/gtughmxfms.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.fzhhl.top/gtxnaxwlbj.html

JS:   require.main === module
来源：http://hz.shanyushiyangkeji.top/gteyrdrdwl.html

TS:   require.main === module
来源：http://hz.sufxvd.cn/gtfvggzbtd.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtlmwyrffl.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtyifyvqhg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.smart0.xyz/gtibamvqys.html

C#:   static void Main(string[] args)
来源：http://hz.fengsongda.top/gtrzbgveia.html

[M08] 获取系统与运行时信息
来源：http://hz.yangfankeji.com/gtylrbjncp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yueranfly.top/gtzwooqadd.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.feifeiyinyue.top/gtljntvpno.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtftktzdwo.html

TS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtkmvjvrxz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtkpwpbpiq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.pengpengdd.cyou/gtmjbihqux.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xinyue.icu/gthyywwwco.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.0kj1m.cn/gtpkszwmyl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvxfdvuie.html

N. 数据结构与算法
来源：http://hz.shuidangran.top/gttlrxzbll.html

================================================================================
来源：http://hz.yj202588.top/gtcuapvmau.html

[N01] 二分查找（有序数组）
来源：http://hz.yueranfly.top/gtfwhrwbem.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.nwbrower.top/gtkladtdnq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yanxiufei.cn/gtkewgiowy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.andypj.xyz/gtfxzxatjc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtmpxhcacg.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtageejlgy.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.birdmap.top/gtdywrqscd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xuanzx.com/gtuvzmyyij.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xylfe.cn/gtfviaafxq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.andypj.xyz/gtpxfohjea.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gttknnkvsh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tanke756.top/gteyjdhgmd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtfounbqne.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gthehvmgmz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yuanzhike.top/gthsccxmfi.html

Go:   slices.Sort(arr)
来源：http://hz.0kj1m.cn/gtlhqksqbe.html

Ruby: arr.sort
来源：http://hz.chenjidiqi.icu/gtsmmxixnp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xylfe.cn/gtchubqpyk.html

[N03] 快速排序（分治示例）
来源：http://hz.xinyue.icu/gttzrkmezw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jinqigfzy.top/gtzpgdpsut.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jiagoushi.top/gtevdmlkqm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yongpay.top/gtxekdsfrx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.feifeiyinyue.top/gtmamonivh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sufxvd.cn/gthkrqctfv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ppjwa.cn/gtzhubmmyk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.c1oappe.top/gtehyseevj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.316326.xyz/gtgapncbit.html

[N04] 斐波那契数列
来源：http://hz.tian-w.cn/gtntbkeupa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.jlsjyb.cn/gtqjwalsfm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtnsvfbfdy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shanyushiyangkeji.top/gtvdeeftsi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangshuangyany.cn/gtnyjkohpd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.redwolf501.top/gtesnhdyje.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtvldyljfv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhaomingkeji.xyz/gtwobxewnh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtzgojsxex.html

[N05] 最大公约数
来源：http://hz.zycfv.cn/gtqxiwqgyp.html

Py:   math.gcd(a, b)
来源：http://hz.birdmap.top/gtihcsdlcg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xingfuxueyuan.xyz/gtezutqecy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yangfankeji.com/gtgnqnvuwq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtxcnrylpe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhaomingkeji.xyz/gtwfpgsttf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhengqikj.top/gtrhalqxhr.html

Ruby: a.gcd(b)
来源：http://hz.guannengcc.top/gtydafmiuj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.redwolf501.top/gtqyqyctne.html

[N06] 判断回文字符串
来源：http://hz.pengpengdd.cyou/gtojeuqwqo.html

Py:   s == s[::-1]
来源：http://hz.52xcode.cn/gtwtladgnr.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtzfmfqfkc.html

JS:   s === [...s].reverse().join("")
来源：http://hz.pycfn.com/gtsjgspkvg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtsjtozfzb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtywmjlklj.html

Go:   // 双指针从两端比较
来源：http://hz.shanyushiyangtech.top/gtdfixicvf.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtkqqzodak.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtwatidjti.html

[N07] 两数之和（返回下标）
来源：http://hz.ywan-chungtsiang.top/gtpmuqzxos.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jiagoushi.top/gtkoyndvze.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ywan-chungtsiang.top/gtbpsqkxkh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.mhx1999.top/gtqizfuywm.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtvhjlvive.html

Java: // 手写 HashMap
来源：http://hz.jianghu66.top/gtnrkrxixn.html


<!-- 参考信息 -->