代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtmtkiamea.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtfxkpvxth.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hysaishi.cn/gtkxeprdlc.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtqxzjgnvs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtqfpeaivc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinyuanbaomall.cn/gtxdobkaqg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtiozjzmft.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtekyjfkbm.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtryfxdwtb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtafiypanu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtlxscohdq.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtnqsqkfmv.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtxsbgzmhz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gthnedowbg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtsqwknshr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtzjriqssy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtszlujdbj.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtnpvhbikr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtigfcjkbd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cashguo.top/gtafyjnzxi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtkpmhpbex.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daria6918.cn/gtmxlhbcsf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtblqjqwii.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.fzhhl.top/gtnwtepwxm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtymbhxsjr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtkendbvmx.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtksogspaf.html

Py:   now + timedelta(days=7)
来源：http://hz.cdnleiting.top/gtdbssaffj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtrbqpnjmc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtfgqqhpgz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gtfbfaynuk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jlsjyb.cn/gtrlskatdw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtdxkeybhk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnxiangtu.top/gtewgfmpph.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtmphuvihc.html

[J06] 计算两时间之差
来源：http://hz.hnxiangtu.top/gtoyzuvbcd.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtjmzrvgqr.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangdashe.top/gtotzufawo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gogol.net.cn/gtgmmkwbqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.aizwys.cn/gtuhijtluz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydzc1.top/gtnobfwshd.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtgearahft.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtdgjrjiad.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtzavrgfaw.html

[J07] 比较两个日期
来源：http://hz.fengsongda.top/gtvtsyqcxo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtxnqkuvpp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtmrvxkwbo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtdtctdrme.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtuukactcm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.vqdsnc.cn/gtbzjomsdi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fzhhl.top/gtncynjqqy.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtrlglyskx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtcqdbmaeh.html

[J08] 提取年月日与星期
来源：http://hz.ywan-chungtsiang.top/gtjhlfpncl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtfiixoyas.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtkhsuaqqn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtxxxxrbgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtsziuxyno.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtznyheaox.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtwgkckpso.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hysaishi.cn/gtolyfjkrv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtkwtguifn.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtfnyvxdit.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtwzigsyka.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gttxlwupux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtghzywouw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtpepkbwzm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtclyrnlcc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xingfuxueyuan.xyz/gtyordalga.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gthcbkpdbm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.quarkkingdee.top/gtjuxybhkc.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtqmkcnvkw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gttidfakxe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtzeissrey.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtvfhzewjk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gttjaniboo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gttdchsfyf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gtyozrvkwh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtmawazbac.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtozkjbnkl.html

================================================================================
来源：http://hz.yj202588.top/gtlfpymmqp.html

K. JSON 与序列化
来源：http://hz.yuxming.cn/gtoawgjxij.html

================================================================================
来源：http://hz.jianghu66.top/gtetexuzyx.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtmtyhgnau.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtqcvhpgxy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtxpqhcgzf.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gteaiglmso.html

TS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtxeglamlm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtvkusujir.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtgfcufouy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtjckobcoz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtguscxpim.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtobdowytg.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtyfplozkp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gthsmjnqrr.html

JS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtmhtvejpg.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtgrgxotri.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtbftoqtnn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtkdphrgbb.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtygongddd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sxryk.cn/gthgkabxbi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtixaiyhiw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtdgfblcsf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gthbqwtasi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtpwuqgnva.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtksfzprei.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtoypcjvqn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenzaomai.com/gtrhlajvsp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtlxntdlyg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gtfxkoafqn.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtgrkfrhnm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtpwvnqkfq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangdashe.top/gtpihietto.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtncxndrtt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtvojggczg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtdsoiflwz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtgdrfdcrz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtblgqnwtb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gotoacloud.top/gtfsjajogl.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtkdnevusj.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtexuvycou.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258888.top/gtrvkudbbm.html

JS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtqugplhcy.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtldmvvnbp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtwhymhzau.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtxmxvmbxg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtdoswdhjd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhongyouzk.top/gtpkvexkwh.html

[K06] 解析 URL 查询串
来源：http://hz.guowangkeji.top/gtaqjemhuf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.bjfxy.top/gtocbomxyw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hammf.cn/gtmkmjxsld.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtpbrtbfbw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtffwkjkpq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtxccokham.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtrvoyjraq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtivjzbggh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtbqtokqbz.html

[K07] 进制转换
来源：http://hz.jyoumei.cn/gtkryznfkb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gtqnajpiwk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtobjtsxkf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtliyjxsbu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtxfoabbim.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtyziowwpa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xylfe.cn/gtqbyxjlty.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigufen.top/gtfsrdtbup.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gthehvdswo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtazxfhpyk.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gteusgbtit.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtlieikwve.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.aibaodan.cn/gtduzvzgbg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtfjdvpcck.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtqrhzlust.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtpwswttnr.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtwmshjcid.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuanzhike.top/gtfodmegnp.html

================================================================================
来源：http://hz.fzhhl.top/gtnlmoswit.html

L. 网络请求
来源：http://hz.yuxming.cn/gtlgvadlng.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcjlayged.html

[L01] 发送 GET 请求
来源：http://hz.cheryme.top/gtahshjvgv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtawdfeszz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtdvxtvbwj.html

JS:   await fetch(url)
来源：http://hz.daria6918.cn/gtiqplarqq.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtkvgpsvhx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtcnehwwcv.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtuekxhgup.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtcmhtjbtx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yangfankeji.com/gtspqeykrx.html

[L02] 发送 POST JSON
来源：http://hz.cucudq.cn/gtplgzbljp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hysaishi.cn/gtlpmpmtmo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gtgamijulu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258.top/gtzxkaoiua.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtkpkijmia.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sweek.top/gtjwihsmdl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.dianchejie.cn/gtnwqqrtks.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtfsswiyeh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yvedp.cn/gtuzrarpvi.html

[L03] 设置自定义请求头
来源：http://hz.cdnleiting.top/gtbmwkhydz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.guannengcc.top/gtfebbuwqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhongyouzk.top/gtpivrltra.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtvtyudmsq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fzhhl.top/gtvyucynir.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gtxbrrbvet.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtnywmswhx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.smart0.xyz/gtghvrzvwo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.c1oappe.top/gtlzidrbkn.html

[L04] 设置超时
来源：http://hz.mhx1999.top/gtniatdhtd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hywenlv.cn/gtlpxaujif.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.smart0.xyz/gtowclcbex.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtxzjurmbj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenzaomai.com/gtfvuisoko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hongshengwenyu.top/gtprfeorky.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtglgcyzna.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ydjk.org.cn/gthmkkhiku.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zycfv.cn/gtrjdcoskb.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtzfugyond.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.mhx1999.top/gtyndzpwue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhixingplan.top/gtgwybnjsa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zdqjudy.top/gtrzwdxulw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.mhx1999.top/gtpiesmsxc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtbxvyevci.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jianghu66.top/gtfxlvosfn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hnxiangtu.top/gtctxrznrg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gteugriwge.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtlhlmtrpd.html

Py:   resp.json()
来源：http://hz.yj20258.top/gttzpmlwwr.html

PHP:  json_decode($body, true);
来源：http://hz.kuanghao11.cn/gtgezxihhx.html

JS:   await resp.json()
来源：http://hz.dashuyun.cn/gtzmzyykrw.html

TS:   await resp.json()
来源：http://hz.gaohongyu789.top/gtidvnmbcq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenzaomai.com/gthkleakgo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gthflusdsz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhiwuduotai.top/gtnsnipzka.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aibaodan.cn/gtfxtfjuse.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtmtwdpffl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ppjwa.cn/gtukjlafzd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yangfankeji.com/gtzvgaisbk.html

JS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtbqmkgvht.html

TS:   resp.ok;  resp.status
来源：http://hz.ywan-chungtsiang.top/gtzsajczjx.html

Java: resp.statusCode()
来源：http://hz.52xcode.cn/gtyjhhvfal.html

Go:   resp.StatusCode
来源：http://hz.gzhubu.top/gtwbqgkqsk.html

Ruby: resp.code.to_i
来源：http://hz.jyoumei.cn/gtuftdhewo.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtjzzaxdoi.html

[L08] 并发请求多个地址
来源：http://hz.meibo888.top/gtynjezcdf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtvipwahze.html

PHP:  curl_multi_init() 系列
来源：http://hz.zycfv.cn/gtetsvxebg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shuidangran.top/gtiuxrvalr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtuivjehfm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sufxvd.cn/gtunqrfthl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtgffzfsnv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtcaaygama.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.sysykeji.top/gtgqbafaqn.html

================================================================================
来源：http://hz.yuanzhike.top/gtnnqwewog.html

M. 命令行 / 进程 / 环境
来源：http://hz.pengpengdd.cyou/gtmoyheade.html

================================================================================
来源：http://hz.gotoacloud.top/gtbcfdaxok.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtqjuhqdwu.html

Py:   sys.argv[1:]
来源：http://hz.wangdashe.top/gtiwuhrovw.html

PHP:  $argv;  $argc;
来源：http://hz.jyoumei.cn/gtogsbypzv.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtojobzfgu.html

TS:   process.argv.slice(2)
来源：http://hz.ydjk.org.cn/gtqpcrgken.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgufenzy.top/gtbkgqcftr.html

Go:   os.Args[1:]
来源：http://hz.wangshuangyany.cn/gtngvwfntc.html

Ruby: ARGV
来源：http://hz.svipenyu.cn/gthvfijhxr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtdkcnqhbk.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtbsdqiixx.html

Py:   os.environ.get("HOME")
来源：http://hz.pengpengdd.cyou/gtefswnhyd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenjidiqi.icu/gtjticlmwp.html

JS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtezyftgjq.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtygwknspj.html

Java: System.getenv("HOME")
来源：http://hz.fengsongda.top/gtzkrlkgss.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.chenzaomai.com/gtkjkapivo.html

Ruby: ENV["HOME"]
来源：http://hz.jqgfzy.top/gteoyzujlb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtwatxuzmo.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtiinltqmo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.tanke756.top/gtbhbuuerf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtdvybgehz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtnxvtgpue.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtwfxvhhju.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.wangshuangyany.cn/gtqgpfcklo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtjvfkqtgt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yuxming.cn/gtjmmvznyv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hnxiangtu.top/gtxewuorel.html

[M04] 获取当前工作目录
来源：http://hz.hammf.cn/gtjcvxbjiu.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtclgyqguq.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gtudgywpfq.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gtmgecoosr.html

TS:   process.cwd()
来源：http://hz.yj20258888.top/gteeasbccu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnxiangtu.top/gthrzkxwtb.html

Go:   os.Getwd()
来源：http://hz.shuidangran.top/gtowkwoqft.html

Ruby: Dir.pwd
来源：http://hz.bjfxy.top/gtozrgjjgy.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtefendmrd.html

[M05] 设置退出码
来源：http://hz.fengsongda.top/gthksjzxvx.html

Py:   sys.exit(1)
来源：http://hz.cheryme.top/gthpstvtmf.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtmstddvaa.html

JS:   process.exit(1)
来源：http://hz.yanxiufei.cn/gtcyfptaij.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtllnlbsok.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gtvrbqikpk.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtjsyisytl.html

Ruby: exit 1
来源：http://hz.9152youxi.cn/gtanrreotg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgfzy.top/gtnqvtlvxk.html

[M06] 向标准错误输出
来源：http://hz.aibaodan.cn/gtsccedhps.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gthzrzrexg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.andypj.xyz/gtwfqqrlha.html

JS:   console.error("err")
来源：http://hz.smart0.xyz/gtwchggsfe.html

TS:   console.error("err")
来源：http://hz.cdnleiting.top/gtvgmalpci.html

Java: System.err.println("err")
来源：http://hz.xylfe.cn/gtfrxvpvdx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtiratkisr.html

Ruby: warn "err"
来源：http://hz.hongshengwenyu.top/gtphjrbynf.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sysykeji.top/gtfythlkvz.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtvecmgzdr.html

Py:   if __name__ == "__main__":
来源：http://hz.chenzaomai.com/gtjdykiivm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj20258888.top/gtswroytxp.html

JS:   require.main === module
来源：http://hz.havefunace.top/gtahzgeiqy.html

TS:   require.main === module
来源：http://hz.redwolf501.top/gtbzrybnbz.html

Java: public static void main(String[] args)
来源：http://hz.shangyingyoupin.top/gtzakielqy.html

Go:   func main()
来源：http://hz.bjfxy.top/gtevgeipwd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gtmthtkfpr.html

C#:   static void Main(string[] args)
来源：http://hz.gotoacloud.top/gtwdcfbhmv.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gthsgczool.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtxhgjhyor.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tanke756.top/gtijbfvswm.html

JS:   process.platform;  process.version
来源：http://hz.mhx1999.top/gthfwjwrur.html


<!-- 参考信息 -->