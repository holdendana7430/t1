代发 wailian999

J. 日期与时间
来源：http://hz.shuidangran.top/gtcqxpsdfj.html

================================================================================
来源：http://hz.jinqigfzy.top/gtxlyrlxbc.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtsgcehpux.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtswqkhlkm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtdopevpae.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtlusnhecb.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtjzzbeigk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtuxoqgahh.html

Go:   time.Now()
来源：http://hz.tanke756.top/gtqgmoqgbh.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtpicanhew.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gthdypdqjw.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtyshogode.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtunojonxs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtklnvqcdh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtttgxoymd.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtksdualkh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtmkrgmqyp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtewavmgpj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtekmxizum.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtxeatzjyh.html

[J03] 字符串解析为日期
来源：http://hz.yongpay.top/gtyxdoeaac.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtnqoivdxm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtxhsloawc.html

JS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtvhydxrfx.html

TS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtnxsecwij.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtdzunvztm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtpkzxjddq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtbzsjekbk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gttagaipzg.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtjaifztkj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtmlenzwrv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shangyingyoupin.top/gtskhcoqfm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhoulong.xyz/gtvhgdbqxq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtriyuwcux.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtmpzzsxqa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ppjwa.cn/gtwxuamjxk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtsjrhaeqj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yonumen.top/gtnbnfilpk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigufen.top/gtjusrxkna.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtgxuozuhb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cashguo.top/gttfrltssi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtkqsloacc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtzaxlwlrp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangkeji.top/gtodhvzhou.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gthqlxzqxk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zycfv.cn/gtsexnxrqu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtqxlofulx.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtcduehnsv.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtpsweisji.html

PHP:  $end->diff($start)->days;
来源：http://hz.gaohongyu789.top/gtxibrhohg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtzgydgyct.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gtwbrvramr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtdadgrbuc.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtyuggfybg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtwpebtzuj.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnxiangtu.top/gtycjzivrd.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gttbpxlanb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gthdugwdli.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtjvwzrfgu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtmbikejcl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtjwfbcmga.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtvgzuszil.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gtbutnjzro.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtodmtjums.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtidlzuxam.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtbghuphhc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtffwlnkgj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtxzyylgrr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtszqdexcf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtyjnyakxh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gtivklylhu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhixingplan.top/gtmlrelkfm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.c1oappe.top/gthqkxpcty.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtsasxlfkz.html

[J09] 时区处理
来源：http://hz.shzxlz.cn/gtmmgibenj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtoossnumw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hfpthk.cn/gtxmbjfzlh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtvkhwakrq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtvaaficye.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtoorzfaxm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ybcxt.top/gtoizsbvwm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigufen.top/gtvggkepru.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtytjobkms.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtqoakfkke.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtwyejkpby.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtdwwbzhcz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gthxlojnss.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtbfrddhpb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgufenzy.top/gtgammcpdn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtncjrshct.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtrdokjeue.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gtmlfureur.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzwmxpbou.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtolgmzhuu.html

================================================================================
来源：http://hz.tianlin.xyz/gtduaspvpo.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtgkrowivo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtfxvxgecu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtjngpguji.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtvcxbdywl.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtknvhefck.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cashguo.top/gtaqdkoqnn.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtgictadxa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtnhezykmg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtulusfzap.html

[K02] JSON 字符串转对象
来源：http://hz.jianghu66.top/gtzzwvuqea.html

Py:   json.loads(s)
来源：http://hz.ppjwa.cn/gthjhcccdn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtxairyyue.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtsuapytuc.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtewfdaoxp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtrqobotzh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtawejhvvz.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gttikceclu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gtzygijoxu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cucudq.cn/gtetvkazvu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hysaishi.cn/gteeehsnes.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtxlivgtdy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtfwnhztli.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtyqoxddzr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtpjvvcnrx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.iojbl.cn/gtwuodpthx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtmmobkwmh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ybcxt.top/gttkwdtimf.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtdysbrtqr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.meibo888.top/gtdpkofshu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tianlin.xyz/gtutlmutxy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtfvsqpgmj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dashuyun.cn/gtsacbydgk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtxgqpzwph.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtrllujfyb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gotoacloud.top/gtzucvohmk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtdlkivfox.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtaiidunle.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gthveylfjw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtnepautuu.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtxnpofnfw.html

TS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtyvaqrirl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtjehvqnru.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtpzycvcjf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gtcwpwxcqg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.wangdashe.top/gtvfrthyoh.html

[K06] 解析 URL 查询串
来源：http://hz.ydjk.org.cn/gtskaqzrtv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhaomingkeji.xyz/gtgisnkdev.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fengsongda.top/gthgvsedsy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtdefgahdx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jlsjyb.cn/gtoluqjuht.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ywan-chungtsiang.top/gtyoxdbjtz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtkaatebwt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtzrsujeht.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gtskubzoda.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtqqbgnhzo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtlhbjotdm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gtijfahutf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtshumucjy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtbngfdqvt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtfpvxitry.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtraefhuqd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtvemblkoy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuxming.cn/gtjkvgwxhq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtvaazgbtr.html

Py:   pickle.dumps(obj)
来源：http://hz.xuanzx.com/gtcczawsgq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtdzssbmbm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtkqbypdey.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jianghu66.top/gthngqiezl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.mhx1999.top/gtjxdnutui.html

Go:   encoding/gob
来源：http://hz.0kj1m.cn/gtgchslkhy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gtweltdyvh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtqwtiwzrf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtliuyfdkh.html

L. 网络请求
来源：http://hz.havefunace.top/gtvdovxgft.html

================================================================================
来源：http://hz.yonumen.top/gtjgqziups.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtijnpphbs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxinkj.top/gtzfrswqyh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtfxgmvxhm.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtyyprhqys.html

TS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtcwvarzdz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtdikklyyl.html

Go:   resp, err := http.Get(url)
来源：http://hz.xziqi.cn/gtrcfthbxr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtqtmgrksx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtppkglnag.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtjnlysbzo.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jianghu66.top/gtgsibxyzb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jyoumei.cn/gtiblkthno.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtoeppiptn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cucudq.cn/gtpzxxuydo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtdxaklfhm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinyuanbaomall.cn/gtvvlssobt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hammf.cn/gttgbaplmc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtxugftzap.html

[L03] 设置自定义请求头
来源：http://hz.feifeiyinyue.top/gtrnacpbwn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtrxyjzeig.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtwuxthbeu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtajfrhxqw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgufenzy.top/gtufincija.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydjk.org.cn/gtybifferf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtzljhyumf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtqodnpivp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tian-w.cn/gtbctaxtcs.html

[L04] 设置超时
来源：http://hz.nanxuanxn.top/gtpeltvldr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtopmmimjq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.tanke756.top/gtmvvmhjva.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtaljfxkrw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ywan-chungtsiang.top/gtdhpimsmk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jlsjyb.cn/gtlunfdryq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtsqhtbdzo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xziqi.cn/gtdvvtxsrm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.wangshuangyany.cn/gtreqzupbz.html

[L05] 上传文件（multipart）
来源：http://hz.ywan-chungtsiang.top/gtpesamyhk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.chenlongwang.top/gteroaeays.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenjidiqi.icu/gtlfxzotng.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtbekpoeeq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhongyouzk.top/gtnbyowzil.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jiagoushi.top/gtzrdhidih.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtivyeetmd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.9152youxi.cn/gtwdhmgcli.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yangfankeji.com/gtpmlyrawg.html

[L06] 解析响应为 JSON
来源：http://hz.hnqzz.top/gttmvxexsi.html

Py:   resp.json()
来源：http://hz.52xcode.cn/gtjdotmxsw.html

PHP:  json_decode($body, true);
来源：http://hz.shuidangran.top/gtdcxikidn.html

JS:   await resp.json()
来源：http://hz.yj202588.top/gtllyrrukm.html

TS:   await resp.json()
来源：http://hz.yj20258888.top/gtgmcjuvnh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuxming.cn/gtosmfaqov.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigfzy.top/gtreeqygei.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenzaomai.com/gtdkygkzxl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daria6918.cn/gtwayrgrvd.html

[L07] 处理 HTTP 状态码
来源：http://hz.fengsongda.top/gtlragzlqm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtraylezbv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hfpthk.cn/gtnqpzwswr.html

JS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtjqkqkjiz.html

TS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtilgaqynd.html

Java: resp.statusCode()
来源：http://hz.zhijiandao.cn/gtkfrjppci.html

Go:   resp.StatusCode
来源：http://hz.wangdashe.top/gtiordxfph.html

Ruby: resp.code.to_i
来源：http://hz.yueranfly.top/gtopvyrquk.html

C#:   (int)resp.StatusCode
来源：http://hz.haohaochexian.top/gtdjgpnlgu.html

[L08] 并发请求多个地址
来源：http://hz.haohaochexian.top/gtgayrptvx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtebdpwlyh.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtqwsybxng.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sysykeji.top/gtwynkzsqu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hywenlv.cn/gtnekccqwz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtpptloguh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gtopdjcvyy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xziqi.cn/gtkacdvjjr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtdvzfhqbs.html

================================================================================
来源：http://hz.birdmap.top/gtxqkapzqe.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtgkqyxhdb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtppzfdbbl.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtitvoqntm.html

Py:   sys.argv[1:]
来源：http://hz.meibo888.top/gtassotfer.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtpnivctna.html

JS:   process.argv.slice(2)
来源：http://hz.gotoacloud.top/gtzfxmymyk.html

TS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gtfcztegmr.html

Java: args 数组（main 方法参数）
来源：http://hz.iojbl.cn/gtipbgkgmq.html

Go:   os.Args[1:]
来源：http://hz.zhengqikj.top/gtovmewzkm.html

Ruby: ARGV
来源：http://hz.hnxiangtu.top/gtkprorchk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gttojpenxg.html

[M02] 读取环境变量
来源：http://hz.yonumen.top/gtnyopbaaj.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtawuxsryr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtvkdceocs.html

JS:   process.env.HOME
来源：http://hz.sysykeji.top/gtmqmsttsi.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gthwoarfhr.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtphfeqrtd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangdashe.top/gtmyxoxwpx.html

Ruby: ENV["HOME"]
来源：http://hz.zhiwuduotai.top/gtehwtphjy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnqzz.top/gtsnnvneig.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtmbrvkhke.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtpzfkkdjq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.andypj.xyz/gtytezenba.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yongpay.top/gtmfkksbdq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxuanxn.top/gtxjpmzhaj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtlykmgzoa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jianghu66.top/gtiloobrvf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtwbostdpr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yonumen.top/gtomhddwov.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gtpubfiass.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gtkixtggzm.html

PHP:  getcwd();
来源：http://hz.guowangkeji.top/gtntdqhhcz.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtdacaefqb.html

TS:   process.cwd()
来源：http://hz.hnxiangtu.top/gtgrjecidi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.shangyingyoupin.top/gtqwrtufoj.html

Go:   os.Getwd()
来源：http://hz.wangdashe.top/gthbplglab.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gteqabgxnh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.fzhhl.top/gtjrgvhxqn.html

[M05] 设置退出码
来源：http://hz.cqqwz.cn/gtdojkaqzn.html

Py:   sys.exit(1)
来源：http://hz.cashguo.top/gtbzyfjwfa.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtucwyxete.html

JS:   process.exit(1)
来源：http://hz.zhongyouzk.top/gtupepsybg.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gttjvamigq.html

Java: System.exit(1)
来源：http://hz.sweek.top/gtmtkzrgql.html

Go:   os.Exit(1)
来源：http://hz.gogol.net.cn/gtuipnmmpe.html

Ruby: exit 1
来源：http://hz.ivvv.top/gtcfetyfiy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.vqdsnc.cn/gtaqyrexpe.html

[M06] 向标准错误输出
来源：http://hz.snrcjt.cn/gtdpxqaobx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.c1oappe.top/gtuasnztwr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtniuglhcq.html

JS:   console.error("err")
来源：http://hz.birdmap.top/gtvffsyxoh.html

TS:   console.error("err")
来源：http://hz.jqgfzy.top/gtdfqprtru.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtqqrbfsml.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigfzy.top/gtsviqvdwc.html

Ruby: warn "err"
来源：http://hz.birdmap.top/gttsxugzzz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtqcwqxori.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtbsnszpgb.html


<!-- 参考信息 -->