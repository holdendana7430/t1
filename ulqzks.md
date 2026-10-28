代发 wailian999

J. 日期与时间
来源：http://hz.9152youxi.cn/gtauxwxxqk.html

================================================================================
来源：http://hz.hfpthk.cn/gtgxsezpfd.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtsdivqsme.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtvwuxopqj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtizfpxwsh.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtriputyma.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtduddipua.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtobwvfonn.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtnrlmtyql.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtnybfjglz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtrxbzyxhd.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtgfvwvbqw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gttdhlqcxy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gthlhppokj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtvseegrag.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtekiofgmz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtbxoigufj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.haohaochexian.top/gtabauoxii.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtklxpsbso.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigufen.top/gtoxuzgybm.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gtyaletrta.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtqyadeeid.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guannengcc.top/gtpcaudumm.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtjjkxosww.html

TS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtlnsaepda.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtfqxrmqvc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.bjfxy.top/gtpgcrdihs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtzzqbrajb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtplkthlhe.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtiyjhbmui.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtojrlbdco.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtcpbkmait.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtvbcyxmkb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gttcvuoxpr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtedprmwym.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtgczyopyp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gtocdktckr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxuanxn.top/gtgrstovbj.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtcqvetsno.html

Py:   now + timedelta(days=7)
来源：http://hz.andypj.xyz/gtwzbsesgo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtfjfztutq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtqujhxdea.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtnelcmdwq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtzaicyqgr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtgfnevwno.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtgdfyscvv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtdvmqprxm.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtlmiipexz.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtgqdznfzo.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuanzhike.top/gtzaizuqob.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gthrrgaltg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtbwgmrken.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtejxxhwgw.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtpzlneeve.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtzuoyzkcb.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtpzesresy.html

[J07] 比较两个日期
来源：http://hz.gotoacloud.top/gtdowbpfoc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtriyjihew.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtzqakewor.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ivvv.top/gthtezquxj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtbdmkekam.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtwnelaakk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtozjfvhur.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtbvavbndm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtxzqwhgjk.html

[J08] 提取年月日与星期
来源：http://hz.xuanzx.com/gtzgqikbgd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtkkhfmhpg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cheryme.top/gtfigkzmwy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtzkpnkvtm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtelzdiolp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hammf.cn/gtznnqzbqw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gthfezpfol.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gtoexkwnnv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gotoacloud.top/gtoajkdvkk.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtdhajpzoy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtqwooqqcq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtkpllzwes.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtpovjkgwn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gthuekegnd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtgjgkwmke.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinghuilouyu.cn/gtkbmgjvet.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gthnkxcics.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtgjomfhno.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtwaaqvbxx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtnmvozcyq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aibaodan.cn/gtndfvtryb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtxngszilc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guowangkeji.top/gtamsbiyit.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtcekeigfv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gtzyjpylsl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yongpay.top/gtxpbzyogp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtiwzicbad.html

================================================================================
来源：http://hz.yueranfly.top/gtqoylfqdu.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gtxugscwuk.html

================================================================================
来源：http://hz.yueranfly.top/gtmgpdjspg.html

[K01] 对象转 JSON 字符串
来源：http://hz.fzhhl.top/gtrbhqjeoo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtbhhalalb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtjymivotp.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtxvusxpax.html

TS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtzwuedkwu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtpvezxrkc.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtoamnpvoo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hywenlv.cn/gttbsaapeu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtvcuacuat.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtnuowjjtv.html

Py:   json.loads(s)
来源：http://hz.hysaishi.cn/gtynakaxpw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yvedp.cn/gtqsurjagn.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtcldzyxou.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtilpklvdz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nwbrower.top/gtnvmtlcfb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtwgppfvcl.html

Ruby: JSON.parse(s)
来源：http://hz.hywenlv.cn/gtngfyjawc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtlvjyfulh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtwyjvxhut.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtnrfzxrxh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtmiarhqtd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtjadsifex.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtujwyboor.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtvxsygkha.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nwbrower.top/gtfqinzhdp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.feifeiyinyue.top/gtymtvdgqy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ydzc1.top/gtsnaxhbkd.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gtcgnvmgng.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtbfuiutsv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xinyue.icu/gtpfjhbphd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtneozhvyb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtjlwiqxjb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shuidangran.top/gtoswvefqj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.9152youxi.cn/gtpddkonkw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.snrcjt.cn/gtcwtyyery.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gtmcvbpevy.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gthyqndxhj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtwuzcnawg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dashuyun.cn/gtbtejaapk.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtrdtehrzu.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtqedtcnle.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtcllevnok.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtfgblpily.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtnpkvgnrc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtdcerykdt.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtlivjdmdg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinghuilouyu.cn/gthiwvcybg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.redwolf501.top/gtrfoemyuh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtlptnptlu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtkrruvxyo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtauargklv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtuzpcphfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtbvxmotjm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ehwqpu.com/gttymzdapx.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtzqgoouqj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtwmsohots.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinyuanbaomall.cn/gtwaotobie.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtuxzanheb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtjqznruar.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtsdlwwipl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtcqoxkpix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yueranfly.top/gtggzuzsmu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gthwkeapsh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gtvwcczvrf.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtiqijncpe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.andypj.xyz/gtvgigjpii.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtgimoftia.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtnzshvtkx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gthhnrcsma.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtcabvugzo.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtryknngwr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtgtnrigjr.html

================================================================================
来源：http://hz.aibaodan.cn/gtmxttjioj.html

L. 网络请求
来源：http://hz.jinqigufen.top/gtxfwmowkq.html

================================================================================
来源：http://hz.jlsjyb.cn/gtnwhyfaba.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtbmsjwdka.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtqnamfcyb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtzhjhkhjb.html

JS:   await fetch(url)
来源：http://hz.c1oappe.top/gtdvwpdkbn.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtcmaebqbp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.fzhhl.top/gtdqlchcje.html

Go:   resp, err := http.Get(url)
来源：http://hz.daria6918.cn/gtupthwlxz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gttnexkpqr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.kuanghao11.cn/gtylesteal.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtbsqsbzer.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tanke756.top/gtefyzaauv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtzkegbqnu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhongyouzk.top/gtzvylojil.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtjcnfnzrt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtkesxjhou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yuanzhike.top/gtvsvuzsik.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aizwys.cn/gthslagmiu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sweek.top/gtcsfjmmcu.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtsxyrpfgd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhaomingkeji.xyz/gthebhefvv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtnojqjkmf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtyoseahxi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtqdbgjbhk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gttdebrgzh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtspdumgvz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.haohaochexian.top/gtcxlmnlgp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hfpthk.cn/gtxzcfxfzp.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtsgaciyfu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ivvv.top/gtpmmmitbl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtebfcbkgi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtwmlsilhe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtkucpbskl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gthbmnxaaa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtdrvzyiqh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtvulhcdtw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtmlqzaddk.html

[L05] 上传文件（multipart）
来源：http://hz.yj20258888.top/gttvmypcps.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258888.top/gtutblpltc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtqtikgekz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xinyue.icu/gteverqmly.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gttwrobgzd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.316326.xyz/gtudvuvljv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtcukzijje.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cucudq.cn/gtlxahijbu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.andypj.xyz/gtfppwkvdd.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gtbjsavnll.html

Py:   resp.json()
来源：http://hz.0kj1m.cn/gttirjdwca.html

PHP:  json_decode($body, true);
来源：http://hz.hfpthk.cn/gttzzclodo.html

JS:   await resp.json()
来源：http://hz.yueranfly.top/gtykmztnvz.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gtvklyeqcb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtxwlxjopr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenjidiqi.icu/gtfvaauilg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yj202588.top/gticctvnod.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gthxywjmvn.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtcrlzlzjg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gtkstxqowt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gtkdkpqxvn.html

JS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtlvhyhsrh.html

TS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gtxchwdstz.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtyvhhfpfv.html

Go:   resp.StatusCode
来源：http://hz.zhoulong.xyz/gthyfdygdg.html

Ruby: resp.code.to_i
来源：http://hz.jinyuanbaomall.cn/gtqiotjxca.html

C#:   (int)resp.StatusCode
来源：http://hz.tian-w.cn/gteemjiidb.html

[L08] 并发请求多个地址
来源：http://hz.daria6918.cn/gtfodoszpf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.quarkkingdee.top/gtxnlsbqjz.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtcitxyixt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shzxlz.cn/gtsssevddc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.aizwys.cn/gtcsroabgi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinghuilouyu.cn/gtjfndmxuo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.wangshuangyany.cn/gtxkmyzazx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangdashe.top/gtcvhpmyyc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ivvv.top/gtpfdkqroz.html

================================================================================
来源：http://hz.gotoacloud.top/gtgduxkkso.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtjpgyytzr.html

================================================================================
来源：http://hz.andypj.xyz/gtctrnycfz.html

[M01] 读取命令行参数
来源：http://hz.zdqjudy.top/gtedbqcwmh.html

Py:   sys.argv[1:]
来源：http://hz.hammf.cn/gtnmpcxmto.html

PHP:  $argv;  $argc;
来源：http://hz.zhiwuduotai.top/gtvoxdtgoe.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtylduxinl.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtcdyocmja.html

Java: args 数组（main 方法参数）
来源：http://hz.hnxiangtu.top/gtooizvxit.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtfwmikjun.html

Ruby: ARGV
来源：http://hz.chenzaomai.com/gtkmkitgra.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtxxspvwor.html

[M02] 读取环境变量
来源：http://hz.jiagoushi.top/gtrwygbyji.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtuflgqutf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtogcotmfh.html

JS:   process.env.HOME
来源：http://hz.dashuyun.cn/gtllkgzuqe.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtvmrmomdg.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtgtbsavxl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.fzhhl.top/gtdfnmigcl.html

Ruby: ENV["HOME"]
来源：http://hz.xuetiantiany.cn/gtyekzaqqw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.iojbl.cn/gtbjojbrfc.html

[M03] 执行外部命令
来源：http://hz.yuanzhike.top/gttcrpsmpx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gteyknsfzr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj202588.top/gtttjwrypc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinghuilouyu.cn/gtdettjusx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtixkyzjed.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xingfuxueyuan.xyz/gtjcfldpjn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenzaomai.com/gtyavdoabp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.pengpengdd.cyou/gtfgsryoww.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtutgalxab.html

[M04] 获取当前工作目录
来源：http://hz.pycfn.com/gtfirdmsht.html

Py:   os.getcwd()
来源：http://hz.cqqwz.cn/gtzvkaswjx.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gttaxunbsu.html

JS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtjyhvwapz.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtgrxllpqo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aizwys.cn/gtsargojuh.html

Go:   os.Getwd()
来源：http://hz.zhongyouzk.top/gtlxonfuaa.html

Ruby: Dir.pwd
来源：http://hz.jqgufenzy.top/gtqiwnkujw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhoulong.xyz/gtlftcdbzq.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gteryrvupo.html

Py:   sys.exit(1)
来源：http://hz.jinqigfzy.top/gthiggmclq.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtngrrjgcb.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtpyrhdrml.html

TS:   process.exit(1)
来源：http://hz.xuetiantiany.cn/gtoswavfez.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtwjrqgnnp.html

Go:   os.Exit(1)
来源：http://hz.chenlongwang.top/gtqcrtmktc.html

Ruby: exit 1
来源：http://hz.gaohongyu789.top/gtjlnmlihl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gttrhyomft.html

[M06] 向标准错误输出
来源：http://hz.ydjk.org.cn/gtopdimpqr.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangshuangyany.cn/gttyyhwvae.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gzhubu.top/gthvsobubi.html

JS:   console.error("err")
来源：http://hz.shuidangran.top/gtcuvnrncm.html

TS:   console.error("err")
来源：http://hz.birdmap.top/gttrxueyvh.html

Java: System.err.println("err")
来源：http://hz.yj20258888.top/gtqtybboks.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtswvvljxe.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gtqnisektb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangkeji.top/gtpcwgngpf.html

[M07] 判断是否为主入口
来源：http://hz.birdmap.top/gtpjfbizqx.html


<!-- 参考信息 -->