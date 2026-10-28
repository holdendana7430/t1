代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtolccncoa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gttpympujf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtorewdugj.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtiphfaajv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtmwubhpxj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gttlllilit.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtpwyvvhhd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gteewfhdfn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtyhewwhbk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtamyjuqed.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtnobxbrap.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtimuxjywp.html

================================================================================
来源：http://hz.yuxming.cn/gtatfafybs.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtuogqzsrv.html

================================================================================
来源：http://hz.hfpthk.cn/gtnafllerx.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtlflwcfhw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtzzjmwzfu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtcwdxjqia.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtperpmmey.html

TS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtadnkneqn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtzewhyzxd.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtqhnqtsgd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtntpdbldu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtzhxjyjqo.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtyeswzwga.html

Py:   json.loads(s)
来源：http://hz.ydzc1.top/gtnwgquzeq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtgyifgsiu.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtjnguyuda.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtsaiuldsf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtxnfpssjt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtlkxxdsjr.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtwsdnujfa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yuanzhike.top/gtywehgzge.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtxqtyfqym.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtqcyikbbp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtlmlallyg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtyyqdqplb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtgsqblvaw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtwjeghhcx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinqigufen.top/gtjgzloqmk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gttlhtffdp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtnsjyztwg.html

[K04] 读取 JSON 文件
来源：http://hz.aibaodan.cn/gtruqeuhkw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtcvtikfkn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daxiang520.top/gtveiwzuef.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtwrerqwly.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtmapooizy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtsspljleb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtqicpaasi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtshnpwrdx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.iojbl.cn/gtqbcycvgz.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtzdjtcswa.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gtuwtecxzp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gthtyklvjc.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtwjlfzykj.html

TS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtynshijgz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtqtcyzbyl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtniblnmyc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.316326.xyz/gtyhsbcaib.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtxqivfpga.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gttnfdasze.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jianghu66.top/gtskcezdjy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gtjioiojch.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtjlrnxvsa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtrrwwcesc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shuidangran.top/gtkfynwgja.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtjrpqrupf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtlzbrehul.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtcqnxzkpk.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gtheegzioy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtsdrswtcs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtmfoaezuc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtsqnobgnp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtwvdffrqp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtdmimdwtz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtzrfcnxon.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guowangkeji.top/gtigkwvvsm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.52xcode.cn/gtoibzrbdx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtghkijjkr.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgufenzy.top/gtxftubwjs.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.tian-w.cn/gtfgbzvwxg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtyblowdbb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtqppenxfs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtufzheyxv.html

Go:   encoding/gob
来源：http://hz.xingfuxueyuan.xyz/gtfbdfvpmr.html

Ruby: Marshal.dump(obj)
来源：http://hz.hammf.cn/gtxxilcroo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtqwezvarh.html

================================================================================
来源：http://hz.xinyue.icu/gtznkcxbyo.html

L. 网络请求
来源：http://hz.ybcxt.top/gtqdwejthx.html

================================================================================
来源：http://hz.tianlin.xyz/gtkztkyvpi.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtnwnitlom.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtmcfrugmv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinyuanbaomall.cn/gtqesfbvjq.html

JS:   await fetch(url)
来源：http://hz.cashguo.top/gtjnfovkdm.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtltvntggw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtygadogel.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtxdctgafd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtgdxwxfie.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.wangdashe.top/gtqxlwszaz.html

[L02] 发送 POST JSON
来源：http://hz.chenjidiqi.icu/gtfrslbqia.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigufen.top/gtvjvnkxpy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gotoacloud.top/gtsjvyzzbp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuanzhike.top/gtjceiknjz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtmkybcoou.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.wangshuangyany.cn/gteuozywmq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gtxbvfsftt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.c1oappe.top/gtgajzcmav.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtareivhdv.html

[L03] 设置自定义请求头
来源：http://hz.yueranfly.top/gtrwwchvee.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shzxlz.cn/gtsifumpbe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtmunjggyl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtoelmqbjy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtvghzgwpl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gturotuaai.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtjpawpyqw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gtvuyvhxrs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.feifeiyinyue.top/gtnjsyekby.html

[L04] 设置超时
来源：http://hz.dashuyun.cn/gteuqhhldg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtxbiboywt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtnlhblsuq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtpotysfxs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gttrqsecqm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtnfmikvbh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtixpuzxak.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangdashe.top/gteflizlai.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtwwfpylce.html

[L05] 上传文件（multipart）
来源：http://hz.hammf.cn/gtvkqsiclb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yvedp.cn/gtsoxsuboh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtzxtnmmdk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtwugtczbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtwlfqzufl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cqqwz.cn/gtfiwzsyop.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shuidangran.top/gtvalcclrn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtbpyubjgj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cdnleiting.top/gtoahlvthw.html

[L06] 解析响应为 JSON
来源：http://hz.xziqi.cn/gtoasmkvnm.html

Py:   resp.json()
来源：http://hz.andypj.xyz/gtflmbgwaq.html

PHP:  json_decode($body, true);
来源：http://hz.nanxuanxn.top/gtsgifjdoa.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtmvtdurad.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtjehsuacg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtqtczprgl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.kuanghao11.cn/gtltqqovrx.html

Ruby: JSON.parse(resp.body)
来源：http://hz.smart0.xyz/gtombrjpre.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhengqikj.top/gtthrgmbtj.html

[L07] 处理 HTTP 状态码
来源：http://hz.yvedp.cn/gttkzcvuhx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.daria6918.cn/gtbdmrlbvh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ydjk.org.cn/gtafpuoilr.html

JS:   resp.ok;  resp.status
来源：http://hz.cdnleiting.top/gtxgmnuytt.html

TS:   resp.ok;  resp.status
来源：http://hz.daxiang520.top/gtipqazhee.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtoptnwoas.html

Go:   resp.StatusCode
来源：http://hz.kuanghao11.cn/gtzadhlmnx.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtrcsaevyt.html

C#:   (int)resp.StatusCode
来源：http://hz.chenlongwang.top/gtnjgdaocr.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtilbhjwzu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtyksafamh.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtwiywqapx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtsiqcoawj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtxhyphvbh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gtzwifnbzg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtclytfigf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtvobhnfif.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gttlinozpm.html

================================================================================
来源：http://hz.andypj.xyz/gtvmmxpzjh.html

M. 命令行 / 进程 / 环境
来源：http://hz.sysykeji.top/gtxzpwjoos.html

================================================================================
来源：http://hz.yueranfly.top/gtkciwfpum.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtadffdgoe.html

Py:   sys.argv[1:]
来源：http://hz.jinyuanbaomall.cn/gtsqkqdwmc.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtjnbrwxva.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtpbrvbvcr.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtyslbrhao.html

Java: args 数组（main 方法参数）
来源：http://hz.jlsjyb.cn/gtzflsjbsi.html

Go:   os.Args[1:]
来源：http://hz.daria6918.cn/gtktqmpzzw.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtrfpdfbrd.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtdsyixjms.html

[M02] 读取环境变量
来源：http://hz.chenlongwang.top/gtypezxxje.html

Py:   os.environ.get("HOME")
来源：http://hz.tianlin.xyz/gtsqefhtbq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gttzgztrgh.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtlmhwhhqq.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtmvulztrf.html

Java: System.getenv("HOME")
来源：http://hz.wangdashe.top/gteteoqmqw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydzc1.top/gtqurbdbzb.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtxfarydkh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gttsngsbnr.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gthiurgkdl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yongpay.top/gtfuikdfuh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtoymxcdwc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.redwolf501.top/gtqorpatkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jlsjyb.cn/gtozsxhomx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhiwuduotai.top/gtenekhyre.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtaxvqqege.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtjxqjqyxl.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinqigfzy.top/gtmxzrrryo.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gthvsrcoyx.html

Py:   os.getcwd()
来源：http://hz.yj20258.top/gtohpjcesb.html

PHP:  getcwd();
来源：http://hz.wangshuangyany.cn/gtboupwibg.html

JS:   process.cwd()
来源：http://hz.cucudq.cn/gtdctsynij.html

TS:   process.cwd()
来源：http://hz.0kj1m.cn/gtrsmtvwdn.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtzemdbxvv.html

Go:   os.Getwd()
来源：http://hz.jqgufenzy.top/gtwrocrtmr.html

Ruby: Dir.pwd
来源：http://hz.sweek.top/gtvmhyertz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cqqwz.cn/gtogfubaao.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtwhjjuutg.html

Py:   sys.exit(1)
来源：http://hz.andypj.xyz/gtwlxxrgcx.html

PHP:  exit(1);
来源：http://hz.guowangkeji.top/gtdbupmczx.html

JS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtlppxlces.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtlcmmfeqz.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gtgebnmzkn.html

Go:   os.Exit(1)
来源：http://hz.yangfankeji.com/gtwlxombvn.html

Ruby: exit 1
来源：http://hz.fengsongda.top/gtpppkgveo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zdqjudy.top/gtsqqixzoi.html

[M06] 向标准错误输出
来源：http://hz.yj202588.top/gtueznrmwh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtpqtoxbcb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinqigufen.top/gtnrwxkwkc.html

JS:   console.error("err")
来源：http://hz.andypj.xyz/gtnbywlevw.html

TS:   console.error("err")
来源：http://hz.wangdashe.top/gtawcxsdgh.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtbapiecnh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jianghu66.top/gtresrvmam.html

Ruby: warn "err"
来源：http://hz.ydzc1.top/gtsggkmead.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtszhrbibv.html

[M07] 判断是否为主入口
来源：http://hz.daria6918.cn/gtzjjyforx.html

Py:   if __name__ == "__main__":
来源：http://hz.zhiwuduotai.top/gtckvcyzjy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cheryme.top/gtomimqgmy.html

JS:   require.main === module
来源：http://hz.jqgfzy.top/gtectlkygt.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtwebvexbi.html

Java: public static void main(String[] args)
来源：http://hz.jyoumei.cn/gtopcuvhll.html

Go:   func main()
来源：http://hz.hongshengwenyu.top/gtgyadiwma.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hywenlv.cn/gtvskqypxt.html

C#:   static void Main(string[] args)
来源：http://hz.jinyuanbaomall.cn/gtmsntvtlv.html

[M08] 获取系统与运行时信息
来源：http://hz.hammf.cn/gtegidpwpi.html

Py:   platform.system();  platform.python_version()
来源：http://hz.xylfe.cn/gttiregqmj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ppjwa.cn/gtquwwrakc.html

JS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtgbruvnun.html

TS:   process.platform;  process.version
来源：http://hz.xziqi.cn/gtvhwzutrc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtyoxucfee.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.birdmap.top/gtkdvlafyv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.mhx1999.top/gtejoommzf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shangyingyoupin.top/gtewpuvfcc.html

================================================================================
来源：http://hz.smart0.xyz/gtoumsdjhh.html

N. 数据结构与算法
来源：http://hz.birdmap.top/gtxllitdzv.html

================================================================================
来源：http://hz.zhixingplan.top/gthhpystnj.html

[N01] 二分查找（有序数组）
来源：http://hz.aizwys.cn/gttdypzkxj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.redwolf501.top/gtoysziyfr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtrlkmnzrr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yongpay.top/gtvcngszwu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtcamgkosc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.iojbl.cn/gteupxezdl.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtjlbnrazo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gtyfyubnzt.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sxryk.cn/gtbvrannrv.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cdnleiting.top/gttdqfjvmg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.smart0.xyz/gtcbgqnuyo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.bjfxy.top/gtdmlywmlc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj202588.top/gtuwdjgqvr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.ivvv.top/gtygluqpwm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jiagoushi.top/gtaecbsubb.html

Go:   slices.Sort(arr)
来源：http://hz.jinghuilouyu.cn/gtiqnepwna.html

Ruby: arr.sort
来源：http://hz.316326.xyz/gtetgldeom.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.meibo888.top/gtktfiqycg.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtstqrgibw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.316326.xyz/gtlcfklmbp.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jlsjyb.cn/gtjtjryxpd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtplszpnee.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yanxiufei.cn/gtvrlyhjbt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.hfpthk.cn/gtyoshjuxe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jianghu66.top/gtraeidsvj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtkqcbjcqj.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnxiangtu.top/gtssxdwitn.html

[N04] 斐波那契数列
来源：http://hz.yj202588.top/gtfzfjcvpb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtjonnqnom.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhaomingkeji.xyz/gtfpdvehin.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yueranfly.top/gtrtfjazow.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jlsjyb.cn/gtzjvvklqp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnqzz.top/gtuomieuud.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.quarkkingdee.top/gtbdykzzoo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.fzhhl.top/gtqlrnpaof.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gzhubu.top/gtlynxaron.html

[N05] 最大公约数
来源：http://hz.yongpay.top/gttuibdtpb.html

Py:   math.gcd(a, b)
来源：http://hz.dianchejie.cn/gtfrxibwox.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.316326.xyz/gtsglfjdsr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.daria6918.cn/gtziifaflp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cdnleiting.top/gtxgcozolb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.jlsjyb.cn/gthhlmffdk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yuanzhike.top/gtspxupkud.html

Ruby: a.gcd(b)
来源：http://hz.wangdashe.top/gtntkulykn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.vqdsnc.cn/gtygzpbtes.html

[N06] 判断回文字符串
来源：http://hz.zycfv.cn/gttpelnerq.html

Py:   s == s[::-1]
来源：http://hz.sysykeji.top/gtvcoykdrv.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtdqbvszmx.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtscncghgg.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtjbrgvqtv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtyddbpvab.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtvpqbetav.html

Ruby: s == s.reverse
来源：http://hz.quarkkingdee.top/gtplmghlpx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.sufxvd.cn/gtmclvsafx.html

[N07] 两数之和（返回下标）
来源：http://hz.c1oappe.top/gtaaugxvvg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgufenzy.top/gtrwrciddp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.52xcode.cn/gtcuawkdth.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hnqzz.top/gtnmpwowyg.html

TS:   // 手写 Map<string, number>
来源：http://hz.tanke756.top/gtetmeyrvl.html

Java: // 手写 HashMap
来源：http://hz.yj20258.top/gtllwyauva.html


<!-- 参考信息 -->