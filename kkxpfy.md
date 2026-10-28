代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtvfjfjedf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtzuthrtds.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtqsuwtboi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtthtfdwww.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gtwwuksshc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gthrlpusxp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtmdfeayyg.html

JS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtvihnchhr.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtaeajpthm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtxkeuxrmc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtioqnhrte.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtyzjvxqza.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtlkwrmxfa.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gttudkxdtx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtapajtltw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuanzx.com/gtpetfnbxg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fengsongda.top/gtgrqbasux.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhoulong.xyz/gtxxpfrejv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gtuflsonne.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtoagajnka.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.meibo888.top/gtpyamzcwf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gttfkphkou.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtymymernc.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gthldualqi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtqctfjmvo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtsavrumzx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtvonfwcmd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ehwqpu.com/gtdcfmicwy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtdyoqpoyh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtqldzgsbi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gteccetgwu.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtuwkcmffr.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gteccdqmbq.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtzixnowad.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gthjimvozg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtwjyodgoy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtubxniavj.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtssbpyvpf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gtyuippdnu.html

C#:   (end - start).TotalSeconds
来源：http://hz.fengsongda.top/gtxgwdubkk.html

[J07] 比较两个日期
来源：http://hz.zhaomingkeji.xyz/gtjytunnfz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtsgwckusi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yonumen.top/gtvffhqwgl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtfqpyxpjt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtktdvjfzn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtpnwrvjpi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtzpolwruq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtkgichjqz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtmhlsjlom.html

[J08] 提取年月日与星期
来源：http://hz.c1oappe.top/gtvqmkoukb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtfgxdtoxh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ybcxt.top/gtoficcgaw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dianchejie.cn/gtwdnrceix.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258.top/gtnslbekpa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.9152youxi.cn/gtdfyfvdlb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtfwonwqsz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.iojbl.cn/gtagoiwqwv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtcnzeyhqt.html

[J09] 时区处理
来源：http://hz.yongpay.top/gtxjayfhdj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtiidsezza.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtgazboqcl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtpemkgmsz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtgqbevohz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtfclejpzu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtheeqihyk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtnnratmdi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gthfibttqq.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtnsfvtkvw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtnvrcynin.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sweek.top/gtopkjvepj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtmkbqtkvg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtbwtnardc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtjpxahrsh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgfzy.top/gtasbdvnjt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtwrgctimg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtdtziaqkg.html

================================================================================
来源：http://hz.zhijiandao.cn/gtciewkybj.html

K. JSON 与序列化
来源：http://hz.tianlin.xyz/gtwwzktynx.html

================================================================================
来源：http://hz.meibo888.top/gtgujgpbak.html

[K01] 对象转 JSON 字符串
来源：http://hz.daria6918.cn/gtrhkdstih.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtvsqaeovc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtyrhurgqm.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtzvdhawrj.html

TS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtcfoqgbib.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtbzqduajz.html

Go:   json.Marshal(obj)
来源：http://hz.0kj1m.cn/gtnhaixaqs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtoazxftkw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.svipenyu.cn/gtifjijpyt.html

[K02] JSON 字符串转对象
来源：http://hz.redwolf501.top/gteukxjlqz.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtjubrdhrm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgufenzy.top/gtgzhagcow.html

JS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtrgcnoatl.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gttjjbecbn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtyyjjmydo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtuigzmgjf.html

Ruby: JSON.parse(s)
来源：http://hz.fengsongda.top/gtvnomdxrd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtmpxktzay.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtjsiuunia.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtrdpzbokw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtrezinmbs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtqtqbsjkl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtcanamlal.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtgfiqlkxc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtwdirubxx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtpxaularv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gthygffblb.html

[K04] 读取 JSON 文件
来源：http://hz.jlsjyb.cn/gtjmgyfrxc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hongshengwenyu.top/gtyrzbzkmd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtfxkfnlyr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtyxgniela.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtgqhwjkgr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jlsjyb.cn/gtnuxlcsus.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtskymapdu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.birdmap.top/gtxcanjqek.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtkesfqvls.html

[K05] 深拷贝对象
来源：http://hz.chenjidiqi.icu/gthhaafryu.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtejizudcb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xingfuxueyuan.xyz/gtwoervwhh.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtrpstzmfv.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtxqnkifft.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtvttvcive.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtmbjrhxat.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangdashe.top/gtspgpnbhe.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtnavvmhit.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gtsuguinln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtljprcgpu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangshuangyany.cn/gtppwnqudx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gttiedatco.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtyifnzzja.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ppjwa.cn/gtpnlovlkf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtvwamrpfo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtxfxqgovn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangkeji.top/gtwcafehqj.html

[K07] 进制转换
来源：http://hz.yonumen.top/gtziermrad.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtexrntlyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtfmcddrdu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtskvpgwxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gthslnphsw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtginchqwp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.9152youxi.cn/gtcgwaqnki.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.andypj.xyz/gtcurddgks.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtueuxfjge.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jyoumei.cn/gtnfvetqkw.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangtech.top/gtmpuzvowf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gtyouosdrj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gteztsgfwo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.aizwys.cn/gtofpdsmlq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gtfbzrmdbu.html

Go:   encoding/gob
来源：http://hz.aizwys.cn/gtravncxkg.html

Ruby: Marshal.dump(obj)
来源：http://hz.snrcjt.cn/gturrmapwr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtcrxuxxbv.html

================================================================================
来源：http://hz.jqgfzy.top/gtoxgdriqm.html

L. 网络请求
来源：http://hz.gzhubu.top/gtkdpxiifk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmnaocskn.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtqbbjnbsi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtfurnuzpi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gtisyavenl.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtqrnntsch.html

TS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtmyndghmc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuetiantiany.cn/gtnkaqwzza.html

Go:   resp, err := http.Get(url)
来源：http://hz.andypj.xyz/gtqarsfdro.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jianghu66.top/gtojwphzzm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj20258.top/gthytwayat.html

[L02] 发送 POST JSON
来源：http://hz.hnxiangtu.top/gtiluprreu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hywenlv.cn/gtnxhlpmui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtmpaxmwkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtbtsotpkk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtrtgnrfhg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gtyigaxsbo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gtbjsdrbvh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtggxqfgek.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.feifeiyinyue.top/gtdcwnbfzv.html

[L03] 设置自定义请求头
来源：http://hz.ehwqpu.com/gtjgacvgnf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtfhstowey.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xziqi.cn/gtmvzwqbsf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtxjyjopvq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtaktlidkh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtaobnfcey.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtsvydzyfn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinghuilouyu.cn/gtkfwjzxkm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangdashe.top/gtxejgdjzg.html

[L04] 设置超时
来源：http://hz.gaohongyu789.top/gtramiryxk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtghjlfbid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gthxkhawcx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtrnfngwlu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtwcgtwqdh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.aibaodan.cn/gtpvnlmgus.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinghuilouyu.cn/gtzcimrtlo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aibaodan.cn/gtrkhunsck.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guowangkeji.top/gtydnfumaq.html

[L05] 上传文件（multipart）
来源：http://hz.ybcxt.top/gtsxqyatms.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtcvhsojyq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yj202588.top/gtllyfksko.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.aibaodan.cn/gtcwclekel.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtyemryxuq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hongshengwenyu.top/gtpcngjarn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtdalguype.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtkrtyufwh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenlongwang.top/gteppnnkzu.html

[L06] 解析响应为 JSON
来源：http://hz.chenlongwang.top/gtqbqvydhj.html

Py:   resp.json()
来源：http://hz.hammf.cn/gtdjxnypxd.html

PHP:  json_decode($body, true);
来源：http://hz.sweek.top/gtndozvyag.html

JS:   await resp.json()
来源：http://hz.ivvv.top/gtevkyhbfs.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtxcshquep.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jianghu66.top/gtnvnonsgc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhiwuduotai.top/gtqbpktagd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gttbqogjig.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtglxoaxxw.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtahlqujhw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.bjfxy.top/gtzavxqrfw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtxfipsmxn.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gttffyqplu.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtbieqztja.html

Java: resp.statusCode()
来源：http://hz.pycfn.com/gtgwbjwlln.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtrtegkhbw.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtjcbdxzbn.html

C#:   (int)resp.StatusCode
来源：http://hz.snrcjt.cn/gtriuznpbl.html

[L08] 并发请求多个地址
来源：http://hz.snrcjt.cn/gtnhypozcw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtyovrzotl.html

PHP:  curl_multi_init() 系列
来源：http://hz.fengsongda.top/gtyafuzymr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtegrzplba.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.vqdsnc.cn/gttrgjndds.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtixdddxlz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shanyushiyangtech.top/gtfbfwkdyj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtdxugafzv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gzhubu.top/gtuyilcmww.html

================================================================================
来源：http://hz.dianchejie.cn/gtnwezaynk.html

M. 命令行 / 进程 / 环境
来源：http://hz.daria6918.cn/gtpiahdnhe.html

================================================================================
来源：http://hz.yueranfly.top/gtkioctgat.html

[M01] 读取命令行参数
来源：http://hz.yangfankeji.com/gtjyslherx.html

Py:   sys.argv[1:]
来源：http://hz.yanxiufei.cn/gtfkwsdtnf.html

PHP:  $argv;  $argc;
来源：http://hz.ydzc1.top/gtanauuwlm.html

JS:   process.argv.slice(2)
来源：http://hz.xingfuxueyuan.xyz/gtnbxwabmi.html

TS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtbucjbrqf.html

Java: args 数组（main 方法参数）
来源：http://hz.fzhhl.top/gteemcirxv.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtkatnuskp.html

Ruby: ARGV
来源：http://hz.guannengcc.top/gtcyhafepx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ydzc1.top/gtbfjazpay.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtdiacqyxh.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtgjwplmyz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtwabnygtt.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gtiarqixhw.html

TS:   process.env.HOME
来源：http://hz.jqgufenzy.top/gtzrhxwlzo.html

Java: System.getenv("HOME")
来源：http://hz.cqqwz.cn/gtginvczde.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.guannengcc.top/gtutbyztzd.html

Ruby: ENV["HOME"]
来源：http://hz.chenzaomai.com/gtdezmdqzs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtifkdhwyw.html

[M03] 执行外部命令
来源：http://hz.ywan-chungtsiang.top/gtpqmugfmz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtgyutiewf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtztjeiifn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gtgxhwomny.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtqnloazoz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtjzvptvtg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jyoumei.cn/gtgjposjge.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtdmtajfns.html

C#:   Process.Start("ls", "-l");
来源：http://hz.xylfe.cn/gtufgavwpf.html

[M04] 获取当前工作目录
来源：http://hz.mhx1999.top/gttedlskqk.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtmgfhtodq.html

PHP:  getcwd();
来源：http://hz.yuxming.cn/gtxdzbyreq.html

JS:   process.cwd()
来源：http://hz.cashguo.top/gtsjtdveoe.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtysnujxps.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.daria6918.cn/gtaqkrglyo.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtmsvcvxmh.html

Ruby: Dir.pwd
来源：http://hz.nwbrower.top/gtcifchzkd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.guannengcc.top/gtjhgchhpg.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtxwowiifx.html

Py:   sys.exit(1)
来源：http://hz.quarkkingdee.top/gtnnlyllvn.html

PHP:  exit(1);
来源：http://hz.zhongyouzk.top/gthfvtkhjl.html

JS:   process.exit(1)
来源：http://hz.9152youxi.cn/gtxwnjdmus.html

TS:   process.exit(1)
来源：http://hz.fzhhl.top/gtdjqqndds.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gthlbesczw.html

Go:   os.Exit(1)
来源：http://hz.jinghuilouyu.cn/gttsinzcep.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtavtyfqrn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.gogol.net.cn/gthjtteodf.html

[M06] 向标准错误输出
来源：http://hz.zhiwuduotai.top/gtxppckycs.html

Py:   print("err", file=sys.stderr)
来源：http://hz.andypj.xyz/gthpmuswsf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtcgqfczon.html

JS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gteetkntgt.html

TS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtctewuibt.html

Java: System.err.println("err")
来源：http://hz.ydzc1.top/gtlquvcugc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zdqjudy.top/gttgqqnbiy.html

Ruby: warn "err"
来源：http://hz.shanyushiyangkeji.top/gtomaqmweu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtnhtfdeny.html

[M07] 判断是否为主入口
来源：http://hz.gaohongyu789.top/gtatznihjw.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtxfiohzin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtzghslucu.html

JS:   require.main === module
来源：http://hz.zhengqikj.top/gtxilnzikp.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtgswrqwzk.html

Java: public static void main(String[] args)
来源：http://hz.jinghuilouyu.cn/gtplbslzvg.html

Go:   func main()
来源：http://hz.dianchejie.cn/gtscxvmzak.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtkbhyofle.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtymzaclrd.html

[M08] 获取系统与运行时信息
来源：http://hz.pengpengdd.cyou/gtzpvpajph.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gttobbuctv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.shangyingyoupin.top/gtvmyqagbc.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtvspcjqhg.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtbxqqjdcp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yvedp.cn/gtvjgglhbh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtsxsppjxl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.xziqi.cn/gtiudpdnso.html


<!-- 参考信息 -->