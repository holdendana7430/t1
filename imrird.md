代发 wailian999

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtxjrpejze.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtbcxogjve.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtkaekbmbe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtcyklbbdi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtaihepzdp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtskyjzbzk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cucudq.cn/gtltjybnbl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtcmplqdtd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtusapsmzo.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtyzdewhuj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtxrtxlaiu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtjzvxejpl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gthevrjbld.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zdqjudy.top/gtnfjbbzwy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtsgllhbwc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtxrxncctz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xylfe.cn/gtxgdzksgs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gthyfkhkft.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtkjzzinea.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtwaepcdhn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtustskrgt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtjduhgjjo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtmyxkawei.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtcnlzpiop.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtxyjeyjax.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuanzx.com/gtcieqhpft.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yvedp.cn/gtduibimyx.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtjxauzzax.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtqnczymdc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuxming.cn/gtiygnebnr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtnvqraane.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtuxdlmqyb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtcgdpdnte.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtonwsixge.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtlslvxswq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtojkkgqdp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtirewoslr.html

K. JSON 与序列化
来源：http://hz.chenlongwang.top/gtzzroniul.html

================================================================================
来源：http://hz.haohaochexian.top/gtambhizjz.html

[K01] 对象转 JSON 字符串
来源：http://hz.jiagoushi.top/gtrajherpq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtdhkexfeh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtzhqgxzro.html

JS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtmmlvlnzd.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtekxbfokw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtweftjjko.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtusbgvtpv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtvmqlryxv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jlsjyb.cn/gtrndzyhga.html

[K02] JSON 字符串转对象
来源：http://hz.ydzc1.top/gtxhdwshvl.html

Py:   json.loads(s)
来源：http://hz.hywenlv.cn/gtnapffqjo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinyuanbaomall.cn/gtwamakmls.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtjjfvqjow.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gttrxdbjxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtqlioatyk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtfcpjncsb.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtwcydwaqq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtdorahbsg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtgtlglbye.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtvrvscmbc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtyyvsxlxj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtenwtxeuj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtvcqtaqwd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtdymxqdqg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.0kj1m.cn/gtoeolwiyl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtvipbzmhg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtbwwxeect.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtqmpblxqe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhongyouzk.top/gtptatdmgi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guowangkeji.top/gtiedikmpe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtihhpaaju.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtmhbtqtqj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtkctcdrdv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtdxaaocga.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtbargxowq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtmdxtswpu.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gttdkchzwp.html

Py:   copy.deepcopy(obj)
来源：http://hz.gzhubu.top/gtjdoianrl.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sysykeji.top/gtiptftdif.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtdtvcjaok.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gthefrbull.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gtnwblgyjy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gtunjlvfok.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtkhlhnnxz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zdqjudy.top/gtkqtljmmn.html

[K06] 解析 URL 查询串
来源：http://hz.yvedp.cn/gtobfxxzuz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hywenlv.cn/gtkrkbvodr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnqzz.top/gtjcymtllo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtcuwedrzz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtwsavctfw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtgxoscnxb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtjjuhobpc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtaogjeakp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtyvjopqap.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtuvrmjajl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yangfankeji.com/gtykkxpzxy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xuanzx.com/gtyqekobzv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtsfkwfycj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtytmzjrbl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtjqiktwvw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ppjwa.cn/gtycsidfac.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gtjniyvlcr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtnnwcafde.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnxiangtu.top/gtzsjbjbux.html

Py:   pickle.dumps(obj)
来源：http://hz.gzhubu.top/gtzkukhbtg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtlbsjmulz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtdxcvrbnn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtvatkbfju.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.wangshuangyany.cn/gtccajiloa.html

Go:   encoding/gob
来源：http://hz.xuetiantiany.cn/gtmvaahqbj.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtowuwaosz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtkgcympqs.html

================================================================================
来源：http://hz.snrcjt.cn/gtrhpabeuv.html

L. 网络请求
来源：http://hz.shzxlz.cn/gtkvbbypjp.html

================================================================================
来源：http://hz.quarkkingdee.top/gttztrnkrc.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtvmksrooz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtwbavgtnv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtahjyegqz.html

JS:   await fetch(url)
来源：http://hz.yuanzhike.top/gtihulqapa.html

TS:   await fetch(url)
来源：http://hz.hnqzz.top/gtyvzjrcjb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.iojbl.cn/gtywoedjzx.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhaomingkeji.xyz/gtjgtkhgka.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtzsctgqyz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cqqwz.cn/gtwiuvmbhv.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gthwuygygr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtkxemfqjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtflwvltsi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtaursfzon.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtkbfevqgn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gtwxnmsqmi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtzvwpuplz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sweek.top/gtbbpkbsrz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtdpmwqgmt.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtwtdhstoa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtthjjbnzb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hywenlv.cn/gtsbwzjzfj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.haohaochexian.top/gtbbcvyrma.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtjbzdqpon.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gthbugujhr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ybcxt.top/gthxjzgbbh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ywan-chungtsiang.top/gtiyifldcd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtwiaukycm.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtglynwmft.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hnqzz.top/gtbywipuww.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fengsongda.top/gtshxysbxh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtqstfaiyf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtjhpobtdr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.bjfxy.top/gtmmhthxzt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yonumen.top/gtrhojoedq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tanke756.top/gtduaowxgl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yj20258888.top/gtisinoopn.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gttqdgosnq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yueranfly.top/gtprqlcroj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtgqncmfjc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtimuenzdi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtvzwjixwd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtbscraagp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ppjwa.cn/gtzsuyblyi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydzc1.top/gtjpxxhrrv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.quarkkingdee.top/gtzcnrvdqt.html

[L06] 解析响应为 JSON
来源：http://hz.ywan-chungtsiang.top/gtusxpistm.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtucphbbuo.html

PHP:  json_decode($body, true);
来源：http://hz.pengpengdd.cyou/gtbqftgdye.html

JS:   await resp.json()
来源：http://hz.zhixingplan.top/gtpjzaiqmg.html

TS:   await resp.json()
来源：http://hz.vqdsnc.cn/gtxpjmhdab.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hysaishi.cn/gtejdurnrq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zdqjudy.top/gtkgmocrqj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtjbnfghgk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.iojbl.cn/gtvvbmvbln.html

[L07] 处理 HTTP 状态码
来源：http://hz.jianghu66.top/gtrmhgvdzo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258.top/gtapvqixbk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtifsrucxm.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtvkvivndt.html

TS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtsfwkhslv.html

Java: resp.statusCode()
来源：http://hz.yueranfly.top/gtyabcihdm.html

Go:   resp.StatusCode
来源：http://hz.quarkkingdee.top/gtwzdkcmxq.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtuaymzpmz.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtpxyusgww.html

[L08] 并发请求多个地址
来源：http://hz.yvedp.cn/gtxvyisyyf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtrryrdezx.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtlthoocdl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtdamskmyl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtjqvtafjq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ivvv.top/gtqwrklaic.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gtwarwhjdt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtmmxaicwn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yonumen.top/gtwozjoskp.html

================================================================================
来源：http://hz.jiagoushi.top/gttkzvonme.html

M. 命令行 / 进程 / 环境
来源：http://hz.gaohongyu789.top/gtauhrardv.html

================================================================================
来源：http://hz.52xcode.cn/gtoxnoxoeu.html

[M01] 读取命令行参数
来源：http://hz.guowangkeji.top/gtneysxvsr.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtubarwvbn.html

PHP:  $argv;  $argc;
来源：http://hz.hammf.cn/gttqfjnadr.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtlgmrnrui.html

TS:   process.argv.slice(2)
来源：http://hz.quarkkingdee.top/gthgrdyiar.html

Java: args 数组（main 方法参数）
来源：http://hz.shanyushiyangkeji.top/gtygyizckl.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtkgthlihm.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtxbiwzvud.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtujtkttdf.html

[M02] 读取环境变量
来源：http://hz.dashuyun.cn/gtdptlokog.html

Py:   os.environ.get("HOME")
来源：http://hz.birdmap.top/gtwprctubx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhiwuduotai.top/gtihghtyml.html

JS:   process.env.HOME
来源：http://hz.hysaishi.cn/gtrpmojqil.html

TS:   process.env.HOME
来源：http://hz.yj20258.top/gtghfausrj.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtvemhuggu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtxqmbrzid.html

Ruby: ENV["HOME"]
来源：http://hz.hnqzz.top/gthyltjegu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtazjkjmzl.html

[M03] 执行外部命令
来源：http://hz.xziqi.cn/gtwbzvpqgs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtihzrklmd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gaohongyu789.top/gtkrxtrqgb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtdmbwwmqv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtocsewqas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.kuanghao11.cn/gtfrvaecoj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigufen.top/gtdxolsxev.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgfzy.top/gtaggareha.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtzinmgjmb.html

[M04] 获取当前工作目录
来源：http://hz.shangyingyoupin.top/gtxgczjwit.html

Py:   os.getcwd()
来源：http://hz.vqdsnc.cn/gttmqviqim.html

PHP:  getcwd();
来源：http://hz.ydzc1.top/gtvmxprpdo.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtujgiodwi.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtpmhoqdsy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guannengcc.top/gtxwphxrkh.html

Go:   os.Getwd()
来源：http://hz.smart0.xyz/gtuwujjtgv.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtgheoyzqt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hongshengwenyu.top/gttobpltcy.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gtfpxhgqsn.html

Py:   sys.exit(1)
来源：http://hz.yueranfly.top/gtpoopdwda.html

PHP:  exit(1);
来源：http://hz.chenlongwang.top/gtmewvujqg.html

JS:   process.exit(1)
来源：http://hz.ydzc1.top/gtfgvngmll.html

TS:   process.exit(1)
来源：http://hz.yangfankeji.com/gtsdodglfg.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gtoukzsfst.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtmmpirsae.html

Ruby: exit 1
来源：http://hz.jianghu66.top/gtmcjecyak.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtsuivelug.html

[M06] 向标准错误输出
来源：http://hz.tian-w.cn/gtvdgqpelb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtsltcmcnv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yangfankeji.com/gtyumfapsf.html

JS:   console.error("err")
来源：http://hz.yongpay.top/gtsbovbhhi.html

TS:   console.error("err")
来源：http://hz.sysykeji.top/gttcxanecs.html

Java: System.err.println("err")
来源：http://hz.hywenlv.cn/gtnanihouw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.haohaochexian.top/gtsvkyjkqz.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtyuqrtmhh.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cdnleiting.top/gtkrrpfvcd.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtbbrrslwe.html

Py:   if __name__ == "__main__":
来源：http://hz.pengpengdd.cyou/gtsxepvnpn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shangyingyoupin.top/gtlhgpcjyp.html

JS:   require.main === module
来源：http://hz.gzhubu.top/gtdaxlkyeb.html

TS:   require.main === module
来源：http://hz.gaohongyu789.top/gtxgiabbhl.html

Java: public static void main(String[] args)
来源：http://hz.hfpthk.cn/gtkiimlfum.html

Go:   func main()
来源：http://hz.yongpay.top/gtqjinxvmy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gttatndygl.html

C#:   static void Main(string[] args)
来源：http://hz.zhijiandao.cn/gtqlhndoig.html

[M08] 获取系统与运行时信息
来源：http://hz.dianchejie.cn/gtjsdxsclc.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ywan-chungtsiang.top/gtdpdmxfpu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.fengsongda.top/gtgetjsdqq.html

JS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtnghkqzod.html

TS:   process.platform;  process.version
来源：http://hz.0kj1m.cn/gtqsfmosbi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtzavojjyx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cucudq.cn/gtpyxxzsyo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtbpkgxere.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ywan-chungtsiang.top/gtkkuofejb.html

================================================================================
来源：http://hz.xylfe.cn/gtlixgighr.html

N. 数据结构与算法
来源：http://hz.ivvv.top/gtfpavozrx.html

================================================================================
来源：http://hz.yuanzhike.top/gtzzcagfkd.html

[N01] 二分查找（有序数组）
来源：http://hz.gaohongyu789.top/gtedixzbsn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhongyouzk.top/gtleferaum.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.zhoulong.xyz/gtyuouojqt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.svipenyu.cn/gtbgtvnrmv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.aizwys.cn/gthvtdhkfq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.birdmap.top/gtidvgpanr.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinghuilouyu.cn/gtvgygaihp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jqgufenzy.top/gtweodlzxa.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.smart0.xyz/gtlkvueupq.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.wangdashe.top/gtfzczuiwp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gtolwrfxtj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yangfankeji.com/gtwufkivxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.dianchejie.cn/gtepympmhg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtkmvcwqpw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jinqigfzy.top/gtumrdgduy.html

Go:   slices.Sort(arr)
来源：http://hz.daria6918.cn/gtsatpsodc.html

Ruby: arr.sort
来源：http://hz.hongshengwenyu.top/gtjhbqbezs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.birdmap.top/gtisxtjtue.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtgdcaskpa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtaahzjdjk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhijiandao.cn/gtxcivllgo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ppjwa.cn/gtalaqippm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hnqzz.top/gtlstwghjf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gogol.net.cn/gtufxahvsc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.andypj.xyz/gtiqfygroy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.gotoacloud.top/gtwsbripgc.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhixingplan.top/gtcbpbnftr.html

[N04] 斐波那契数列
来源：http://hz.sweek.top/gtlwwogkpv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sysykeji.top/gtyajigqfy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.haohaochexian.top/gtdrqfibgg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtujtsqidk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hywenlv.cn/gtrtpfddgy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.dashuyun.cn/gtuisekkmh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.smart0.xyz/gtafqomyhw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.chenlongwang.top/gtaqfuiofr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.52xcode.cn/gtqykahdvr.html


<!-- 参考信息 -->