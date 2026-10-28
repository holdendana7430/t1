代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtnlkzfqgp.html

JS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtxntqazsx.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtzbmcywji.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gaohongyu789.top/gtpemidkpk.html

Go:   time.Now()
来源：http://hz.jlsjyb.cn/gtlfboyiqe.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtyihqojvd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtesjtfxby.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gtmlleqxwl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtsmytvnvc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtwaukddxt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtsvrhgabn.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtcikfxoob.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtcidwfkia.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtwjmqzzlx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtzntxewoe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtacsbovqi.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gthzajrgbe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtpuzxylzl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yangfankeji.com/gtorvqmdqz.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtuzxnuoii.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtncmvecro.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtvxfkqdwc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yongpay.top/gtbeujhaqf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtuaocivpz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtatekxyoq.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtgkqoxfmr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gthlfioxph.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtncmuxjcy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtbugkhixq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gttroksfmj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gttcxqeoqh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtgpmvnple.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtbopaivde.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtkitixfdz.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtmnytuoao.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtpsdezcvr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yonumen.top/gtmnmowuzo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtafcetndo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gthvrdzmxg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtpoulvohi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gtuamrutts.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtadatifou.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtbvqxqblp.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gtytsowwvw.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtprjvyjov.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtskwqegmj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.redwolf501.top/gtihhnjjlm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shzxlz.cn/gtkbwhikih.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtomhnmade.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtknlxmoam.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtpnipbrmy.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gtvxzojfiy.html

[J07] 比较两个日期
来源：http://hz.jinqigufen.top/gtaedafwzh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtsjluvfth.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtwfzvqzql.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtbmgapwrg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtjzvisipj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gteyqozqdi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtmhnhucgm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtifnjoabi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jlsjyb.cn/gtwecfflzh.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtihnowpts.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ybcxt.top/gttenhyhlw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydzc1.top/gtiahhbydp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtqounbzww.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtymyvcxdq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtxeamjtuk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gttweiagmz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhixingplan.top/gtpypwxtgz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtkyikixob.html

[J09] 时区处理
来源：http://hz.pengpengdd.cyou/gtmjjwsrva.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtwihfkfmd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtlcrkmvmt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtwmvlbmfr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtrrhcnfbn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtpoxtsaby.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jlsjyb.cn/gtbfmauipz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtikplhjgx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtgabtakpz.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtaptskzgq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yonumen.top/gtnkuzafzn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinghuilouyu.cn/gtevlrtzqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtwedfqmcy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gtyhbizhsc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtinnrjmxh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ivvv.top/gtsilbbbxa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtumeqxmhx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtwcrhjmev.html

================================================================================
来源：http://hz.yanxiufei.cn/gttmzkiyhk.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gtmanpnluf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtmklvotpb.html

[K01] 对象转 JSON 字符串
来源：http://hz.tanke756.top/gtqimyevia.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtbdtvnrfv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtvdefgqha.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtrjxhwlag.html

TS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtsufhajcs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtwxojfwof.html

Go:   json.Marshal(obj)
来源：http://hz.sufxvd.cn/gtcjnacdnl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinyuanbaomall.cn/gtbtxfohev.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtsvwofvse.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258888.top/gtrxsjhfwc.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtqsmwoyvj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtairlxkql.html

JS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtnhtmhtrc.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtnyijrbee.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenzaomai.com/gtannfproi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zycfv.cn/gtvijvmrik.html

Ruby: JSON.parse(s)
来源：http://hz.cqqwz.cn/gtaihdjsfd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gtvbkbtsyp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cdnleiting.top/gtwgreaqfc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtjhytgrfe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtfjnfpaqq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtudywqtsd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtiatzrapg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtnufvbptx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtvyfenmji.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gttgxqyyio.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtlcaevpff.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtczvmdcoa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtrssobmld.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.quarkkingdee.top/gtpnpnlgpx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinyuanbaomall.cn/gtneyzyvnd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtsludakek.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtepdkhfbv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtpjzmgvvp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtbogtjjqw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtflatvbus.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtbnydzwdv.html

Py:   copy.deepcopy(obj)
来源：http://hz.svipenyu.cn/gtnksuszqi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gtcbipnpqt.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtraakevsp.html

TS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtyqqqpbxw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtilwdnuii.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtswxsjkll.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtvbugjsbc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dianchejie.cn/gtfrmgonid.html

[K06] 解析 URL 查询串
来源：http://hz.jlsjyb.cn/gtpvrqltzl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sufxvd.cn/gtdpkbmoom.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xingfuxueyuan.xyz/gtwhudccsu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtwmffbdmy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtqgeajzkr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtpvmpbrpl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtavfzpckd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtdzitnjhm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.birdmap.top/gtfpolocfp.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtkzqfvksp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinqigufen.top/gtaryeovjb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zycfv.cn/gtbaebynqh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtrypyofzr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtldffbuob.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtcxhntrig.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtnwnhrccr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.aizwys.cn/gtysteiilu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhengqikj.top/gtaxxocrjl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gtenbnwsoa.html

Py:   pickle.dumps(obj)
来源：http://hz.sysykeji.top/gtiedinofv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtdxvglwou.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zdqjudy.top/gtcjxfzemk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hywenlv.cn/gtauugitmn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gtkptujexz.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtizvpbzul.html

Ruby: Marshal.dump(obj)
来源：http://hz.316326.xyz/gtzdfvotsj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtiojbozgn.html

================================================================================
来源：http://hz.zhijiandao.cn/gtrdwmgkkc.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtmcpmxsly.html

================================================================================
来源：http://hz.andypj.xyz/gtekkttivs.html

[L01] 发送 GET 请求
来源：http://hz.xziqi.cn/gtpvcahenl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hywenlv.cn/gtutjybpsn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtqvvipdge.html

JS:   await fetch(url)
来源：http://hz.jinyuanbaomall.cn/gtlrpuuylb.html

TS:   await fetch(url)
来源：http://hz.yueranfly.top/gtvdkudqoo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tian-w.cn/gtohhryqgb.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtryobdzmi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.meibo888.top/gtvzxkwxwe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhijiandao.cn/gtgnqrwjln.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtefjafhqc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shanyushiyangkeji.top/gtoibzkfjc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtuqnvyozi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtopbkkxil.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtgqeuxqul.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuxming.cn/gtdyrsijuw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.tanke756.top/gtignnaozo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gtaelzuchk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jianghu66.top/gthshdrfhe.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtsdzmzyao.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shanyushiyangtech.top/gtyzyigceo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtfqaskzle.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtceuwydma.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gttwuuobld.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.guannengcc.top/gtedzmxalv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtwahquygs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jianghu66.top/gtcxkoojua.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.mhx1999.top/gtyltvqttc.html

[L04] 设置超时
来源：http://hz.zhixingplan.top/gtyuoqprrv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yanxiufei.cn/gteswgmjce.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xinyue.icu/gtgghuvmnr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtkhsqvefp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shuidangran.top/gtzzlgtvlp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.c1oappe.top/gthoxoufvi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtzuspfwwq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gtqhyayjir.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jiagoushi.top/gtzdpyxljl.html

[L05] 上传文件（multipart）
来源：http://hz.sufxvd.cn/gtowwfqeak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtksuqglcq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtqorgcvbd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fengsongda.top/gtlmqhwrgg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtpgxdotak.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtsvwlrurn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yongpay.top/gthzqctzhk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.gaohongyu789.top/gtgwqfmsmn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.gzhubu.top/gtohogqqoz.html

[L06] 解析响应为 JSON
来源：http://hz.dianchejie.cn/gtsgxpttld.html

Py:   resp.json()
来源：http://hz.shuidangran.top/gtswipqtrk.html

PHP:  json_decode($body, true);
来源：http://hz.shzxlz.cn/gtgaumhluv.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtliwfwdgv.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtvtqspbwi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtmbbtyxfw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhoulong.xyz/gtwvrdjgqq.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fzhhl.top/gtnsmyozxp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtfcyrueoa.html

[L07] 处理 HTTP 状态码
来源：http://hz.jyoumei.cn/gtziffbvas.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhijiandao.cn/gtlkdswesd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxinkj.top/gtkijmlckn.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtbowijftl.html

TS:   resp.ok;  resp.status
来源：http://hz.shuidangran.top/gtskrqtkpl.html

Java: resp.statusCode()
来源：http://hz.zhiwuduotai.top/gtnszfqhtx.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtdazbstqi.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gtwvrndwye.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtmwhoioep.html

[L08] 并发请求多个地址
来源：http://hz.hywenlv.cn/gtzyiwihwb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtgekkrhkv.html

PHP:  curl_multi_init() 系列
来源：http://hz.dianchejie.cn/gtzmdphvng.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ehwqpu.com/gtveufjsgu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtewtgrcfn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ywan-chungtsiang.top/gteymdlagh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.havefunace.top/gtmtiamcsy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.svipenyu.cn/gtwbqcpkgz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.aibaodan.cn/gtnmlaafdx.html

================================================================================
来源：http://hz.shuidangran.top/gthpwgikvb.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxuanxn.top/gtqyupdnxu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtswxecwbh.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtsiaimsms.html

Py:   sys.argv[1:]
来源：http://hz.mhx1999.top/gtfzhwumye.html

PHP:  $argv;  $argc;
来源：http://hz.hongshengwenyu.top/gtmfvntvjb.html

JS:   process.argv.slice(2)
来源：http://hz.zhiwuduotai.top/gtzbwpbmzf.html

TS:   process.argv.slice(2)
来源：http://hz.0kj1m.cn/gtqvambjli.html

Java: args 数组（main 方法参数）
来源：http://hz.xingfuxueyuan.xyz/gtlongrmht.html

Go:   os.Args[1:]
来源：http://hz.jinqigufen.top/gtyreyscov.html

Ruby: ARGV
来源：http://hz.xinyue.icu/gtsuqmbnyx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.meibo888.top/gtkpeiqmsp.html

[M02] 读取环境变量
来源：http://hz.zhongyouzk.top/gtoymaaeoz.html

Py:   os.environ.get("HOME")
来源：http://hz.cashguo.top/gtpixijboe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fengsongda.top/gtkkhstzlo.html

JS:   process.env.HOME
来源：http://hz.feifeiyinyue.top/gttfxohqpn.html

TS:   process.env.HOME
来源：http://hz.ivvv.top/gtjuvypnmc.html

Java: System.getenv("HOME")
来源：http://hz.zhiwuduotai.top/gtqeiqgvhi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj202588.top/gtizsettde.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gttfbtgigt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guowangkeji.top/gthhvoxdtv.html

[M03] 执行外部命令
来源：http://hz.havefunace.top/gtukjhelns.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gtgcudblox.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yangfankeji.com/gtmwqihikq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhongyouzk.top/gtzjdiwohd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtnrmplpcy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hfpthk.cn/gtglfwjfsp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtpygyjsxn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hongshengwenyu.top/gtzwixpmul.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtwdadguka.html

[M04] 获取当前工作目录
来源：http://hz.tianlin.xyz/gtgmakfifa.html

Py:   os.getcwd()
来源：http://hz.nanxuanxn.top/gtskiezbid.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtorsijlhk.html

JS:   process.cwd()
来源：http://hz.yj202588.top/gtibqysdgc.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtdgwvxxuo.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtzoplteta.html

Go:   os.Getwd()
来源：http://hz.yj202588.top/gtajutmdzj.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtdtzqolhj.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinqigufen.top/gtgezyotll.html

[M05] 设置退出码
来源：http://hz.aibaodan.cn/gtohmdfozi.html

Py:   sys.exit(1)
来源：http://hz.kuanghao11.cn/gtoilmkryq.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtwnydxcxh.html

JS:   process.exit(1)
来源：http://hz.jinghuilouyu.cn/gtxioydpso.html

TS:   process.exit(1)
来源：http://hz.hammf.cn/gtqqgskdqz.html

Java: System.exit(1)
来源：http://hz.andypj.xyz/gtuqcljjtt.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtfmcioyqy.html

Ruby: exit 1
来源：http://hz.sufxvd.cn/gtqvhjsozk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.fengsongda.top/gtnyvegroo.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtfalcfbyp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtadffgzem.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shuidangran.top/gtfmxkkmpj.html

JS:   console.error("err")
来源：http://hz.yonumen.top/gtfhvlcqba.html

TS:   console.error("err")
来源：http://hz.tian-w.cn/gticiukzzd.html

Java: System.err.println("err")
来源：http://hz.sxryk.cn/gtkarbgoty.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.daxiang520.top/gtfwyhttyu.html

Ruby: warn "err"
来源：http://hz.ydjk.org.cn/gtyezstwyi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sufxvd.cn/gtntoezwyk.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtgzovvfsq.html

Py:   if __name__ == "__main__":
来源：http://hz.jinghuilouyu.cn/gtgegdqiaz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.dianchejie.cn/gthjuywuhz.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtkhsaftzd.html

TS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtizckrjdz.html


<!-- 参考信息 -->