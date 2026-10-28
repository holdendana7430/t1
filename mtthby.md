代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtuutwtjhz.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gtjqwzpyqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gtnhwcsyfj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yongpay.top/gtsrolidxg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.c1oappe.top/gtrwfyyseu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtepblhbya.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hywenlv.cn/gtkqpsvtau.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtxhkecgbl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtmdwosyic.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtbsesoiel.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gthlhvthjz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtefqyvoqn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.c1oappe.top/gtfynjyflu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtsehukpmg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtfwdyzoxh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtxzccouqq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtzwiqlrnz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xinyue.icu/gtepnuiurh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxuanxn.top/gtcjqaulmb.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtqxgimybw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtakjvdfmb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ivvv.top/gtcxnskzlw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtcslicxkq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtmbmumlji.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtwlcnruqo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtmipudvnx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.svipenyu.cn/gtpzjbvmfg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtkozztunh.html

================================================================================
来源：http://hz.smart0.xyz/gtqksovfhn.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtemczsqij.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtncwxfnbk.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtidhesmkl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtwyngfkbn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtepprpcip.html

JS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtvobzwbwh.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtkypcdggl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj20258888.top/gtypqfgivw.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtkhjgjwml.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.bjfxy.top/gtvwowmzro.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangshuangyany.cn/gtlvdqtpyf.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtoupgnutu.html

Py:   json.loads(s)
来源：http://hz.fengsongda.top/gtngkzxlfo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangkeji.top/gthrevuucx.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtbgoopvgg.html

TS:   JSON.parse(s)
来源：http://hz.ivvv.top/gtjzwnfzyo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tian-w.cn/gtgxqozmhc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jqgfzy.top/gtpotsecrf.html

Ruby: JSON.parse(s)
来源：http://hz.zhixingplan.top/gtdiybxeuv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.52xcode.cn/gtpabwqjpl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtbcboxgaf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtbsvxvgtw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtjdfdhtjh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtapjahgra.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtbfxbnluw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtaubifkfv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtmgwsubss.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtotgqfsae.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhengqikj.top/gtmnavbjpf.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtcpiwselj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangshuangyany.cn/gtmbwwvpfj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.nanxuanxn.top/gthrqwsstm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtydtokcwz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtgialmosx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtwcngzrkx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtstssyjva.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtxncmobqt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtbqsfbmlz.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtacqserht.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtwldaqyip.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtafinvdug.html

JS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtfdziyyvn.html

TS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtlcvjiywx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtpfjlexac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtlhgmfmmj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sysykeji.top/gtzlnbciht.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtqcvwkacz.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtnafemhul.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.vqdsnc.cn/gtvcmtaheh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtlfetgour.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtyjmhkpxd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtopirxhoz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtndhxyrpn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtlxwfnnfc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtwpxsjomp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtwirmfaub.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtrddyyjzb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtlnkavqfu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtblxnhlnz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtnaaugvvg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtcqgsoodk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtfwoebyck.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtnokangjv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydzc1.top/gtulbvmlwv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtqachetdh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pycfn.com/gtjgeatwts.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtextmrhyj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtqviszvye.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuxming.cn/gtggfeohuj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtugewabit.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.52xcode.cn/gtlvgufcam.html

Go:   encoding/gob
来源：http://hz.yanxiufei.cn/gtefdblzco.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtzkctdbfk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtwbwwafhu.html

================================================================================
来源：http://hz.haohaochexian.top/gtkcluopet.html

L. 网络请求
来源：http://hz.andypj.xyz/gtpjthtwuj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzdfthtgx.html

[L01] 发送 GET 请求
来源：http://hz.gotoacloud.top/gttpccvcav.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtcizkhegp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtcdsiuofa.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtissdfmod.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtcpaerjum.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xziqi.cn/gtibilcucq.html

Go:   resp, err := http.Get(url)
来源：http://hz.ivvv.top/gtfmjbxkmq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtbuqjrwot.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtqvglqblx.html

[L02] 发送 POST JSON
来源：http://hz.xinyue.icu/gtamesknbn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.redwolf501.top/gtgooeeqne.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gticrmmopn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aizwys.cn/gtkeyjwlqx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zycfv.cn/gttakjxixa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtwzmcpysc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gaohongyu789.top/gtohatllmo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtxxgkgyrh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.c1oappe.top/gtxinjpllp.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtlfijkcwh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtavtndlbf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtixplwtpp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtqlmqgoqe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinqigufen.top/gtfhnumtyt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gtqttnxscj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.52xcode.cn/gtrjfahpbx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gaohongyu789.top/gtfngtzbux.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gthceubzpj.html

[L04] 设置超时
来源：http://hz.pycfn.com/gtfakfusec.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258888.top/gtynnfvjju.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sysykeji.top/gthizeljre.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtljtldzff.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.dianchejie.cn/gtdqizrktn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtopivtfyi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shanyushiyangtech.top/gtriofacpy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtqgbywwnx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.feifeiyinyue.top/gtokkknemd.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtbusjejcp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtezimtiat.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gthyjzfvst.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gotoacloud.top/gtdgzbvcci.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnxiangtu.top/gtviomivvr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.wangshuangyany.cn/gtjmcgjmmd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhixingplan.top/gtlgntcvkt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.haohaochexian.top/gtuggcgvgy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gtrrngoyxd.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtipxrnass.html

Py:   resp.json()
来源：http://hz.yonumen.top/gtiblothbd.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtvzskaqlw.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtbalunpzb.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtcunfqizc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tianlin.xyz/gtrysyjzgg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hfpthk.cn/gtmpytlgfw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nanxuanxn.top/gtwwhkchex.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daxiang520.top/gtkuzsogox.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtqvtmvzbq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gtwamqadpi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtcyrbgikw.html

JS:   resp.ok;  resp.status
来源：http://hz.guowangkeji.top/gtpqwjysng.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtoswkcohd.html

Java: resp.statusCode()
来源：http://hz.52xcode.cn/gtugtbjipa.html

Go:   resp.StatusCode
来源：http://hz.yueranfly.top/gtueftygit.html

Ruby: resp.code.to_i
来源：http://hz.haohaochexian.top/gtpxkuvbhy.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtvwfplkpe.html

[L08] 并发请求多个地址
来源：http://hz.yj20258.top/gtxohnmbdv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sufxvd.cn/gtzhrhspxq.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtzsemhpff.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gthfpazthc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtdeuqjcnx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtfnqogwit.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtrbpptryw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtndawljga.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangshuangyany.cn/gtolnkgvtj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjmjhvqog.html

M. 命令行 / 进程 / 环境
来源：http://hz.cucudq.cn/gtfraaxruo.html

================================================================================
来源：http://hz.yangfankeji.com/gtwjiuahrp.html

[M01] 读取命令行参数
来源：http://hz.daria6918.cn/gtszixksqg.html

Py:   sys.argv[1:]
来源：http://hz.guowangkeji.top/gtbsxrezam.html

PHP:  $argv;  $argc;
来源：http://hz.dianchejie.cn/gtvpjmkjxh.html

JS:   process.argv.slice(2)
来源：http://hz.hywenlv.cn/gtbkdhvgaz.html

TS:   process.argv.slice(2)
来源：http://hz.jlsjyb.cn/gthzlmdeqq.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gtrmquwnhj.html

Go:   os.Args[1:]
来源：http://hz.cqqwz.cn/gtykokugwe.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtshefhoae.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydjk.org.cn/gtanvuckxh.html

[M02] 读取环境变量
来源：http://hz.wangdashe.top/gtgiozkcrg.html

Py:   os.environ.get("HOME")
来源：http://hz.guowangkeji.top/gthubjhjpr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.guowangkeji.top/gteszyqmsa.html

JS:   process.env.HOME
来源：http://hz.yongpay.top/gtucuwxfbb.html

TS:   process.env.HOME
来源：http://hz.guannengcc.top/gtniertimd.html

Java: System.getenv("HOME")
来源：http://hz.xuanzx.com/gtbzvouymq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gtnqyywsyd.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtttuzspnh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gtddbtnboh.html

[M03] 执行外部命令
来源：http://hz.gzhubu.top/gtryelekms.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cashguo.top/gtufkmslhd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zdqjudy.top/gtloczttxm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtonyajmqy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtdzegqncq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtprbmjizu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtkelfxjzm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtcjsirtcm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtkmzrmhgs.html

[M04] 获取当前工作目录
来源：http://hz.zhiwuduotai.top/gtpwfmzzlq.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gtelxqzpmm.html

PHP:  getcwd();
来源：http://hz.fengsongda.top/gtifrzrhag.html

JS:   process.cwd()
来源：http://hz.daxiang520.top/gtyfedyxnx.html

TS:   process.cwd()
来源：http://hz.gaohongyu789.top/gtjhhoclbc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.pycfn.com/gtmbwsqdkk.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtkjgtbgfr.html

Ruby: Dir.pwd
来源：http://hz.vqdsnc.cn/gtjdtrrfnq.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yvedp.cn/gtuiwvmxze.html

[M05] 设置退出码
来源：http://hz.zhixingplan.top/gtzvgdyyxy.html

Py:   sys.exit(1)
来源：http://hz.gzhubu.top/gtvxwiggsa.html

PHP:  exit(1);
来源：http://hz.bjfxy.top/gtqqwcrzyk.html

JS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtqzjttgqf.html

TS:   process.exit(1)
来源：http://hz.chenlongwang.top/gtakqiyayu.html

Java: System.exit(1)
来源：http://hz.hysaishi.cn/gtvlwfobqy.html

Go:   os.Exit(1)
来源：http://hz.ybcxt.top/gttqeqzxij.html

Ruby: exit 1
来源：http://hz.ywan-chungtsiang.top/gtgrkmnpac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnqzz.top/gtafkirnmc.html

[M06] 向标准错误输出
来源：http://hz.pycfn.com/gtgbontwkz.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtoeswwgln.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jqgfzy.top/gtyzdcktop.html

JS:   console.error("err")
来源：http://hz.ybcxt.top/gtnbuzxcwb.html

TS:   console.error("err")
来源：http://hz.chenjidiqi.icu/gtfoyjicnv.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtujhxfgzg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xingfuxueyuan.xyz/gttiqxydle.html

Ruby: warn "err"
来源：http://hz.hammf.cn/gtvbxyrjba.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuanzx.com/gtaojjozmj.html

[M07] 判断是否为主入口
来源：http://hz.ywan-chungtsiang.top/gtdgglmbxo.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtldgtjzbv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aizwys.cn/gtfztnpvub.html

JS:   require.main === module
来源：http://hz.nwbrower.top/gtigvxsuxd.html

TS:   require.main === module
来源：http://hz.hfpthk.cn/gtoybdeyyf.html

Java: public static void main(String[] args)
来源：http://hz.0kj1m.cn/gtietbngpu.html

Go:   func main()
来源：http://hz.jianghu66.top/gthncjeubn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.52xcode.cn/gttfhydprc.html

C#:   static void Main(string[] args)
来源：http://hz.aibaodan.cn/gtfqxnpmur.html

[M08] 获取系统与运行时信息
来源：http://hz.quarkkingdee.top/gtffedrbdg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinyuanbaomall.cn/gtvbmmbjuf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yonumen.top/gtiqebpbfi.html

JS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtwobtsrpm.html

TS:   process.platform;  process.version
来源：http://hz.zhongyouzk.top/gtoscgorug.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenlongwang.top/gtfmacgdvw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jianghu66.top/gtusuftfxz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtttbfbwnz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xylfe.cn/gtszmrdixm.html

================================================================================
来源：http://hz.cashguo.top/gtmoxlogad.html

N. 数据结构与算法
来源：http://hz.sxryk.cn/gtgqbmatbq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthpitmijp.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtplnznxlc.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.daxiang520.top/gtflohbxzy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.nanxuanxn.top/gtqozxysjg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.tian-w.cn/gtmpvccsrz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtioyonxzi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhixingplan.top/gtusykyrlr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.aizwys.cn/gtciukivsj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.hongshengwenyu.top/gtwtxdqpmj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtdnuckvlz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.yj20258888.top/gtgraosobb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gttpaxrqgs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yongpay.top/gtuklkdlpf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shzxlz.cn/gtktfidzwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtaenlljvb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhijiandao.cn/gtbizwmhih.html

Go:   slices.Sort(arr)
来源：http://hz.fzhhl.top/gtjspxcepu.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtxshexbnr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yueranfly.top/gtsdwqkgmx.html

[N03] 快速排序（分治示例）
来源：http://hz.0kj1m.cn/gtawceiabe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtxuutjqts.html

PHP:  // 递归实现，或用 usort
来源：http://hz.wangdashe.top/gtqqmxzmsc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xylfe.cn/gtowhroqyo.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.jinqigfzy.top/gtymvhynuz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yangfankeji.com/gtxpwvaweq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtjfxxxikb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.smart0.xyz/gtzekdlyte.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhiwuduotai.top/gtosnulvci.html

[N04] 斐波那契数列
来源：http://hz.yj20258888.top/gtgfhvxvit.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhoulong.xyz/gtluinplru.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.sweek.top/gtendiqnym.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtbquxirwx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cqqwz.cn/gtbefkfgtb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jianghu66.top/gtcycfjkfc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangdashe.top/gtjhadmmne.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj202588.top/gtackuzczz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.chenlongwang.top/gtwgtmwmvm.html

[N05] 最大公约数
来源：http://hz.nanxuanxn.top/gtghgrfekb.html

Py:   math.gcd(a, b)
来源：http://hz.ydjk.org.cn/gtuubcrcar.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtfkjdhyvu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sweek.top/gtgauimjuh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ydzc1.top/gtqwhoekvs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.quarkkingdee.top/gtndbtvxfo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zycfv.cn/gteaauvpdj.html

Ruby: a.gcd(b)
来源：http://hz.jyoumei.cn/gtkdyfhqse.html


<!-- 参考信息 -->