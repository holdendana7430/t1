代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtngxhptwa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gthamezuwu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtwkiikdqa.html

TS:   d.toISOString()
来源：http://hz.xuanzx.com/gtfzflomps.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtqugqmfgt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pycfn.com/gttunkakye.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtpzmjbhfr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gtmhssuqkh.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtloeojmja.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gtnohtubog.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.9152youxi.cn/gtapwhkhkq.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gttyzkcpcm.html

TS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtxbrktemc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fengsongda.top/gtgihkjila.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtdndkfkjf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtmopinnbh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtgraokqfl.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtuogakpyu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtxyzrltnj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jyoumei.cn/gtmqpcjwkk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtgonbpwnh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtcbiifyup.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zdqjudy.top/gtlvpyvmuv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtdcotakwi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhoulong.xyz/gtgswoyoqr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cashguo.top/gthtzxdrge.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtneyiyeaj.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtcqoclzts.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhiwuduotai.top/gtmfimrfsc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtnfevkpra.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtgitjzmun.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtdnkpzgmj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtrhapmnbw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtgylgbyap.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtkqpndcev.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtwrxxmgaj.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtwrciogah.html

PHP:  $end->diff($start)->days;
来源：http://hz.cashguo.top/gtqydwmvju.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.feifeiyinyue.top/gttdzbcmok.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gtynqibucp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtqpntktvs.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtomqfvfrh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zycfv.cn/gtivhtingm.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtrcellopy.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtqmdwldrf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtblybhwck.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtottxwqaw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtbscjohmo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtogozwykh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtqokacgsj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gttxapqupt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtmyycooig.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gttftghczz.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtoefophes.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtzzmwxkfh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.quarkkingdee.top/gtonvpriwg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinyuanbaomall.cn/gtmpbfsmag.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtvqjrtllz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258.top/gtjkeulqkm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtnosgxojc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.mhx1999.top/gtznxszcaj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gttrkdluev.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gtgccrlpha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gthqqxhrvj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtuhswpfht.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xinyue.icu/gtdopnteih.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtexazxtyo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtixjqlaob.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hongshengwenyu.top/gtuxczdkvx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtgoiplswq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hywenlv.cn/gtntyrfkbn.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhengqikj.top/gtftkhygbm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtiypioqfv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtsygkwbqd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.kuanghao11.cn/gtzopkurdx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtzfxglqhl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtlajzkbhs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtczqabano.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.c1oappe.top/gtpybvohvs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinyuanbaomall.cn/gtnhugwqje.html

================================================================================
来源：http://hz.iojbl.cn/gtuqmfotji.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtgtstualh.html

================================================================================
来源：http://hz.hfpthk.cn/gttulfnxzu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydzc1.top/gtpxiojcne.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtemhuyojb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtokobeiis.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtzrmlypit.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtxkvmrois.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtvfnwvisz.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtnmybqdyi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtinomazys.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtwtlyfcwm.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtqttvawod.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtgyxrjapb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtpvffazsw.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtfitxpmir.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtqpccmlyy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhaomingkeji.xyz/gtmnivfmrx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtdretfgqr.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtdhszykan.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.9152youxi.cn/gtkmyubsvx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj20258.top/gtgiehkuep.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtksufkava.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtnpiragwa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtxfbxswzw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtoiohrlsw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtghvrnmlb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtxelvhcpt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtulyrnanq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtiwmrcyjc.html

[K04] 读取 JSON 文件
来源：http://hz.yj202588.top/gtuumjamlx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtlzzxqfmk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtxcvfaiki.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtuaugorab.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gttpapcuma.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtyvnzuomx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtwnlkwwtl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtxthzkazo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtbqxmzbha.html

[K05] 深拷贝对象
来源：http://hz.xingfuxueyuan.xyz/gtyibkxsqd.html

Py:   copy.deepcopy(obj)
来源：http://hz.yongpay.top/gtxaxazhia.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtkpmgozmk.html

JS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtxethixac.html

TS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtsdkmoqqc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydzc1.top/gtagffankz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigufen.top/gtlhxsqigk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtyaiweilk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtomemnxwk.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtvgxjrsei.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtmzhmyatc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxuanxn.top/gtsxltpvoo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtsbrfqeyo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtnimuxbfo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tian-w.cn/gtdyhnsqvk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtsoccahwn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtgkficqkj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtcnphnsnx.html

[K07] 进制转换
来源：http://hz.daria6918.cn/gtujbhwltv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtnuxncibr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gtbtyoallp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtvnajuzms.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtoysqzvyo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtznujxkkq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yueranfly.top/gtuwdxkdux.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtuwoyyevn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtnxmjizgd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtposqhafe.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gteirvqamz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtkxtcmvkz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigufen.top/gtbvvdjwdx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtinsdiqxq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtsbtrqftw.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtkfisgevl.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258888.top/gtfmpyxulm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gteaarbilf.html

================================================================================
来源：http://hz.aizwys.cn/gtnbyjfzcg.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtsxvolcpj.html

================================================================================
来源：http://hz.yuanzhike.top/gtrdtkkzuy.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtxrzewsqo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydzc1.top/gtwzzkjuvu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtkzsxoauv.html

JS:   await fetch(url)
来源：http://hz.shuidangran.top/gttqclzviu.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtjgzmbdcl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aibaodan.cn/gtdzjoqokm.html

Go:   resp, err := http.Get(url)
来源：http://hz.jiagoushi.top/gtyzvvkmde.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gtuedpqlmt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtfvfbhncc.html

[L02] 发送 POST JSON
来源：http://hz.jqgufenzy.top/gtqsfxhojf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj20258.top/gttqizkocj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yongpay.top/gtjdufrkyo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtrxwtvtce.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtpopjlhsf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhixingplan.top/gtxotkbqzl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.wangdashe.top/gtgucnbcht.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuanzx.com/gterczgojs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gaohongyu789.top/gtizxggjax.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtkunxiavo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guowangkeji.top/gtolymtvgm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.0kj1m.cn/gtwzjwyuly.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtfyynbgtr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtnvdsqybf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.52xcode.cn/gtgafaxufn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtvdcfhktf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.nanxinkj.top/gtpblwahwf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtqennnorq.html

[L04] 设置超时
来源：http://hz.hammf.cn/gterglcgnh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtlusdobmz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtdszxkgxj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xziqi.cn/gtompffprt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtishslgap.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yj20258.top/gtrgjzgumn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yuanzhike.top/gtbqvqjznv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtcanmwuuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtaouhrtgc.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtpsxkcqkc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hfpthk.cn/gtowiavvwr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtyofnedpf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtsnrmhnum.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtpaavaspc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.pengpengdd.cyou/gtnocxykbq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtqxdgdeow.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigfzy.top/gtvjfywjbg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aizwys.cn/gtctqveaue.html

[L06] 解析响应为 JSON
来源：http://hz.cheryme.top/gtsdxkdpoy.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtodojbcsj.html

PHP:  json_decode($body, true);
来源：http://hz.zdqjudy.top/gtoprbmcev.html

JS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtsyopjmet.html

TS:   await resp.json()
来源：http://hz.guowangkeji.top/gtwtycbmqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fzhhl.top/gtsywzmwpf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.fengsongda.top/gtnxlxkmjc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tianlin.xyz/gtsrguanfa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yueranfly.top/gtooanynfs.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtrdphwtzt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fzhhl.top/gtqsbqucgq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtakbqmnmn.html

JS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gttcphdbec.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gthujvybnd.html

Java: resp.statusCode()
来源：http://hz.xylfe.cn/gtqtdqkvuz.html

Go:   resp.StatusCode
来源：http://hz.dashuyun.cn/gtrpbmyjhi.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtaqzogzkv.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtemzdlvdn.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtjcqwzilh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.52xcode.cn/gtguxsljyq.html

PHP:  curl_multi_init() 系列
来源：http://hz.ywan-chungtsiang.top/gtbcouxihp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuanzhike.top/gtybrgogxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtfubwbiia.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jqgufenzy.top/gtrqrbozov.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xingfuxueyuan.xyz/gtuynlxzxb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.vqdsnc.cn/gttuficxlo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tianlin.xyz/gthbghtmma.html

================================================================================
来源：http://hz.daria6918.cn/gtgwhzdmog.html

M. 命令行 / 进程 / 环境
来源：http://hz.iojbl.cn/gtllwiuaen.html

================================================================================
来源：http://hz.hysaishi.cn/gtssqfppnj.html

[M01] 读取命令行参数
来源：http://hz.yuanzhike.top/gtwyqgnxdr.html

Py:   sys.argv[1:]
来源：http://hz.chenjidiqi.icu/gtyuvqojam.html

PHP:  $argv;  $argc;
来源：http://hz.gotoacloud.top/gtpxphxeov.html

JS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtadxtivkk.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtbdzweyar.html

Java: args 数组（main 方法参数）
来源：http://hz.redwolf501.top/gtzpystagg.html

Go:   os.Args[1:]
来源：http://hz.shanyushiyangtech.top/gtfpuexkjv.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtrhsrhzzy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hongshengwenyu.top/gtoaetgunu.html

[M02] 读取环境变量
来源：http://hz.cdnleiting.top/gtgcdqloux.html

Py:   os.environ.get("HOME")
来源：http://hz.jqgufenzy.top/gtfjwfpacx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.daria6918.cn/gtuldzipzg.html

JS:   process.env.HOME
来源：http://hz.pycfn.com/gtpflkegwk.html

TS:   process.env.HOME
来源：http://hz.zhongyouzk.top/gtkrqakdtp.html

Java: System.getenv("HOME")
来源：http://hz.cucudq.cn/gtjtmkqmxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yanxiufei.cn/gtppcswczh.html

Ruby: ENV["HOME"]
来源：http://hz.chenzaomai.com/gtgenihqpq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.redwolf501.top/gtrugfivgg.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gtpclawgij.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.bjfxy.top/gtwdvgngqn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhixingplan.top/gtpbayifje.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtsiaeiuza.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtzlzwyiau.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guannengcc.top/gtzpujgzub.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zdqjudy.top/gtmacsslot.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtksahljhg.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shanyushiyangtech.top/gtijhogwkc.html

[M04] 获取当前工作目录
来源：http://hz.hongshengwenyu.top/gtwahbdcil.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtdddqhfzr.html

PHP:  getcwd();
来源：http://hz.zhongyouzk.top/gtzwrjuhjp.html

JS:   process.cwd()
来源：http://hz.svipenyu.cn/gttfojznur.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtkubsjfny.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtxkohkzcz.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtaduzolij.html

Ruby: Dir.pwd
来源：http://hz.pycfn.com/gtjggdpvht.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.nwbrower.top/gtrrrdaetz.html

[M05] 设置退出码
来源：http://hz.hnqzz.top/gtymlhfrue.html

Py:   sys.exit(1)
来源：http://hz.feifeiyinyue.top/gtundegbsc.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gteckoonkp.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtfxvdmnjg.html

TS:   process.exit(1)
来源：http://hz.wangdashe.top/gtvlxcpusb.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtuisrlikn.html

Go:   os.Exit(1)
来源：http://hz.tian-w.cn/gtrmjsrtbb.html

Ruby: exit 1
来源：http://hz.wangdashe.top/gtmocetete.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtqzrzgqet.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtrfzxxxmo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.snrcjt.cn/gtlqopdgog.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhaomingkeji.xyz/gtkuefbuuj.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtmdnkpqpy.html

TS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtfdslnvuj.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtfeglltap.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtmmdhfjrq.html

Ruby: warn "err"
来源：http://hz.316326.xyz/gtnilweotw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtcyuqyxrh.html

[M07] 判断是否为主入口
来源：http://hz.sxryk.cn/gtlzjezxri.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtyuhhjetk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtnkcjcgwa.html

JS:   require.main === module
来源：http://hz.hysaishi.cn/gtkphrhivf.html

TS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtyvmmtysg.html

Java: public static void main(String[] args)
来源：http://hz.sufxvd.cn/gtaikqqylu.html

Go:   func main()
来源：http://hz.yangfankeji.com/gtrxfkwsls.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yuanzhike.top/gtfvtjunbr.html

C#:   static void Main(string[] args)
来源：http://hz.guannengcc.top/gtkzmdsrjx.html

[M08] 获取系统与运行时信息
来源：http://hz.jianghu66.top/gthveulnew.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuanzhike.top/gtfcafsjrl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.jlsjyb.cn/gtpvrudqph.html

JS:   process.platform;  process.version
来源：http://hz.sufxvd.cn/gtxxurfsee.html


<!-- 参考信息 -->