代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gthfqonzvc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtarvqytnj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gthycxrzox.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jiagoushi.top/gtabvailfu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tanke756.top/gtwerawdth.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.svipenyu.cn/gthueifwtf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtcnwdkppp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtwipsriye.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkdenqwsj.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gtqevrlisf.html

================================================================================
来源：http://hz.birdmap.top/gtbgdhmrlu.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtxwemtpbl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtqwhctrrq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtkbpybztk.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtsbxogsrk.html

TS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtgrcupisb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yueranfly.top/gtaadiavhe.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gtajagfnko.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtnegrxnhf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtrrqtbjhb.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtlmvjpynn.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtjfwqzukg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtqdjsamqh.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtddchpiaa.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtaageapzd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtpypbqfpl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtnnxptkap.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtwrvlhlfj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtflfrtieg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aizwys.cn/gtlpixugnq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtifvegftm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtatwwfseh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtelornyuz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtsmainzrw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yangfankeji.com/gtpczpzfut.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtgsrorzrg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtgkbsjrms.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gtqgmgasol.html

[K04] 读取 JSON 文件
来源：http://hz.fengsongda.top/gtcacjtzib.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtpsmxlypk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtbhacznmk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtkrvnzyjk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtssxypdog.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtpscqqtyl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtmaceouhe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gteuoxymaz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtcvtlchdu.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gttnskpvrf.html

Py:   copy.deepcopy(obj)
来源：http://hz.aizwys.cn/gtgbbtgjwy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aizwys.cn/gtjeibrhtj.html

JS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtjugtzgvo.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtxpyabtrl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtqdwfltmm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtvqwnnxij.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtaakhhzjm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yongpay.top/gtybptoyxn.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtagmehusl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtiswptnav.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.birdmap.top/gtvuiwtfex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtttvaocae.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtqxiwbaaq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtzzwnpxwm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fzhhl.top/gtbkspylxv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtxhyoodtj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gtzvzjlwnh.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gttirjmazn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sufxvd.cn/gthigltwib.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.mhx1999.top/gtdqfycnky.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtzoagfmwj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gthbudqxpe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtctdwbuxh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gtopgdtwvv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtxkthckxy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtowzqioez.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xuetiantiany.cn/gtqclrvqls.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtkxfuhbqp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtoipuaobs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtwgptdnog.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtncgntspy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtevtchxno.html

Go:   encoding/gob
来源：http://hz.fengsongda.top/gtfeqihxmx.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtgkddsxol.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuanzx.com/gtboxmssba.html

================================================================================
来源：http://hz.gzhubu.top/gtsdbreerj.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtqjtzuvkd.html

================================================================================
来源：http://hz.aizwys.cn/gthbelwiqf.html

[L01] 发送 GET 请求
来源：http://hz.aibaodan.cn/gtgczlrhfv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtnliimbgv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtqavypweo.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtxtvumroo.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtrbvphamj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fengsongda.top/gtpwzzmczj.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtltgajgou.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yonumen.top/gtrlkccuss.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtejmdfvbb.html

[L02] 发送 POST JSON
来源：http://hz.cqqwz.cn/gthkqadlkw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.aibaodan.cn/gtijxznydi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sxryk.cn/gtrjkinvuh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtmuihsfzj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtluhmiblg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtmevpqlja.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.0kj1m.cn/gtymuphzdv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtykejmzvz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuetiantiany.cn/gtncnzfwpu.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtutzphysm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangshuangyany.cn/gtcdnamerf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.9152youxi.cn/gtzpnojeyj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtgmtzgxfz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtbfxdihql.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gtoiijuiug.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtcithfkjm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangdashe.top/gtxewxgjrm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtfyzbrhpb.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtsufzjuxk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtsprfcoss.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangkeji.top/gtzqcjkpmd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtxpjwsrcr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhixingplan.top/gtfgabwphm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sufxvd.cn/gtsmznscyv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zycfv.cn/gtknlhmmfx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.andypj.xyz/gtcryjpvsa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jinqigufen.top/gtmssmcqzo.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtdozedlua.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gtycsceucu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtemlgiqcr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yangfankeji.com/gtqlziijng.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtudmnzrct.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtvwnchbru.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shzxlz.cn/gtyadyxwyh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yuxming.cn/gtcyngdbeo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.quarkkingdee.top/gtwyycsbud.html

[L06] 解析响应为 JSON
来源：http://hz.hongshengwenyu.top/gtfduqkenv.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gteplrcjeb.html

PHP:  json_decode($body, true);
来源：http://hz.ydjk.org.cn/gtzroaqqcm.html

JS:   await resp.json()
来源：http://hz.shzxlz.cn/gtiallscua.html

TS:   await resp.json()
来源：http://hz.xingfuxueyuan.xyz/gtedfhtnig.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.haohaochexian.top/gtecgsaahi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtgciyrxng.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtniosxica.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtfxsljoqt.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinghuilouyu.cn/gtkotkxpbw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shuidangran.top/gtldnidsyf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinqigufen.top/gtitgnxbiw.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtotblezed.html

TS:   resp.ok;  resp.status
来源：http://hz.zhijiandao.cn/gtxddxwdpv.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtpldbtrto.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtitoxaywr.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtlbproulq.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtkfthcisk.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtbagmlvxg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.tianlin.xyz/gtodcpaqnz.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtieonnikt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gthjprwxfe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtithsrtiu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.snrcjt.cn/gtwgxkbxsg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenzaomai.com/gtnxrrehzm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtsnultxrc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sufxvd.cn/gtovmrszso.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlrgfkuqp.html

M. 命令行 / 进程 / 环境
来源：http://hz.cdnleiting.top/gtnwoazsfo.html

================================================================================
来源：http://hz.9152youxi.cn/gtwdzuixhy.html

[M01] 读取命令行参数
来源：http://hz.0kj1m.cn/gtgpeuathg.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtlovukvse.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtgkztosso.html

JS:   process.argv.slice(2)
来源：http://hz.jinqigufen.top/gtqxyfvuaj.html

TS:   process.argv.slice(2)
来源：http://hz.yuxming.cn/gtxnwlrqte.html

Java: args 数组（main 方法参数）
来源：http://hz.316326.xyz/gtdzgwoxzr.html

Go:   os.Args[1:]
来源：http://hz.dashuyun.cn/gtxmkiextf.html

Ruby: ARGV
来源：http://hz.ppjwa.cn/gtcgntgktq.html

C#:   args 数组（Main 方法参数）
来源：http://hz.c1oappe.top/gtbicchzsh.html

[M02] 读取环境变量
来源：http://hz.haohaochexian.top/gteynpwdcg.html

Py:   os.environ.get("HOME")
来源：http://hz.sweek.top/gtiulfwzls.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jqgufenzy.top/gtfaqqdurg.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtyznnhpwi.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtnvisibjy.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gtblmtwtcm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtzrhuaayb.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigfzy.top/gtkpcusxpg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yj202588.top/gtrobkhree.html

[M03] 执行外部命令
来源：http://hz.cucudq.cn/gtycqthigl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtntohwpik.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jlsjyb.cn/gtvdaczwtf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtgngymsnn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtdeiazxmc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xylfe.cn/gtiefwqhhi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ybcxt.top/gtgsezofky.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shzxlz.cn/gttvtydbnn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gttzlvazfn.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtbqptqrea.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtyoxkuiki.html

PHP:  getcwd();
来源：http://hz.yj202588.top/gtbobpohwy.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtccamtywa.html

TS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtojzyvonk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.svipenyu.cn/gtndjskzol.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtzuztdjpg.html

Ruby: Dir.pwd
来源：http://hz.fzhhl.top/gtnvokradi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtonkvipoq.html

[M05] 设置退出码
来源：http://hz.svipenyu.cn/gthitogvar.html

Py:   sys.exit(1)
来源：http://hz.hnqzz.top/gtgaqtwpsb.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtjnqopzyn.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtftwargbb.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtsbmnfvzf.html

Java: System.exit(1)
来源：http://hz.tanke756.top/gtrqnxuqns.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtgmqwztec.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtsyttvfos.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangdashe.top/gtzjrivjvg.html

[M06] 向标准错误输出
来源：http://hz.yuxming.cn/gtdhyltcuc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ywan-chungtsiang.top/gtzhqiybfa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.cashguo.top/gtcddtvdtl.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtacthydvf.html

TS:   console.error("err")
来源：http://hz.9152youxi.cn/gtybdpjgab.html

Java: System.err.println("err")
来源：http://hz.iojbl.cn/gtkubszanh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtapzitlmg.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gtmindvhkz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hammf.cn/gtjrcidzgz.html

[M07] 判断是否为主入口
来源：http://hz.yangfankeji.com/gtlnsgbwjb.html

Py:   if __name__ == "__main__":
来源：http://hz.jinyuanbaomall.cn/gtmqkyuqdb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtpqdtqcno.html

JS:   require.main === module
来源：http://hz.tianlin.xyz/gtyznytren.html

TS:   require.main === module
来源：http://hz.yvedp.cn/gtbcwbymum.html

Java: public static void main(String[] args)
来源：http://hz.zhixingplan.top/gtfuuhrkee.html

Go:   func main()
来源：http://hz.pengpengdd.cyou/gtxhppwayd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tianlin.xyz/gtjrjvsnbd.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtbogmlvjt.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gtniwzwohf.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hywenlv.cn/gtovfyvesu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cashguo.top/gtqvskoxqf.html

JS:   process.platform;  process.version
来源：http://hz.yanxiufei.cn/gtyjqidutz.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtqxwcosfu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtjqyfgwac.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtzwkfgqfb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtjknzinuw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtgbgcfhfd.html

================================================================================
来源：http://hz.nwbrower.top/gtuizhyvyd.html

N. 数据结构与算法
来源：http://hz.ydjk.org.cn/gtgpfrrnlu.html

================================================================================
来源：http://hz.jiagoushi.top/gtbephhgoz.html

[N01] 二分查找（有序数组）
来源：http://hz.smart0.xyz/gticctgqvy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhiwuduotai.top/gtugwdaupl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.gotoacloud.top/gtscitqimj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jiagoushi.top/gtzkxkwdtz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigufen.top/gtzvcwhxhv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.smart0.xyz/gtnyftqurn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.fzhhl.top/gtmevwxbop.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hnqzz.top/gtxtuoiskq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.zhoulong.xyz/gtxylektnb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtfnmdnvjb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtnbuagmxi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.zhongyouzk.top/gtzwrtjrzg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtoczqvupr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtfbgoyffb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.haohaochexian.top/gtcjcfyqdw.html

Go:   slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtxfizmbqs.html

Ruby: arr.sort
来源：http://hz.ehwqpu.com/gtxvmgdgzi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ivvv.top/gtgcwmtznb.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtmmyovzkq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guowangkeji.top/gtgqqadesy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hongshengwenyu.top/gthudaaevu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtxxgbyopr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.yonumen.top/gtzmhicqds.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gtyurjdfnz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinyuanbaomall.cn/gtuiyblkao.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.snrcjt.cn/gtfongypfu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhongyouzk.top/gtlkvekimd.html

[N04] 斐波那契数列
来源：http://hz.jinqigufen.top/gthodorflq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.havefunace.top/gtqpddwvdf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxuanxn.top/gtewohvhal.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtiqayqnxx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sufxvd.cn/gthlzfcace.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgfzy.top/gtvurclxqm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhijiandao.cn/gtggkvxlub.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yueranfly.top/gtcwzablcy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtbnxjvrnp.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gtpvyeiqos.html

Py:   math.gcd(a, b)
来源：http://hz.gaohongyu789.top/gtroizqomm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.wangdashe.top/gtsielfoma.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtrmvebina.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jyoumei.cn/gtztxkmlgq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtrcuduevn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cheryme.top/gtteeoubzy.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtbcewvgto.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ybcxt.top/gtrzhoopbi.html

[N06] 判断回文字符串
来源：http://hz.havefunace.top/gtsfoztjnv.html

Py:   s == s[::-1]
来源：http://hz.cheryme.top/gtzeblhiis.html

PHP:  $s === strrev($s);
来源：http://hz.yj20258888.top/gtdhcmozhg.html

JS:   s === [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtvzipcyly.html

TS:   s === [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtdeyhljuc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daria6918.cn/gthynbwlzg.html

Go:   // 双指针从两端比较
来源：http://hz.sufxvd.cn/gtjnckgylr.html

Ruby: s == s.reverse
来源：http://hz.cdnleiting.top/gtgccfkhdp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtxnajykzp.html

[N07] 两数之和（返回下标）
来源：http://hz.jinqigufen.top/gtggnemtrj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yanxiufei.cn/gtqooikaqa.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.ivvv.top/gtblwlmfwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shangyingyoupin.top/gtimbufenn.html

TS:   // 手写 Map<string, number>
来源：http://hz.xinyue.icu/gtdkwjffdk.html

Java: // 手写 HashMap
来源：http://hz.cucudq.cn/gtbfopwpoq.html

Go:   // 手写 map[int]int
来源：http://hz.guowangkeji.top/gtugxvtqtn.html

Ruby: // 手写 Hash
来源：http://hz.snrcjt.cn/gtxeqwexfo.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhijiandao.cn/gtitihokkw.html

[N08] 生成全排列
来源：http://hz.yanxiufei.cn/gtnfddejvj.html


<!-- 参考信息 -->