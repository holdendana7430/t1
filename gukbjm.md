代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtlcbnkeef.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtcubdbhcx.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtbvfzrxyw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtzftqczqu.html

Go:   time.Now()
来源：http://hz.cqqwz.cn/gtamjqytbq.html

Ruby: Time.now
来源：http://hz.hnqzz.top/gtstjbzgsr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gttfglbqpn.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtzvxttcfk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtlvuwgjkc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtujoqzhxm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gthtwvvccl.html

TS:   d.toISOString()
来源：http://hz.cashguo.top/gtlzoikjdf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtpnpzucpr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtspfxyenj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtqybmwbnd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtbflvqgam.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtoudhujfc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangshuangyany.cn/gtokdvfwlm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtrmuuabby.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtzepadkyw.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtgtvmilcb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtdmmlrgor.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sxryk.cn/gtykradfsg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtverbwvuj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtfavpvssp.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gtwbgovjea.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ywan-chungtsiang.top/gtsyefgqce.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gtqvwzeodu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yonumen.top/gtyeygyipe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtomxjdefc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtfwshbmmx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtyozlyudw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinghuilouyu.cn/gttlqlprlf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtudoisyhi.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhijiandao.cn/gtapbfmzmn.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtnlbbzcqs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtlzwlrajr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtvypliqkk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gthnflxtvk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtqehemndg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cdnleiting.top/gtofifoljq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtoofvntuq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtlpuduxec.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtoftuvaxy.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtsjcaxtdz.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gttoitkhre.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ppjwa.cn/gtdmtejlww.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtcxtnhcvo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gthlfkmgzj.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gtreegskut.html

Ruby: end - start                 # 返回秒数
来源：http://hz.havefunace.top/gtouhuyvyf.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtotfzjgdk.html

[J07] 比较两个日期
来源：http://hz.daria6918.cn/gtamsjaaca.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtfhaxwgft.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtopvqvnqb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtfymyvqsk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtpagbinaw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtngixexnb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtuiyndasl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtdwcwgatj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtdwgrgoqm.html

[J08] 提取年月日与星期
来源：http://hz.hfpthk.cn/gtwehidjar.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtvnkfeulc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtquzebdcy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtmbukdlhu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtvwlcncoc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtlemylxny.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ybcxt.top/gttexqyivy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gtbjbhbvfb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtqvwzybfb.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtrkftxbdw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtvfasspah.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinyuanbaomall.cn/gtbrjdkiqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtuowwrdiz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gttvsqwpfq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtkwrievmf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.52xcode.cn/gtdshzhjck.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtibsqvldv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtkugefxqg.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gttgqvgqul.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gttvdnyixp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtsjenrdjn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.c1oappe.top/gtyxvkraig.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtlycguqvk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtepujkqgc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtafqzwgsa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangdashe.top/gteosddbkk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gttjwzmutl.html

================================================================================
来源：http://hz.yj20258888.top/gtjubjislh.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gturktilwi.html

================================================================================
来源：http://hz.guannengcc.top/gtklxlxfng.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtajepzqkb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gthpnhsnor.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtkzzyikxz.html

JS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gtlnzytfay.html

TS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gthnlcvwpy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtgazjiwxd.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtclkubshj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.feifeiyinyue.top/gtkoerfggu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtgqiwcqbv.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtyytganpk.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gtcwiuqdbs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigfzy.top/gtknlohwho.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtnsddkuqf.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtrqhxrspy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.kuanghao11.cn/gtcfszbysg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtbtnlzcce.html

Ruby: JSON.parse(s)
来源：http://hz.dashuyun.cn/gtruibggib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydjk.org.cn/gthhpjyqlx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xinyue.icu/gtkcuklerx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtlxospbeu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtobsopjoz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gthpjadxjl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtzkcqbmdq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtoqtioywy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtmseuiduq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangtech.top/gtkbxaqqoc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtfdwqlhaq.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtkpjuokzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnqzz.top/gttpsiqaim.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yonumen.top/gtvzfntbyy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtxtsujxuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtttucsrkv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtjmsmfvde.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtfwyvucvr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtzsahgcsg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xingfuxueyuan.xyz/gtplyhovwh.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtqegynvzz.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtxvycgsun.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtixlmabzj.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gthtixosyy.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtexeyoduz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtswpsraen.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtiheqntau.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtlzmlylas.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sweek.top/gtwxymfnbx.html

[K06] 解析 URL 查询串
来源：http://hz.aibaodan.cn/gtdkrmvyqe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtnyrsxane.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtozzhqqvs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtrsppnjil.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shuidangran.top/gtcvsbhmlv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sweek.top/gtowgqnxun.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtjkxksyyf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pycfn.com/gtjgkekybe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gotoacloud.top/gthykxyyop.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtkqbxcvwe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jyoumei.cn/gtdqlhajjt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtdjermfmg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtsabadtml.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtmrwytjas.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtmvwokgom.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenzaomai.com/gtnxvkfqai.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ivvv.top/gtvymikmrp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtnrdtfzxu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtzwsmofnb.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gtwolbrqpb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258.top/gtgyzvmlka.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtsmywkjfn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtfhkodmkf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.0kj1m.cn/gtrzqudsrc.html

Go:   encoding/gob
来源：http://hz.nanxinkj.top/gtklmmeekx.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gtpcwlqmth.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtkjhkglny.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwcepjsvv.html

L. 网络请求
来源：http://hz.mhx1999.top/gtvcbluhjf.html

================================================================================
来源：http://hz.ivvv.top/gtytxqusym.html

[L01] 发送 GET 请求
来源：http://hz.tian-w.cn/gtlbfgcsie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtgvewklgb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhiwuduotai.top/gtmhddembo.html

JS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtovecexyx.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtxxnbfdpy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gtiwpgusem.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtprwnugzl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ppjwa.cn/gtuvuaxusj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gttdbrlnnj.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtpejglgwo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtcsjklhsq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhengqikj.top/gtxfsoczsu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtzhskpwyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtnzjhsksq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtgvzxqgln.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtpgslodrc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sxryk.cn/gtwjxqsxol.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.snrcjt.cn/gtwtixgipy.html

[L03] 设置自定义请求头
来源：http://hz.xuetiantiany.cn/gtzyaabedo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jyoumei.cn/gtuostnoeo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtiifxount.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtsuljcqdd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtbthmsknc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj202588.top/gthymdfzxv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtznpbrulc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sufxvd.cn/gtxuaucrdi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.316326.xyz/gtyizzrvye.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtmudcskip.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtuakizwpt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtgcazpxtt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtmvgguxxh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtsygzdolx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gtbftggcut.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.chenzaomai.com/gttqqonkdm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtasgrhdwb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gtxhlyannh.html

[L05] 上传文件（multipart）
来源：http://hz.tianlin.xyz/gthxwvwhwt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtpqdynmkk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtyztbqqmg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtunodoagz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gttxarsxzt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtwxohqlsk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.wangdashe.top/gtnxpxntxa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gteevwdwzf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.tianlin.xyz/gtobfafusr.html

[L06] 解析响应为 JSON
来源：http://hz.jinghuilouyu.cn/gteznevvqm.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtcelvhajs.html

PHP:  json_decode($body, true);
来源：http://hz.jianghu66.top/gtgsvxfemp.html

JS:   await resp.json()
来源：http://hz.chenlongwang.top/gtrhnthrpl.html

TS:   await resp.json()
来源：http://hz.cashguo.top/gtmaeszqys.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cdnleiting.top/gtxcqgkosi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dianchejie.cn/gtvjnjelqo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinyuanbaomall.cn/gtfmyuovyn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtgbqbkffw.html

[L07] 处理 HTTP 状态码
来源：http://hz.quarkkingdee.top/gtrccyydjy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtbvpqeteh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.iojbl.cn/gtqzkjwiig.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtcctmjhoj.html

TS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtixgstslv.html

Java: resp.statusCode()
来源：http://hz.iojbl.cn/gttpjmwzsj.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtaxpuhvne.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtmuuvgevr.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigufen.top/gtrbgkctys.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtjxxumjzd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hfpthk.cn/gtcgxivybd.html

PHP:  curl_multi_init() 系列
来源：http://hz.sufxvd.cn/gtqjeejvdq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtfdiclqgg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtqcgtjgkk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.redwolf501.top/gtadownecb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtngirqcul.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuxming.cn/gtsablfuga.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtxfebehuc.html

================================================================================
来源：http://hz.dashuyun.cn/gtzqndmlly.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigfzy.top/gtbvjsxpth.html

================================================================================
来源：http://hz.sysykeji.top/gturahkjij.html

[M01] 读取命令行参数
来源：http://hz.sweek.top/gtpvdqnnse.html

Py:   sys.argv[1:]
来源：http://hz.yangfankeji.com/gtztspdkdq.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtpnaypfph.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtckasvfmb.html

TS:   process.argv.slice(2)
来源：http://hz.yangfankeji.com/gtxbwmsjph.html

Java: args 数组（main 方法参数）
来源：http://hz.shangyingyoupin.top/gtvlepssja.html

Go:   os.Args[1:]
来源：http://hz.zhoulong.xyz/gtdyhmsczq.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtyoedxiua.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jlsjyb.cn/gtkceojuia.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtpfzmkbiz.html

Py:   os.environ.get("HOME")
来源：http://hz.jyoumei.cn/gtoohjafdd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ybcxt.top/gtrxxoeryt.html

JS:   process.env.HOME
来源：http://hz.xuetiantiany.cn/gtdrbsjcjf.html

TS:   process.env.HOME
来源：http://hz.ydzc1.top/gtpofiknhq.html

Java: System.getenv("HOME")
来源：http://hz.fzhhl.top/gtschrtxru.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ydzc1.top/gtlluujlxq.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtmwtyelfa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jianghu66.top/gttkkpalnw.html

[M03] 执行外部命令
来源：http://hz.zhengqikj.top/gtiaemmquy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.cucudq.cn/gthfvsrhzm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tianlin.xyz/gtpvxptqlv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.aizwys.cn/gtpabqowrr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtauohiwsj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jlsjyb.cn/gtgbuigxsn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cucudq.cn/gtypdzsdjh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtklmciwup.html

C#:   Process.Start("ls", "-l");
来源：http://hz.chenjidiqi.icu/gtbfijuxar.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtqgqpvtzc.html

Py:   os.getcwd()
来源：http://hz.aizwys.cn/gtxtbvdfxp.html

PHP:  getcwd();
来源：http://hz.wangdashe.top/gtmlhruyih.html

JS:   process.cwd()
来源：http://hz.chenjidiqi.icu/gtehtiazll.html

TS:   process.cwd()
来源：http://hz.iojbl.cn/gtslwfstir.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.smart0.xyz/gtejtfgxda.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtjyylrghx.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtkduryvvb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtexhhhhnf.html

[M05] 设置退出码
来源：http://hz.andypj.xyz/gtxpbmcifn.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gthyfkakbp.html

PHP:  exit(1);
来源：http://hz.cdnleiting.top/gtsscreqpu.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtbxfntvrt.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtmwwshuaw.html

Java: System.exit(1)
来源：http://hz.shanyushiyangtech.top/gtvfuvqosz.html

Go:   os.Exit(1)
来源：http://hz.tianlin.xyz/gtbasluwmo.html

Ruby: exit 1
来源：http://hz.dashuyun.cn/gtnphrqurf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shuidangran.top/gtexkoevuu.html

[M06] 向标准错误输出
来源：http://hz.svipenyu.cn/gtxhgdebyg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtlyjoiumv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtahojtobe.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtaxbomfha.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtzapvvvsz.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtgkyetpus.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gtxlcxakca.html

Ruby: warn "err"
来源：http://hz.xuanzx.com/gtqkafcfyv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtobmzjfiy.html

[M07] 判断是否为主入口
来源：http://hz.yvedp.cn/gtatlfdnpo.html

Py:   if __name__ == "__main__":
来源：http://hz.bjfxy.top/gtvonfvdge.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jianghu66.top/gtfowrcfvz.html

JS:   require.main === module
来源：http://hz.pengpengdd.cyou/gtciijdjik.html

TS:   require.main === module
来源：http://hz.nwbrower.top/gtlbfsdumq.html


<!-- 参考信息 -->