代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtbebrrevc.html

[J08] 提取年月日与星期
来源：http://hz.gogol.net.cn/gtwbhrvyqt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtaplgrbxw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtofeufvfe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gthxkcvkje.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hysaishi.cn/gtfrdzlehw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtonuacigo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtcormbwqg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtgcoamhyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtlqpoduay.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtgncfbezz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hongshengwenyu.top/gtwnrxzesg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtwaxvoalc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtwaxedczx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gttvxhgimo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtriwievwa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtjwrcczzg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtwwuemlkq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtrnrktcsi.html

[J10] 取今天 / 本月第一天
来源：http://hz.havefunace.top/gtmgpmuwrx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gttyuqortq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fengsongda.top/gtwtmyzjzd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jyoumei.cn/gtanuqfilh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tianlin.xyz/gtoxndcafa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtxhtfqmep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sxryk.cn/gtfpadnphn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtmnmtmrun.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtmdsbkawq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtlicubdop.html

K. JSON 与序列化
来源：http://hz.yuxming.cn/gtbqzgfvje.html

================================================================================
来源：http://hz.jiagoushi.top/gtmsovrway.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtvaethcwl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtbbbkfxfa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtqtwxrcvg.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtvxlfsjql.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtfgwnjqgp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.mhx1999.top/gtzgqtmntp.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtnelarmxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.snrcjt.cn/gtpedodrkj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhijiandao.cn/gtyrqwgumt.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtrdhhosok.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtujbkezri.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtbpzvwwfc.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtfhutilmc.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtbcujlqor.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xziqi.cn/gtazajdtal.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtlzwukprm.html

Ruby: JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtgvlvfjll.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtdjzcodye.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtwebfvcaj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gttyjgknda.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtznhtfymb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtrqyuuzgi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtfxrjodxk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gtgmunkvtn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtishayjnj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtozizmtby.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtcjupmucm.html

[K04] 读取 JSON 文件
来源：http://hz.smart0.xyz/gtikzjpmnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.smart0.xyz/gtsnlmfqby.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtjmtkfzku.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtgsnmnsno.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtrtnqiuss.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zycfv.cn/gtcelhgghd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtntqlisqd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtpscnibpc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangshuangyany.cn/gtnzlkgfuz.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtknasyuof.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gttwkexkdg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtpvyhvtob.html

JS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtpnilaeje.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtcgmmchic.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtbfnpbxin.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtliekpdwh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.fengsongda.top/gtdwzgwbbm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.birdmap.top/gtaktlcqns.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gtwxdfpuou.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtmugrcogp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtvoigodws.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtpxrpkhhq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtbfqdgdnd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gtzfqhfsby.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtjgluznkk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shzxlz.cn/gtnugrxkvb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtabljrffr.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtbthtcwnz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtwtpwbcqj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnqzz.top/gtefovyfio.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtfnpdzrej.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtvxcanttq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtwtjwcpue.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj202588.top/gtgnufcobj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gtpxhkyult.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtbziyudmw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtvydsiuil.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gtorfeytio.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtndjgummm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtgfdpqkir.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgufenzy.top/gtwdpmpuaj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jqgufenzy.top/gtcrzsaquk.html

Go:   encoding/gob
来源：http://hz.9152youxi.cn/gtzrzrslqu.html

Ruby: Marshal.dump(obj)
来源：http://hz.meibo888.top/gtedogaaly.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtxxvyanhs.html

================================================================================
来源：http://hz.yonumen.top/gtlxznbxvq.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtmczmedzd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcjdvxnyt.html

[L01] 发送 GET 请求
来源：http://hz.hysaishi.cn/gtvwqrvzca.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhijiandao.cn/gtlrbrrvnh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtrlbzzytl.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtdyqacwts.html

TS:   await fetch(url)
来源：http://hz.hnxiangtu.top/gtkvcfpjat.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.vqdsnc.cn/gtluiozwfe.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gthmiflnuw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtcjxiiwud.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtklmulxct.html

[L02] 发送 POST JSON
来源：http://hz.meibo888.top/gtftampsqm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtxzejsopl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtmjymusji.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tian-w.cn/gtktqdwqci.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtkvclczmi.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtsgupygah.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xuanzx.com/gtelbtiwjl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yueranfly.top/gttxaftfkc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.iojbl.cn/gttnivdbgq.html

[L03] 设置自定义请求头
来源：http://hz.zhixingplan.top/gtqmbjnhyu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gzhubu.top/gtjqriomdy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gttgybbian.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtufaolsez.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtkzehsmlb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtclvigkvk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.haohaochexian.top/gtcjokuswq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtyaojmvfp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yvedp.cn/gtbffjaxss.html

[L04] 设置超时
来源：http://hz.yuxming.cn/gtmxmwnaga.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sysykeji.top/gtcgauwdzu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtkyvnkzes.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtvtoinelv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtyxusbojo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnqzz.top/gthklpdfbq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xinyue.icu/gtxpubhepv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.smart0.xyz/gtsvrgnisr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yonumen.top/gtwzwaocop.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtikvaicbz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtlbnjnxuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258888.top/gtoficocvv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gttvddexrl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gttpvkgvwh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnxiangtu.top/gtdapsncvu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.316326.xyz/gtxpunioln.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtvwjgvwdn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtdqucluda.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtpvqfavjj.html

Py:   resp.json()
来源：http://hz.meibo888.top/gtvngxfgrd.html

PHP:  json_decode($body, true);
来源：http://hz.xingfuxueyuan.xyz/gtehnlkbhk.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtgamcmvsp.html

TS:   await resp.json()
来源：http://hz.andypj.xyz/gthyhwrhhe.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.tian-w.cn/gtsrvfmasg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtvpoxrykg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtmnqpfbrh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtjzkcybeq.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtpmoczhsl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtsztthcad.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gtrqoxivxi.html

JS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtprxzfdlw.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtymcmaqrc.html

Java: resp.statusCode()
来源：http://hz.redwolf501.top/gtxhvbxota.html

Go:   resp.StatusCode
来源：http://hz.nwbrower.top/gtzbizddbr.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtqgxhbwih.html

C#:   (int)resp.StatusCode
来源：http://hz.ydzc1.top/gtfndkdjyz.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtoxcrlcur.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cqqwz.cn/gtdtqdhjes.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtgtrkynle.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtmyjduluw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtliekdsoe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtrnaxzazg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtqafbdpan.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.gaohongyu789.top/gtibzrtmeo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gtbnvclvlg.html

================================================================================
来源：http://hz.hfpthk.cn/gtxnchnshr.html

M. 命令行 / 进程 / 环境
来源：http://hz.sxryk.cn/gtzfhfuknz.html

================================================================================
来源：http://hz.jqgufenzy.top/gtkapsoeob.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtbwtjuaij.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtwvzquhgs.html

PHP:  $argv;  $argc;
来源：http://hz.iojbl.cn/gtitchmnkq.html

JS:   process.argv.slice(2)
来源：http://hz.jqgfzy.top/gtsnvblrlf.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtftfcjowx.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtcgturwda.html

Go:   os.Args[1:]
来源：http://hz.hnxiangtu.top/gtjyhutgmt.html

Ruby: ARGV
来源：http://hz.jqgufenzy.top/gtxnzdrkif.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cqqwz.cn/gtejyeotji.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtoirfwdgp.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtbnsmifst.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hammf.cn/gtxvfpzdoj.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtmxcpwkkk.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gthmnjrjxz.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtphavagud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xuetiantiany.cn/gthhyvbvyw.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtstchuybg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sxryk.cn/gtjsmueymk.html

[M03] 执行外部命令
来源：http://hz.ehwqpu.com/gtikhangzu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ehwqpu.com/gtoqdvtbxa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtetwitmzu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtwlpcerxs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtoqnglgxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhoulong.xyz/gthygtnwpe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydjk.org.cn/gtnpgiadfr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ybcxt.top/gtwkwoawne.html

C#:   Process.Start("ls", "-l");
来源：http://hz.fzhhl.top/gtuorgplll.html

[M04] 获取当前工作目录
来源：http://hz.c1oappe.top/gtykhenrtq.html

Py:   os.getcwd()
来源：http://hz.shangyingyoupin.top/gtrtzabzaz.html

PHP:  getcwd();
来源：http://hz.hnxiangtu.top/gtrgaivlnq.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtqctdjnoo.html

TS:   process.cwd()
来源：http://hz.yongpay.top/gtwphrfama.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtkjlcwdoq.html

Go:   os.Getwd()
来源：http://hz.jiagoushi.top/gtfenpznbp.html

Ruby: Dir.pwd
来源：http://hz.hongshengwenyu.top/gtlskqbtxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.smart0.xyz/gtxtflcjjj.html

[M05] 设置退出码
来源：http://hz.shanyushiyangkeji.top/gtuomawbhi.html

Py:   sys.exit(1)
来源：http://hz.chenzaomai.com/gtdgjrhyte.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtrotkamct.html

JS:   process.exit(1)
来源：http://hz.shzxlz.cn/gtpevgehxx.html

TS:   process.exit(1)
来源：http://hz.yj20258.top/gtlertwpgb.html

Java: System.exit(1)
来源：http://hz.9152youxi.cn/gtgoncltwj.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gttnpfzpay.html

Ruby: exit 1
来源：http://hz.52xcode.cn/gtsjhoijix.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtuizmptgj.html

[M06] 向标准错误输出
来源：http://hz.mhx1999.top/gtsmtvfhnq.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtmrbdeufc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.9152youxi.cn/gtwzkcsfrd.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtecsruple.html

TS:   console.error("err")
来源：http://hz.cqqwz.cn/gtkzbhdnog.html

Java: System.err.println("err")
来源：http://hz.shangyingyoupin.top/gtgkopnjal.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yueranfly.top/gtpmkzspms.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gtdkigddiq.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinyuanbaomall.cn/gtblhbnnjm.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gttaplyvsi.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtbjwexgxr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.daria6918.cn/gtetzkbity.html

JS:   require.main === module
来源：http://hz.yanxiufei.cn/gtcxbirjmt.html

TS:   require.main === module
来源：http://hz.bjfxy.top/gtffyboeag.html

Java: public static void main(String[] args)
来源：http://hz.ybcxt.top/gtmkznrxcj.html

Go:   func main()
来源：http://hz.tian-w.cn/gtupmhcglb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydzc1.top/gtdnlypewn.html

C#:   static void Main(string[] args)
来源：http://hz.jyoumei.cn/gtvfbbnfpa.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtqspgdvqe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhaomingkeji.xyz/gtspnxdmma.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daria6918.cn/gtvcjrtxeo.html

JS:   process.platform;  process.version
来源：http://hz.havefunace.top/gtouennzmu.html

TS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtlvfeqxqj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuanzx.com/gtshnehovb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258.top/gtwvcuyxek.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jyoumei.cn/gtphejskkp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hongshengwenyu.top/gteqgbvkdb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtezwgvxhd.html

N. 数据结构与算法
来源：http://hz.sysykeji.top/gttkmamrdf.html

================================================================================
来源：http://hz.gaohongyu789.top/gtxnvpnuox.html

[N01] 二分查找（有序数组）
来源：http://hz.jianghu66.top/gtcviovwvx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj20258.top/gtncbvxkxt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtrkobrovd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.iojbl.cn/gtpekyobck.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtxzbkmetv.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhiwuduotai.top/gtipnlwleo.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.iojbl.cn/gtowivhprv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gttgbqpsjp.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.gotoacloud.top/gtreqqqeqc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtaqfuduoa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtmnxzjtow.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yueranfly.top/gtqvcrztlm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gthamliifh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.haohaochexian.top/gtotjhnlla.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.xziqi.cn/gtruwrfvvb.html

Go:   slices.Sort(arr)
来源：http://hz.yj202588.top/gtijqdojcv.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtphmbygzl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jinqigufen.top/gtrbhhsxds.html

[N03] 快速排序（分治示例）
来源：http://hz.hnqzz.top/gtdxqstkcj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.tanke756.top/gtdzfnhpec.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shzxlz.cn/gtvrgjzudb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hammf.cn/gthgjphjua.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtmmlxxmco.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtakjddzmx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.xinyue.icu/gtqjyfegsg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ehwqpu.com/gtszzwvjcp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.mhx1999.top/gtjtjwxqsi.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtezzngkup.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.gotoacloud.top/gtcfwozfiu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.shuidangran.top/gtdmaguthu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gttowyvvcf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yangfankeji.com/gtsgbaiazs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.quarkkingdee.top/gtmagtuuee.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtrbnpzqow.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hfpthk.cn/gtmmjxmubi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.birdmap.top/gttjpbrflk.html

[N05] 最大公约数
来源：http://hz.yvedp.cn/gtoqkxcqta.html

Py:   math.gcd(a, b)
来源：http://hz.svipenyu.cn/gtbdfjzcho.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtgfjpemog.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shangyingyoupin.top/gtuuvevkds.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.aizwys.cn/gthunmntdj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.smart0.xyz/gtbcfnexzc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.dashuyun.cn/gtufxpcqrh.html

Ruby: a.gcd(b)
来源：http://hz.aibaodan.cn/gtpjdpspxf.html


<!-- 参考信息 -->