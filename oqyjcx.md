代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtvmvfsvnb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtszrqlfiv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtlqzrwkum.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtlpptwmtf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtunkbexsf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gttrztpecq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtgvwzfynu.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtdcryqqlw.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtwlvbwwqi.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtstrhhnnp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jyoumei.cn/gtbyrtfdpc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtlqekamuy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtyrrdrdcv.html

Go:   end.Sub(start).Hours()
来源：http://hz.gaohongyu789.top/gteyhmbfor.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gthxmwczgu.html

C#:   (end - start).TotalSeconds
来源：http://hz.ivvv.top/gtcwwclibq.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtvqkuorli.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gthlbnadte.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gterwnsjga.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtlsuhpqth.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtsqqzqdtz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guannengcc.top/gtkblzpdgj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtcdnaoakv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtziozgmtn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtivptcreg.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtdgkbxtae.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtktlvxmye.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shuidangran.top/gtffykpzbf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtefynlysf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yonumen.top/gtnyiwgbrs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shuidangran.top/gtjppziibr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtourxiwmm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhijiandao.cn/gtjxcwzuea.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtuibcuffv.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtvuojiapg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtoshcykia.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtpqorybyh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtwqlogmwb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtrcxbafht.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.quarkkingdee.top/gtgejqyzwe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtahthyrnv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtvmjfvyds.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtpnzbtqsa.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtdhpoycxp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtrvyomhhd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtnnzqxtar.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtsyvdueab.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.kuanghao11.cn/gteannbing.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gttovudrgp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtwdfsqeib.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtchthlgbz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gttoidtjlh.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkageiany.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtsrbptaqf.html

================================================================================
来源：http://hz.zhengqikj.top/gtncxmtpqu.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtdwjwcpkw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtnugzqzoc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtokyfkuqs.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtvdbhhvvt.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtfrcwclib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhoulong.xyz/gtggakiauz.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtvokgylws.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtczelkzmo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtggxaprpu.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gtezfxctug.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtzwjtvjft.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ehwqpu.com/gtawemrdsf.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtroozyxbj.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtdxfdxxhg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtqkrpytun.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtgduqnfay.html

Ruby: JSON.parse(s)
来源：http://hz.guannengcc.top/gtxtuuxlvt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtblgrwwko.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtuhplevbr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtupcujeqy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtvtyqgavn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtjsapljyp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtwsacttmy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.andypj.xyz/gtwhybocsp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtofagidez.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cqqwz.cn/gtjgchvfrf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.birdmap.top/gtusvrrvnv.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtgtecxyew.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtxuyokgpe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnqzz.top/gtxypibafl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtjfymampd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtvmjsotti.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtoevqaxhe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtwfjjwowq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtisroerpp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtqetrgrkg.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtalzvjeyo.html

Py:   copy.deepcopy(obj)
来源：http://hz.jyoumei.cn/gtbaonzqcz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydjk.org.cn/gtklhgxrdq.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtzwfxgoad.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtkeymepke.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxuanxn.top/gtkopvuqej.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yangfankeji.com/gttlrjphvc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtocsgxmmj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtbiyijqjg.html

[K06] 解析 URL 查询串
来源：http://hz.guowangkeji.top/gtndnxkfwr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gthmihkdgf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sufxvd.cn/gtudriolgf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtqzeedzki.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtydmzxrxv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.dashuyun.cn/gtogzrohrc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtlzhdoldg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cdnleiting.top/gtbaliwkmi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtrlcscgxf.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtvawpntrx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtgjtfbpde.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhixingplan.top/gtqngeqjqm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtqkxrstkl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtrsmciwgl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtqbpdczwb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtpdjuhxho.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tianlin.xyz/gteloehcxo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtkokhlnwl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtxzmzsjkt.html

Py:   pickle.dumps(obj)
来源：http://hz.zhiwuduotai.top/gtazgbrtak.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nanxinkj.top/gtackpaqjx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtugglvtly.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtqukfkcqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sxryk.cn/gtzmoivghj.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtencdanhn.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenlongwang.top/gthcftrwrg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtranjvjyb.html

================================================================================
来源：http://hz.shuidangran.top/gtufshgvuj.html

L. 网络请求
来源：http://hz.xuetiantiany.cn/gtkybhkxei.html

================================================================================
来源：http://hz.316326.xyz/gtfxpzirei.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtirwvgcdl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hammf.cn/gtajbsuueg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtxlhlmico.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtjzkuiozz.html

TS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtdhyfpatz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtqfjvtqrz.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtetirwram.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtcvlrxufb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daxiang520.top/gtntgplshe.html

[L02] 发送 POST JSON
来源：http://hz.ybcxt.top/gtyhrjtdtm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtjrifzfor.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.guowangkeji.top/gtqvslebry.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtululcszz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtljikzvkj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtxjklztuw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shanyushiyangkeji.top/gtsypdaral.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yj202588.top/gtmznrgwlq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtijqigbua.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtcshlkahe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ivvv.top/gtcegiezoh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ywan-chungtsiang.top/gtdsbculss.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtsoryhcqx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sufxvd.cn/gtnyxealiz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtgpamuqwt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hammf.cn/gtxgdolaoc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhaomingkeji.xyz/gtwtxcwfqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtezogkjba.html

[L04] 设置超时
来源：http://hz.ehwqpu.com/gtwsmvdiup.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtmroscthk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xylfe.cn/gtgaeikwil.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtsmqdlerk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.snrcjt.cn/gtsdgruyle.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtntwengdp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gtmdfkspbu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hongshengwenyu.top/gtlffdxcpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gtuyzwdixz.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtshtkzccy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yongpay.top/gtkegvptea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj20258888.top/gtqnwmuldh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtprbfgnvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtzbvrghms.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgufenzy.top/gtqusvjwyx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtaesdnvjj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yj202588.top/gtiabdznbt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtmhceglbb.html

[L06] 解析响应为 JSON
来源：http://hz.ydzc1.top/gtdvcmquiw.html

Py:   resp.json()
来源：http://hz.wangshuangyany.cn/gtjhharnan.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtnrdeakwr.html

JS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtjxobxscr.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gtjhobkmyl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtxnvmnhut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.daxiang520.top/gtyunlicfi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtiebxllgl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.feifeiyinyue.top/gtcxlbzpal.html

[L07] 处理 HTTP 状态码
来源：http://hz.aizwys.cn/gtogndouox.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gthiowtaho.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtnugvevki.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtsjgghywu.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtcslvytdn.html

Java: resp.statusCode()
来源：http://hz.ywan-chungtsiang.top/gtelyvutjr.html

Go:   resp.StatusCode
来源：http://hz.vqdsnc.cn/gtudrnkdpv.html

Ruby: resp.code.to_i
来源：http://hz.quarkkingdee.top/gtzpropzrm.html

C#:   (int)resp.StatusCode
来源：http://hz.jinghuilouyu.cn/gtubqsjtqj.html

[L08] 并发请求多个地址
来源：http://hz.zdqjudy.top/gtmuaglxtr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtivxovmhg.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtpajbvahg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtaljxhmib.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhengqikj.top/gtshmdkltl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gtdzvegruj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hfpthk.cn/gtytxogknm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.sxryk.cn/gtbmqnvkbv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ydjk.org.cn/gtoxguhgoo.html

================================================================================
来源：http://hz.birdmap.top/gtbkgywcgd.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtwwfptoig.html

================================================================================
来源：http://hz.kuanghao11.cn/gtccjuhzai.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtoncikahy.html

Py:   sys.argv[1:]
来源：http://hz.pycfn.com/gtnqtygypp.html

PHP:  $argv;  $argc;
来源：http://hz.bjfxy.top/gthzguznrw.html

JS:   process.argv.slice(2)
来源：http://hz.iojbl.cn/gtxueoxwyb.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtqbhndzqa.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtmwqtxqpc.html

Go:   os.Args[1:]
来源：http://hz.andypj.xyz/gtmniwdqge.html

Ruby: ARGV
来源：http://hz.cheryme.top/gtdfkkczdp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtdwcaxnbg.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtizbodgvc.html

Py:   os.environ.get("HOME")
来源：http://hz.quarkkingdee.top/gtuyeddgbn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xuetiantiany.cn/gtyttaiihn.html

JS:   process.env.HOME
来源：http://hz.nwbrower.top/gtrzgsaguc.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtbmxjjeff.html

Java: System.getenv("HOME")
来源：http://hz.pycfn.com/gtltdnhpvz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtomyoroyu.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtxpdgussg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.quarkkingdee.top/gtajqamfzv.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gttnzrwwtp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.daxiang520.top/gtuspfwhvq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinghuilouyu.cn/gtpvjkopup.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gtedfosdvh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.sufxvd.cn/gtrojwawlw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gtdoazpvjl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.dashuyun.cn/gtiojmvuag.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hammf.cn/gtditnundw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xingfuxueyuan.xyz/gtvgwnogbl.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtfmlsiidt.html

Py:   os.getcwd()
来源：http://hz.chenjidiqi.icu/gtmyyvhcoa.html

PHP:  getcwd();
来源：http://hz.hysaishi.cn/gtlrwauyhs.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtjzmjuzot.html

TS:   process.cwd()
来源：http://hz.mhx1999.top/gtuodtdjwu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtivhvnrae.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtdfxelkvx.html

Ruby: Dir.pwd
来源：http://hz.jqgfzy.top/gtevqcvtnp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.tanke756.top/gtliwpmoxx.html

[M05] 设置退出码
来源：http://hz.ybcxt.top/gtakhtqsqn.html

Py:   sys.exit(1)
来源：http://hz.sweek.top/gtnwzqqcyz.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtpbfaxhbq.html

JS:   process.exit(1)
来源：http://hz.shuidangran.top/gtmexjfcjy.html

TS:   process.exit(1)
来源：http://hz.0kj1m.cn/gtqmwfclma.html

Java: System.exit(1)
来源：http://hz.pengpengdd.cyou/gtzouapopo.html

Go:   os.Exit(1)
来源：http://hz.shzxlz.cn/gtimgvxhjw.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtjnumozmk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hnxiangtu.top/gtrmspwzub.html

[M06] 向标准错误输出
来源：http://hz.zhoulong.xyz/gtkobebksw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtfscavpwm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.mhx1999.top/gtmulqoviv.html

JS:   console.error("err")
来源：http://hz.jiagoushi.top/gttzghkjqb.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtwigjeqib.html

Java: System.err.println("err")
来源：http://hz.fzhhl.top/gtkgxknubs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.andypj.xyz/gtpdlnumtm.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtcnqhowei.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.vqdsnc.cn/gthbakxeza.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtpwdibumy.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gtilpqaich.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gthtforzby.html

JS:   require.main === module
来源：http://hz.yuanzhike.top/gteiksxokp.html

TS:   require.main === module
来源：http://hz.yanxiufei.cn/gtjphqbfvu.html

Java: public static void main(String[] args)
来源：http://hz.316326.xyz/gtmwrcaczn.html

Go:   func main()
来源：http://hz.yj20258888.top/gtsldqfflr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtnnpxenrw.html

C#:   static void Main(string[] args)
来源：http://hz.cucudq.cn/gttpxqkbib.html

[M08] 获取系统与运行时信息
来源：http://hz.xinyue.icu/gtmjvixjgq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yangfankeji.com/gtddglbxjk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.aizwys.cn/gtvqnamgxv.html

JS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtxcxroztm.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtoryehjuw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sysykeji.top/gtxbrcfkye.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtecjjwezc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtmiutbgjs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.gzhubu.top/gtmboxmpdk.html

================================================================================
来源：http://hz.hywenlv.cn/gtzxspiobc.html

N. 数据结构与算法
来源：http://hz.smart0.xyz/gtimapgnor.html

================================================================================
来源：http://hz.hywenlv.cn/gtrwwpqkka.html

[N01] 二分查找（有序数组）
来源：http://hz.chenjidiqi.icu/gtrzksmloj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ybcxt.top/gtubicqkyv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.fzhhl.top/gtzdhjnsgg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zdqjudy.top/gtygurhhop.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtmqyxksdl.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.c1oappe.top/gtfxtnmcfd.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.kuanghao11.cn/gtuicgpjra.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yanxiufei.cn/gtpmycavrz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.guannengcc.top/gtbypkeoew.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.haohaochexian.top/gtatdyvunf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtvydnuywv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.wangshuangyany.cn/gtonwilzac.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gttqadgcru.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gtcdaslxfa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sweek.top/gtubbopjom.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtetuhuftn.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtkkzscsxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.zhiwuduotai.top/gtggnenwva.html

[N03] 快速排序（分治示例）
来源：http://hz.cdnleiting.top/gtqvccswnt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnqzz.top/gtxlaqnzrc.html


<!-- 参考信息 -->