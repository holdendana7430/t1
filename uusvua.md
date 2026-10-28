代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtpmvkubao.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gttijjrbkj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtflnutgua.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.c1oappe.top/gtxkomhurq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtfkkumtnc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtxgpbhckc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtidakcbeu.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtkswhckze.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgfzy.top/gtezxgulaj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtruyefvfr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtwnosdzeb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtakoysqjr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtrnmpogcl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dashuyun.cn/gtlhhzancx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtszwgkqqk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtlacugtne.html

================================================================================
来源：http://hz.jqgfzy.top/gtujhtltmx.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gttggscsxo.html

================================================================================
来源：http://hz.yj20258888.top/gtfmahtsuf.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuxming.cn/gttqzgwkpl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtrhgofvuk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gteshpljdk.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtedbanwfr.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtsyieslrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtkyjyretd.html

Go:   json.Marshal(obj)
来源：http://hz.jiagoushi.top/gtgjppjrzu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtowsvbjie.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gttvybinqc.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtfmzjorsg.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtgkqolfqs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtklccqsgi.html

JS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtcxiaerbt.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtgesazqcp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtrldzwffu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtrmpsuolp.html

Ruby: JSON.parse(s)
来源：http://hz.hammf.cn/gtrgjhmusf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtxygbzjgh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tian-w.cn/gtyfucapsn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtecmkxoow.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtnruccijp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtwizlbbfe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtcmwkrzpy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.quarkkingdee.top/gtasjzedyz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.meibo888.top/gteuubfcyh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.birdmap.top/gthpgyiwbw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jyoumei.cn/gtjpmaqntz.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtkqvbxucu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtdllbhwgz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangshuangyany.cn/gtngfondub.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtczxfnexq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtepyvqprb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtrjfnelhb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtwgjnlozv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtblvxchkw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gtbfaenxov.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtrvvwqqgc.html

Py:   copy.deepcopy(obj)
来源：http://hz.hfpthk.cn/gtffxytmyc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtknunzcsc.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtyyxtnrhp.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtyzoryrem.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gtaxbmvlqu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtdfwuiwlz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.havefunace.top/gtrsoixeyx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtbqxxupqo.html

[K06] 解析 URL 查询串
来源：http://hz.yuxming.cn/gtlrqzqizz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtdclucgiy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtxdbsxaej.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtlkmndsty.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtguhiecvm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtubfbwllk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gteaptpzqg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtvivcsbnk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtyxsosazi.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtxfydzbne.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtnbmybnxv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gthazriocc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtlhapyfjx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtbulegdaw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtzgodbdxt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtapzanmbs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cqqwz.cn/gtmzjgzzba.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtzsfcvxlh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gtzzpogdpq.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtluuguban.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtddtrkqzg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtipypdrzm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtgebogwjv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zycfv.cn/gtnroypevz.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtbicqivab.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtojzwsqwv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtysuajhwm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyfkurwqx.html

L. 网络请求
来源：http://hz.redwolf501.top/gtlivovlca.html

================================================================================
来源：http://hz.yj20258.top/gtspsryhbt.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtbidzmwvt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtefnorfow.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtolwlznhn.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtffpctkhf.html

TS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtfcswfwyt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtdrwganyf.html

Go:   resp, err := http.Get(url)
来源：http://hz.tianlin.xyz/gtbgctfbro.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtlmmimpvr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.kuanghao11.cn/gtzsqhcqll.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtgtayrkhf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.mhx1999.top/gthjymdseb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gteavamose.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gterqhqxmn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gteybwbgkn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yvedp.cn/gtnzigvvof.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cheryme.top/gtdjiyqtac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtyeqjnygz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.redwolf501.top/gtpalcmlrw.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtdqdsrvgo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtnugmfiye.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtjxfoqwko.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtbbruhgbm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gtxxwfcuxz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenjidiqi.icu/gtdamhlxyn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtjhdpchuy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258888.top/gtrmeonliy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtinsgfdtd.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtqiqeutjf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtdnntygvu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxinkj.top/gtcwogvxoy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtyagxpaqk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtpmgqpzkv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tian-w.cn/gtycdrymvc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.0kj1m.cn/gtuslhhhrw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtrwjocxzw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangdashe.top/gtzmugumoy.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtxotgqnrg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtvkdyzbie.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtrgiuiefm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtczenxmkc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydzc1.top/gtrqzlegkn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sysykeji.top/gtuczqlcxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinghuilouyu.cn/gtjffrvrem.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtcowxhcnd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258888.top/gtsaetpbaw.html

[L06] 解析响应为 JSON
来源：http://hz.vqdsnc.cn/gtnwmhrtnn.html

Py:   resp.json()
来源：http://hz.ppjwa.cn/gtxlczrbwj.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtcnspurqv.html

JS:   await resp.json()
来源：http://hz.daria6918.cn/gtobhmsrja.html

TS:   await resp.json()
来源：http://hz.haohaochexian.top/gtrasvufpn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhaomingkeji.xyz/gtwbpyuqwr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenlongwang.top/gtacvpmhuk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtoiqdvqeg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtpbxzcvas.html

[L07] 处理 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtgtnasdbi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangdashe.top/gtdhdmvwsc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.bjfxy.top/gtgblinzul.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtktjsffkr.html

TS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gtuhppzlfc.html

Java: resp.statusCode()
来源：http://hz.dashuyun.cn/gtaxctdtet.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gthxiluvgl.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtgnhbhsca.html

C#:   (int)resp.StatusCode
来源：http://hz.pycfn.com/gtfocmaisq.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtyvbuxtxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnqzz.top/gtlbkiaszc.html

PHP:  curl_multi_init() 系列
来源：http://hz.daria6918.cn/gtcnedgshd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtomtivvoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.9152youxi.cn/gtmtfcbuhk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtfrcvdbma.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtztygkspe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtwdyletve.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtjuoynwvq.html

================================================================================
来源：http://hz.zdqjudy.top/gtvfwviuij.html

M. 命令行 / 进程 / 环境
来源：http://hz.jianghu66.top/gtfuynaxno.html

================================================================================
来源：http://hz.yongpay.top/gtueiryxlz.html

[M01] 读取命令行参数
来源：http://hz.yuxming.cn/gtzxyarllp.html

Py:   sys.argv[1:]
来源：http://hz.gaohongyu789.top/gtneuvxzfy.html

PHP:  $argv;  $argc;
来源：http://hz.guannengcc.top/gtnphswyfs.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtpeycnqbm.html

TS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtczxgmgzw.html

Java: args 数组（main 方法参数）
来源：http://hz.yongpay.top/gtzetlffdl.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtlvshkvye.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtmovfqmbz.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtxcccmqef.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gthjtejais.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtkibuidcr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sxryk.cn/gtrxamijyq.html

JS:   process.env.HOME
来源：http://hz.yvedp.cn/gtkvjgfqau.html

TS:   process.env.HOME
来源：http://hz.sufxvd.cn/gtafrsxghz.html

Java: System.getenv("HOME")
来源：http://hz.yj20258.top/gtrfrqetmz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hnqzz.top/gthyvqzgey.html

Ruby: ENV["HOME"]
来源：http://hz.nanxuanxn.top/gtnafjtqrm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhaomingkeji.xyz/gtqtolhuee.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtoichomyb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guannengcc.top/gtalrmqgcc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pycfn.com/gtdmbyxfcb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.fengsongda.top/gtcidigtzf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtsdqefxap.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinyuanbaomall.cn/gthjqfjked.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shanyushiyangkeji.top/gtviriiocz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtyvxehnjc.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtvhzxoskg.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtuiiqscly.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gtggjzecub.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtuwhjaozf.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtpqlfcxys.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtidpsslok.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtkrjkxddo.html

Go:   os.Getwd()
来源：http://hz.ybcxt.top/gtkoahktux.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtsqmghicl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sysykeji.top/gtesvieola.html

[M05] 设置退出码
来源：http://hz.fengsongda.top/gtbcmufkxb.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtjkrwmmte.html

PHP:  exit(1);
来源：http://hz.snrcjt.cn/gthwytezne.html

JS:   process.exit(1)
来源：http://hz.xuanzx.com/gtfyrmkpbp.html

TS:   process.exit(1)
来源：http://hz.aizwys.cn/gtxgsweohn.html

Java: System.exit(1)
来源：http://hz.birdmap.top/gttclvtuln.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtpuztdota.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtbgfderhc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.cheryme.top/gtusgchcgv.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtyezatfvt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hammf.cn/gtxetxzhkg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.wangdashe.top/gtlxsskxay.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtoykrmatf.html

TS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtatjogxqh.html

Java: System.err.println("err")
来源：http://hz.shzxlz.cn/gtbsbdolgl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtqiqrxerp.html

Ruby: warn "err"
来源：http://hz.cqqwz.cn/gtcluhcgqu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtosgofhks.html

[M07] 判断是否为主入口
来源：http://hz.zhaomingkeji.xyz/gtqugcaydv.html

Py:   if __name__ == "__main__":
来源：http://hz.yuanzhike.top/gtjfhohlle.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtmdjsxato.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtvjlfbjoc.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtsxbiyzzz.html

Java: public static void main(String[] args)
来源：http://hz.chenlongwang.top/gtgjjzawsh.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtfbnagdei.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtjcgynutj.html

C#:   static void Main(string[] args)
来源：http://hz.snrcjt.cn/gteiyjrdmj.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtqltnefek.html

Py:   platform.system();  platform.python_version()
来源：http://hz.shanyushiyangkeji.top/gtecvbaraz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dianchejie.cn/gtybbmgkdo.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gttteejlur.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtupyufexb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yuxming.cn/gtunpbxubb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xuetiantiany.cn/gthiyosyro.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.birdmap.top/gtwtxynviu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhengqikj.top/gttawfjabo.html

================================================================================
来源：http://hz.jiagoushi.top/gtbhliaktm.html

N. 数据结构与算法
来源：http://hz.tanke756.top/gtlclvpyzp.html

================================================================================
来源：http://hz.birdmap.top/gtafludrwe.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtpospmadd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.fzhhl.top/gtexjjdnxw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.quarkkingdee.top/gtyjaxdbfb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgufenzy.top/gtkcuzrhfx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhiwuduotai.top/gtlytoothe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ehwqpu.com/gtsbqgtszp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gttfnmxhyl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ywan-chungtsiang.top/gtqfmhseqh.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.vqdsnc.cn/gtddfwnzfd.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtnysdjqpv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtsguhnuhk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shzxlz.cn/gtqxmzlkpf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtyscdtuhf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yanxiufei.cn/gtrnimxzti.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.kuanghao11.cn/gtapndtxes.html

Go:   slices.Sort(arr)
来源：http://hz.yvedp.cn/gtcgsmbeql.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtkiunqazf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yuanzhike.top/gtqhpxsuvp.html

[N03] 快速排序（分治示例）
来源：http://hz.gotoacloud.top/gtibnvlqqh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yanxiufei.cn/gtqhzoaysv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.chenlongwang.top/gtyzeshepy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtzamsluyz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shangyingyoupin.top/gtvmnunups.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.fzhhl.top/gtzqnjdnen.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.chenjidiqi.icu/gtdhjjdfpl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhijiandao.cn/gtlaaniqvf.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hongshengwenyu.top/gtagihhslv.html

[N04] 斐波那契数列
来源：http://hz.ydjk.org.cn/gttxavovhh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258.top/gtxqskqmzc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tianlin.xyz/gthxzcuobx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ivvv.top/gthquojfbt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.svipenyu.cn/gtfjtudjbc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yanxiufei.cn/gtxqfdjogz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.birdmap.top/gtlyotczql.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hongshengwenyu.top/gtnfhlbnaz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtnxzqmrve.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gtzggeexse.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtqwozaojf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgfzy.top/gtgdnvqhik.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj20258.top/gttdqgdipz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.c1oappe.top/gtvpssxnvj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.sxryk.cn/gtenkwxjrc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtfclmkwly.html

Ruby: a.gcd(b)
来源：http://hz.daxiang520.top/gtehxhyeqo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.chenjidiqi.icu/gthtdwbrft.html

[N06] 判断回文字符串
来源：http://hz.xingfuxueyuan.xyz/gtfgcerxze.html

Py:   s == s[::-1]
来源：http://hz.zhoulong.xyz/gtjcvjxbgx.html

PHP:  $s === strrev($s);
来源：http://hz.mhx1999.top/gtyascvfmb.html

JS:   s === [...s].reverse().join("")
来源：http://hz.birdmap.top/gthftsienf.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtyvzprlfb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtnbphxqfs.html

Go:   // 双指针从两端比较
来源：http://hz.pycfn.com/gtnmtpwkog.html

Ruby: s == s.reverse
来源：http://hz.yj20258888.top/gtsvviyqpp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtmwluzzjp.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gttcquodmc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shzxlz.cn/gtiflntmag.html


<!-- 参考信息 -->