代发 wailian999

J. 日期与时间
来源：http://hz.xylfe.cn/gtthpjorrq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtepcfyoia.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtfvdjibyr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtefteaojf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtvqhmvokc.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtbesjxdwr.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtnghyyxdk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtwqeflieu.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gthotzxolf.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtlgeylwbt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtctvhgmgh.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gthxvgjeeg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhiwuduotai.top/gtzlrmfwsg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtsvlrikwl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtlcccepwx.html

TS:   d.toISOString()
来源：http://hz.yuanzhike.top/gtwgrxkhrd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtrcnigybn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtlooeqarz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.mhx1999.top/gtkdvjzysn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ybcxt.top/gtgrzgrcls.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gthjtfzqxe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj202588.top/gtoboywubh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtyjsinukj.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtumfffvxx.html

TS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gttkkdbuod.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtbsxrltlg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gttvkkbkfu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtojylycmb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gogol.net.cn/gtbjgxpogq.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtstghqzhx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtcfzjvpdl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtfpsctorp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinyuanbaomall.cn/gtwuaqmsth.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258888.top/gtjkxkarzc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtpalncofz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtixfvksvy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtzrkjpdhu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtjwemmocd.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gtfeymkzok.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtindikxtb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj202588.top/gtefzcvjkt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtgquqveza.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtgmofieoi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jlsjyb.cn/gtlwmzxrfg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtwrmzxspl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtfqsfooxq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gthvtfiyrt.html

[J06] 计算两时间之差
来源：http://hz.pycfn.com/gtmbqkiceg.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtwrmrjnsz.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtvuvkfxox.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.iojbl.cn/gtdobvfgcr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.52xcode.cn/gtmlyrqziz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydzc1.top/gtiozelkwu.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtyteylevz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtfhdplfbl.html

C#:   (end - start).TotalSeconds
来源：http://hz.shangyingyoupin.top/gtogeskwxh.html

[J07] 比较两个日期
来源：http://hz.tanke756.top/gtbzrgfsol.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtmqanfjwj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtrmgxublq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pengpengdd.cyou/gtndryqsvb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtaodvyict.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtazldqqpx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ywan-chungtsiang.top/gtjrzjraku.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtmbvkfbug.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtqguylcdk.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtwhxxodyd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.wangshuangyany.cn/gtkpnkdxjg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gttmuleqoa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtvkyrcspp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gttaobnhhw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtyciuhcdh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtvoasnmpj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tanke756.top/gtdcwyxueg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtxdmyqntm.html

[J09] 时区处理
来源：http://hz.jiagoushi.top/gtwdlszmfc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtpwgorrfk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtlfvoabfh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtsdcdtits.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtioorrhwk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhaomingkeji.xyz/gtrquxwghu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtwqzlyhsn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtomrdzfsq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtcjrepkyo.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtaaogpreb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtrkmpfibt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtvqycozyv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jyoumei.cn/gtwmdvhgys.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtxkrbhoyt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gtgzvyxmol.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zdqjudy.top/gtfwsniudq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtwbhhgjbj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhongyouzk.top/gtkcmvgitb.html

================================================================================
来源：http://hz.cashguo.top/gtwmilmmld.html

K. JSON 与序列化
来源：http://hz.sxryk.cn/gthsejmegt.html

================================================================================
来源：http://hz.zdqjudy.top/gtmlmtqwet.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gtihqzevrv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gttbjxtnoq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtwgbjmreg.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtzcloodrf.html

TS:   JSON.stringify(obj)
来源：http://hz.xuetiantiany.cn/gtqnvgdmwp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtuhmtpyna.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtgncviidy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtdfqyhwaf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtyppnjuzy.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtiqiboncj.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtftscohbo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yvedp.cn/gtgyfghbwq.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtmpitmmze.html

TS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtvrypiefs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.redwolf501.top/gtgahyciqs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtjigzrdty.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtzgurimxw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtndwujfwl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.chenlongwang.top/gtanfyhjbt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtygrxvrld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtbekfvxuw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gttrstnila.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtwtuxpnxw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jyoumei.cn/gtxszgmqdd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtghwizgdw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtsfdzivbj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtdoypsklo.html

[K04] 读取 JSON 文件
来源：http://hz.hnqzz.top/gtdzxqqdtq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtnbzyvfcq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtmknycwpu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtfjxughpx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtnoyzbzno.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258888.top/gtlubptxyr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtsunghepb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtwlrrpedx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtkvteauzd.html

[K05] 深拷贝对象
来源：http://hz.jianghu66.top/gtvukgurkd.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhiwuduotai.top/gttfwjpyvg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258888.top/gtrymhboau.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtvmdfezpq.html

TS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtjtbnvscx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtyjfsjrlk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nwbrower.top/gtyavbzvjc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtrubtjucm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtnbccqqab.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtxzixjxzb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtxycbpjpn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtpvyiqyal.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtnphlrrcy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtcdwsnweu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtmkgauijw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtitmfvuss.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtsoidbror.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fzhhl.top/gtlrdmucki.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtybirydqj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenlongwang.top/gtxhkpsfmg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuanzhike.top/gttilpjmmc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtaxsthefk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtttdbkxms.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtdqmnhjzr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtztlokwqi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xylfe.cn/gtuodkqkwr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangshuangyany.cn/gtgmqydmgo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtdudwwweh.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtyratazoo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtuqmlfuns.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtbeuuhuqx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtfjymlsmr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tian-w.cn/gtypqheamp.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtnrpdmsat.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtvehenmzx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gttrkqjdrf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtktdtazol.html

L. 网络请求
来源：http://hz.cheryme.top/gtwkwppsvk.html

================================================================================
来源：http://hz.mhx1999.top/gtkxtlhnaz.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtcatdqjdo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtbubsnrfx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtgobdgpfh.html

JS:   await fetch(url)
来源：http://hz.hfpthk.cn/gtrcbhypby.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtfukrgupj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtxkqnwbyk.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtbwytdtil.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cheryme.top/gtzuqsmuym.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aibaodan.cn/gtaqodurid.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gtexdewcvd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dianchejie.cn/gtkbdcpagw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.chenjidiqi.icu/gtpinrhgly.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtqllyrxtm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtcwzqbyqv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jianghu66.top/gtcbmatkuk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhoulong.xyz/gtkrxucgvy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.316326.xyz/gtsmlhitia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258888.top/gtsumzchhw.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtmyapegdf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hongshengwenyu.top/gtfvfagcya.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinghuilouyu.cn/gthbpxmjud.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daxiang520.top/gtzzqpkady.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtsodllftd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gtihszvcfe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gtwiwznkqi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.feifeiyinyue.top/gtxfpunawy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhoulong.xyz/gteamqzpae.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtsgbereaf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtehvnekwo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtdyovsizj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtjnhyfjrt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtvfiivzgc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sweek.top/gtwragmyai.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtzipuraln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtabsflfpc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jlsjyb.cn/gtdyxomoac.html

[L05] 上传文件（multipart）
来源：http://hz.xylfe.cn/gtkanscxmx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gtwmcpavwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gtykrpsrdj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuanzx.com/gtqhkxvfnl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtzryomshd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gthlggtmsc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydzc1.top/gtbefhxdxv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yongpay.top/gtztztpswu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gthqxwwpnn.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtdmbkekup.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtnqoxnrkq.html

PHP:  json_decode($body, true);
来源：http://hz.zhoulong.xyz/gtsjccceas.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtshpkvlus.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtfoyfiwgw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtyhwepzdu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtnzzjifnw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.pengpengdd.cyou/gtclmlxata.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tian-w.cn/gtswwbtizd.html

[L07] 处理 HTTP 状态码
来源：http://hz.316326.xyz/gtcfwpkgct.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yangfankeji.com/gtkffazjsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtjwxziugb.html

JS:   resp.ok;  resp.status
来源：http://hz.hfpthk.cn/gtvmginhqw.html

TS:   resp.ok;  resp.status
来源：http://hz.mhx1999.top/gtupykdcma.html

Java: resp.statusCode()
来源：http://hz.quarkkingdee.top/gtrijkuwes.html

Go:   resp.StatusCode
来源：http://hz.birdmap.top/gtgibsfyqf.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtgzguallj.html

C#:   (int)resp.StatusCode
来源：http://hz.wangdashe.top/gteneesfjk.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtjfvndaxi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtnrjseoft.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgfzy.top/gtrlucnycy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtoapkxfit.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gttcvpadjb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtzbzughkd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtjpdpzoey.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yuxming.cn/gtovvokatj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.andypj.xyz/gtjuezqaar.html

================================================================================
来源：http://hz.tianlin.xyz/gthksxarha.html

M. 命令行 / 进程 / 环境
来源：http://hz.yonumen.top/gtiaocsbyu.html

================================================================================
来源：http://hz.zhongyouzk.top/gtasuqnaab.html

[M01] 读取命令行参数
来源：http://hz.bjfxy.top/gtwteemcfq.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gtmsnowwig.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtnjcejsni.html

JS:   process.argv.slice(2)
来源：http://hz.yvedp.cn/gtzjhhcgzu.html

TS:   process.argv.slice(2)
来源：http://hz.sxryk.cn/gtxzwsiwai.html

Java: args 数组（main 方法参数）
来源：http://hz.shzxlz.cn/gtllhorbnc.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtveujtxek.html

Ruby: ARGV
来源：http://hz.cucudq.cn/gtzqgfabjk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sysykeji.top/gtopvwcssz.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtwevvczax.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtddfhcqrt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtxinfwyje.html

JS:   process.env.HOME
来源：http://hz.quarkkingdee.top/gttnmfvvdm.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtinkzjfqn.html

Java: System.getenv("HOME")
来源：http://hz.jiagoushi.top/gtizmwykbh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sufxvd.cn/gtaculczdd.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtotnvxtqz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtjygcegve.html

[M03] 执行外部命令
来源：http://hz.jiagoushi.top/gthtgccpsp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtzgabgneq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuetiantiany.cn/gtdkkfyqic.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.snrcjt.cn/gtzyzvkmfa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ppjwa.cn/gtdjthribu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.dashuyun.cn/gtjpnayqnu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtaesjjngu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangkeji.top/gthrligidz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gzhubu.top/gtkkdpazzq.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtjiwgddsd.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtgcxhlcle.html

PHP:  getcwd();
来源：http://hz.cashguo.top/gtphtlkgak.html

JS:   process.cwd()
来源：http://hz.tanke756.top/gtxrmcktou.html

TS:   process.cwd()
来源：http://hz.tian-w.cn/gtixcwegga.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xylfe.cn/gtxxplfuwt.html

Go:   os.Getwd()
来源：http://hz.jyoumei.cn/gtrmfctlft.html

Ruby: Dir.pwd
来源：http://hz.yuxming.cn/gtfyjsawsp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hysaishi.cn/gtkutgmibw.html

[M05] 设置退出码
来源：http://hz.tian-w.cn/gtxxretccc.html

Py:   sys.exit(1)
来源：http://hz.haohaochexian.top/gtsbvynnbv.html

PHP:  exit(1);
来源：http://hz.c1oappe.top/gtwqaodhgk.html

JS:   process.exit(1)
来源：http://hz.zhijiandao.cn/gtsiokwgtw.html

TS:   process.exit(1)
来源：http://hz.tianlin.xyz/gtgqpeottk.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtakmztxzp.html

Go:   os.Exit(1)
来源：http://hz.zhijiandao.cn/gtvathuopl.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtujmhtvjp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtyweilsho.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtpyydjbga.html

Py:   print("err", file=sys.stderr)
来源：http://hz.chenlongwang.top/gthakvtwty.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhongyouzk.top/gtrnvqarrm.html

JS:   console.error("err")
来源：http://hz.daxiang520.top/gtgovfrnap.html

TS:   console.error("err")
来源：http://hz.gotoacloud.top/gtqoxxpreq.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtqnoiloqb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinghuilouyu.cn/gtziunstwa.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtbeywbrwu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxuanxn.top/gtosbhcssr.html

[M07] 判断是否为主入口
来源：http://hz.nanxuanxn.top/gtqvzudwyo.html


<!-- 参考信息 -->