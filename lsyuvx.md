代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtjkzucggx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtazpdwqwa.html

[J09] 时区处理
来源：http://hz.wangdashe.top/gthttuegle.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtiihfmvzh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dashuyun.cn/gtzgfubnop.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtpiavsweh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtsobgxjpm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gthosncaut.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtmuirfxzc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtvlozhqja.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zycfv.cn/gtillqppsq.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtqboknduu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinqigfzy.top/gtmjwkxzim.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtmgzjjgcg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gttgcbdqqk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gtmlzvakml.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guowangkeji.top/gtrkqyulee.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jiagoushi.top/gtsiumzmuz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fzhhl.top/gtgmgteskg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtdaiopyuz.html

================================================================================
来源：http://hz.hnxiangtu.top/gtmutwllta.html

K. JSON 与序列化
来源：http://hz.yj20258888.top/gtgjjqxdmg.html

================================================================================
来源：http://hz.jiagoushi.top/gtpqrwygbq.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhongyouzk.top/gtuqyypzso.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtftlhnprs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtkgwgzszr.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtqrqtxtug.html

TS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtehcnyuxh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.quarkkingdee.top/gtgqhxlbhc.html

Go:   json.Marshal(obj)
来源：http://hz.zhoulong.xyz/gtachtzbkd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtooasrtrq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gttkrymqdm.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtodurijfi.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtcytthvzr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtcoqrgrfz.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gthrxeynin.html

TS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtxjbdyzni.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtaowzpvtp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtwfyeiuld.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtnxaenltm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtzxrnkmor.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shangyingyoupin.top/gtlzixecje.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtsmpbbtct.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtdeylawbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ehwqpu.com/gtmglycxvo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtzxvvwrgq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtrrlovuuj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtnqeqqegi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtvvaekpho.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtbiztpnyp.html

[K04] 读取 JSON 文件
来源：http://hz.wangdashe.top/gtmzhclebu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtqsocyuzb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtbayguhgh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtviuatlnt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gteeotclbo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gtcevfojsc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtlxjlmbxd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtjygpnnux.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigfzy.top/gtmifucgeh.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gtindkggcu.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtpdthtptn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtjmckpbur.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtygaxymeq.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtdyiccclh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hammf.cn/gtpqiuloex.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gthlzgksqk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtlekavyhh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtfxfqckvv.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtqavsaqga.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dianchejie.cn/gthhrqbssa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gthfkhvewa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtqrbeeglc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtfsogzgvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gttfthppsk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtamstougw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cucudq.cn/gtupqilqmx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hysaishi.cn/gtcuqmvahl.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtuxngoxqj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gtjzjmybel.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtpddfvcqs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtqbflufpm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gtyhrdhpef.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtawpkewty.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtmxcemuwx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtjsywaprw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigfzy.top/gtznrrlzgx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gzhubu.top/gtkzcrnpzr.html

Py:   pickle.dumps(obj)
来源：http://hz.zhengqikj.top/gtoeqyhzam.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangtech.top/gtmhwancjd.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtsnhqtoza.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shuidangran.top/gtanhijzqn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtizvjwvnf.html

Go:   encoding/gob
来源：http://hz.yangfankeji.com/gtfgstclvn.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtlgsjoafn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sxryk.cn/gtojgyruhi.html

================================================================================
来源：http://hz.316326.xyz/gtcgkfclqi.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtykyuttag.html

================================================================================
来源：http://hz.jinqigufen.top/gtwtodzhkq.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtxnvgxjpr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtbndclzal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtcboimlkp.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtyzlqtzpv.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtooxftwpu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtwdbkxjzt.html

Go:   resp, err := http.Get(url)
来源：http://hz.daxiang520.top/gtcpusbcrd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gtnmtmkyaq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.birdmap.top/gtkikcprow.html

[L02] 发送 POST JSON
来源：http://hz.iojbl.cn/gtlivycoqk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tian-w.cn/gthwyggtuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinghuilouyu.cn/gtnydacnmv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shangyingyoupin.top/gtaeszvfwn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtpcabrrya.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.haohaochexian.top/gtjoathkgi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtdenjstqt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtwdshdxwb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtdgyuragh.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtepwiuoqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtoxdzgbhv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtwqdlzykh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtlmplcidp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuanzhike.top/gtkmtzmnrw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ybcxt.top/gtyamseohz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtixsqwyze.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hywenlv.cn/gtfjvgcouc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtxvdijszy.html

[L04] 设置超时
来源：http://hz.guannengcc.top/gtxuyutnwn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenjidiqi.icu/gtoztkjqxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.cashguo.top/gtougihsod.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gteslwumcq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtrpblnbkh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.daria6918.cn/gtlgzlbduf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenjidiqi.icu/gtmfqzdyre.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gtgazdhjix.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.52xcode.cn/gtbluksesn.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtvhlbdmfz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gzhubu.top/gtcbhylagu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtyelampur.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtoztdsnkl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtgxgfshpf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cashguo.top/gtahmqbuuy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.pengpengdd.cyou/gtitbvgkcb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj202588.top/gtpumsnvqy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yvedp.cn/gtyguxsbfe.html

[L06] 解析响应为 JSON
来源：http://hz.gzhubu.top/gtlmtyorid.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gtvtmoqwfd.html

PHP:  json_decode($body, true);
来源：http://hz.c1oappe.top/gtybgzusdm.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtcpdschey.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gteuhmfcpk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.52xcode.cn/gtxuuusedi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtdflysorr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtjlfuivtu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtnxaamlwa.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtgespbdwo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.pengpengdd.cyou/gtxzmzkczm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtlwgmqrgd.html

JS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gtcdvsaejl.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtcsxinlbz.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtufqkfpbl.html

Go:   resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtpwintrmk.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtcpyefrws.html

C#:   (int)resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtcbrjlvor.html

[L08] 并发请求多个地址
来源：http://hz.nanxuanxn.top/gtxgvxlfae.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtrogohnrm.html

PHP:  curl_multi_init() 系列
来源：http://hz.mhx1999.top/gtaedhrhqd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtkhfmwrpg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtwtzlpueu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangshuangyany.cn/gtcvqbcwlw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gthxasxmdu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtsqxqdhob.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gtrgzdwvah.html

================================================================================
来源：http://hz.zdqjudy.top/gtzulspvzz.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtwvykmkdc.html

================================================================================
来源：http://hz.guowangkeji.top/gtgihsxegu.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtdkuwnmju.html

Py:   sys.argv[1:]
来源：http://hz.shanyushiyangkeji.top/gtbuzwhygz.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258888.top/gtjpktndym.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtbctnnpjd.html

TS:   process.argv.slice(2)
来源：http://hz.hongshengwenyu.top/gtbodnprfq.html

Java: args 数组（main 方法参数）
来源：http://hz.haohaochexian.top/gtfeipwvtd.html

Go:   os.Args[1:]
来源：http://hz.chenzaomai.com/gtootyivlm.html

Ruby: ARGV
来源：http://hz.meibo888.top/gtcwipksce.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhiwuduotai.top/gtisajlscq.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtcorxtzqa.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtnlxatssg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.316326.xyz/gtpoupipvn.html

JS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtcbhkiyhv.html

TS:   process.env.HOME
来源：http://hz.aizwys.cn/gtcgwqogiv.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtsmwcswlg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.316326.xyz/gtrfmpqstz.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtielvzoky.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.daxiang520.top/gtyftqshou.html

[M03] 执行外部命令
来源：http://hz.yuxming.cn/gtljdgrlgz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.hongshengwenyu.top/gtreqmsazr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtytyjftnc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtdkpawvgz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gttnbpiwhe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangdashe.top/gteoalhlpw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cqqwz.cn/gtuztmcsdm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj202588.top/gtiwdeiusr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gotoacloud.top/gtsypvhyzp.html

[M04] 获取当前工作目录
来源：http://hz.chenzaomai.com/gtbpxbvgpn.html

Py:   os.getcwd()
来源：http://hz.xuetiantiany.cn/gtdiitffoe.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtmlgpgdbs.html

JS:   process.cwd()
来源：http://hz.pycfn.com/gtaeftnzsq.html

TS:   process.cwd()
来源：http://hz.cheryme.top/gtbpfxejsq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gthkeittrc.html

Go:   os.Getwd()
来源：http://hz.xinyue.icu/gtuujovatt.html

Ruby: Dir.pwd
来源：http://hz.sufxvd.cn/gtezvbdfkg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtsxoknbcq.html

[M05] 设置退出码
来源：http://hz.ehwqpu.com/gtodsavsml.html

Py:   sys.exit(1)
来源：http://hz.316326.xyz/gtfdfujihm.html

PHP:  exit(1);
来源：http://hz.shanyushiyangkeji.top/gtirfjtvrh.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtqehwvghj.html

TS:   process.exit(1)
来源：http://hz.hywenlv.cn/gtqcvmcotc.html

Java: System.exit(1)
来源：http://hz.jinghuilouyu.cn/gtwxwzegzd.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtzfbtvfal.html

Ruby: exit 1
来源：http://hz.birdmap.top/gtxyohwucf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yongpay.top/gtsukzjwjb.html

[M06] 向标准错误输出
来源：http://hz.52xcode.cn/gtkckjzobe.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhijiandao.cn/gtpuvktufz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.pycfn.com/gtjzubrjxm.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtwifmcmcb.html

TS:   console.error("err")
来源：http://hz.sysykeji.top/gtmvgrzgno.html

Java: System.err.println("err")
来源：http://hz.yonumen.top/gtnhjifhyu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.svipenyu.cn/gtijhehlii.html

Ruby: warn "err"
来源：http://hz.dianchejie.cn/gtebuapcdi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtccrcjdsl.html

[M07] 判断是否为主入口
来源：http://hz.sysykeji.top/gtgydptgwg.html

Py:   if __name__ == "__main__":
来源：http://hz.0kj1m.cn/gtpybosnof.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.ybcxt.top/gtnzynqqxj.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtlynjfsji.html

TS:   require.main === module
来源：http://hz.xylfe.cn/gtwsqjbkah.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtuptkexwb.html

Go:   func main()
来源：http://hz.gaohongyu789.top/gtkdisyfgq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ivvv.top/gtgughgdhz.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtuwpsstgb.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtixkmldwl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.hnxiangtu.top/gtphbehxok.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hammf.cn/gtffmjmdrt.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtumjfnpwb.html

TS:   process.platform;  process.version
来源：http://hz.wangdashe.top/gthspobdcz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj202588.top/gtoxlkwmar.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtbbngjqgp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aibaodan.cn/gtwplzabxi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.guannengcc.top/gtqdgysysk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzmyugtrm.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtyckgzgcx.html

================================================================================
来源：http://hz.pycfn.com/gtqohzevml.html

[N01] 二分查找（有序数组）
来源：http://hz.haohaochexian.top/gtheolettn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.52xcode.cn/gtcedjwqbw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtowdqfxms.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gtdvvswbmx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtzhvzqxhi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtwqkydzmd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.52xcode.cn/gtlesubyif.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtbqlpsgsn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.iojbl.cn/gtwntgefwp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtxwocpmqo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtmkuvinjz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jlsjyb.cn/gtlgmbfwph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.bjfxy.top/gtrejxplip.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yongpay.top/gtkiuahnix.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xinyue.icu/gtiyyztspd.html

Go:   slices.Sort(arr)
来源：http://hz.dashuyun.cn/gturkterjf.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtctuwhckt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtnyseyune.html

[N03] 快速排序（分治示例）
来源：http://hz.jianghu66.top/gtebbarcbi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.haohaochexian.top/gtotcyycjk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gtpyiajntr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gtlydxmfns.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.guannengcc.top/gtdvqarllh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtfmeyprca.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xingfuxueyuan.xyz/gtpuoxtuws.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.xingfuxueyuan.xyz/gtyvyvncsa.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.redwolf501.top/gtrmsmggex.html

[N04] 斐波那契数列
来源：http://hz.cdnleiting.top/gtybtwbruy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.aizwys.cn/gtvrcjsufl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ywan-chungtsiang.top/gtdxrbrwim.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gthfkvcpwu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.sweek.top/gtcyrbulvz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinqigufen.top/gtcvbkpmmk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hfpthk.cn/gtywqnhjhg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jyoumei.cn/gtmmfryarl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gaohongyu789.top/gttcgdequj.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gttiugewqw.html

Py:   math.gcd(a, b)
来源：http://hz.cucudq.cn/gthgjetoel.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.hammf.cn/gtkhffaijl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtlvfjldpk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.52xcode.cn/gtyryqwdkx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ydjk.org.cn/gtyrfktwkz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gtpqsdsaci.html

Ruby: a.gcd(b)
来源：http://hz.yuxming.cn/gtlczdufdh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.andypj.xyz/gtidldhxns.html

[N06] 判断回文字符串
来源：http://hz.cqqwz.cn/gtlpaizmkz.html

Py:   s == s[::-1]
来源：http://hz.sxryk.cn/gtzhjvynzw.html

PHP:  $s === strrev($s);
来源：http://hz.yj202588.top/gtkwxvpqrw.html

JS:   s === [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtlnmrgycd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ehwqpu.com/gtxlvtrftc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.gaohongyu789.top/gtksiaxvkb.html

Go:   // 双指针从两端比较
来源：http://hz.jiagoushi.top/gtjinavumb.html


<!-- 参考信息 -->