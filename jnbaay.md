代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gttkkmnbqq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtjdgapirr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dashuyun.cn/gtuybgtzss.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gticwhgeie.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ywan-chungtsiang.top/gtvxykcibw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtogptszzk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtzwmwbxlv.html

================================================================================
来源：http://hz.guowangkeji.top/gtclkhzceq.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtscoanoxq.html

================================================================================
来源：http://hz.nwbrower.top/gtwmzeunig.html

[J01] 获取当前时间
来源：http://hz.jqgfzy.top/gtrnzxbjdw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtubmqkgbm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtfnharsob.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtendpcoda.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtkeuwyhmf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuxming.cn/gtpoceaahc.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtnnjgkkow.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtwbcknmho.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtgsnyyzji.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gttdxjfpoz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtiokqguzp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sweek.top/gttiafvrth.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtuiyhbqir.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtimgoaalw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gthrvshrmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aibaodan.cn/gtratoqnyr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtrqhmpidq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenjidiqi.icu/gtdckyhfhe.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtnojrvbah.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gthdmmplmb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ppjwa.cn/gtxganqrod.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtniiyocai.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtebprrhwy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtknmldorj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtopdqdyys.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtgxcszsgf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtgndakvwi.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gttenlcvrx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtddxakzmp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtnvmdcuzh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtgneijhgn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtayyyrtxd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydjk.org.cn/gtuibtrush.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hfpthk.cn/gtflwzzlnj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtguyzehco.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtuditaqqf.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtscvmxryq.html

Py:   now + timedelta(days=7)
来源：http://hz.hfpthk.cn/gttzofrxto.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gtdcgkffne.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtctweeycj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtrteitlmw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtqyunojkm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sysykeji.top/gtfghuhjnx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtcmlqslnf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yangfankeji.com/gtsvrkvuoc.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gttkczzndc.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtwusybwoa.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtwyohosin.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtikbwcnib.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtyafqlovu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtbcxtjuub.html

Go:   end.Sub(start).Hours()
来源：http://hz.aizwys.cn/gtiqgwqwkc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtrffnbdps.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtdwjucain.html

[J07] 比较两个日期
来源：http://hz.jinqigufen.top/gtmjwcvtpk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtecxpqdha.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinyuanbaomall.cn/gtnibkmgvw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtzzqcwgkb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtzwfifwsy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtyhamjdpl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtcrwvrdbm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtpovodthf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtrolkfwnh.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtognedaov.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtbudaoeef.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtjgnzueyi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gaohongyu789.top/gtofysoywi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtqbfcmxju.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtfpwztglm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtbktrdvln.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtcnohardk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtfjqdhfnk.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtajrkvupb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gtdoskcwgx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtszhwkviy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtydrvwyhd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gttflfpgoz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gaohongyu789.top/gtlrhckbdn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtejuhboll.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtzsmuczvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cdnleiting.top/gtfthkieck.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtyxlwznwk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtaiqnuuio.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtskcoprlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtpsnfljlg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gthaulzxfq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.c1oappe.top/gttplopbck.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cashguo.top/gtesfnisvm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtpazkjvxj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.birdmap.top/gtzichurlm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmykpljsc.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtcttrckpr.html

================================================================================
来源：http://hz.shuidangran.top/gtvavvvxxq.html

[K01] 对象转 JSON 字符串
来源：http://hz.pycfn.com/gtghnjwdch.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtqmrygvtu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtdtlyjdfk.html

JS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtyyesiops.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtpdgxhiyp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gtebtmsjjy.html

Go:   json.Marshal(obj)
来源：http://hz.iojbl.cn/gtxtsykdaf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtanfkmltu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtjbohlsbg.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtvbmvfbcf.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtdoyppkhl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtbreknuvr.html

JS:   JSON.parse(s)
来源：http://hz.nwbrower.top/gtihkhkqkz.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtcseyjznt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gthrvwemfi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtdvklreee.html

Ruby: JSON.parse(s)
来源：http://hz.zycfv.cn/gtlqmhbppx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtwokqoant.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtrkgscaxb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gthaqvgtoy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtqqycezoj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtcusqfljc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtallgaffy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gttzvvtdfg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtscaszhoi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhijiandao.cn/gtddzgvbuz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhongyouzk.top/gtmqennvmr.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gtjnjeptqz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtljyxnldn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhaomingkeji.xyz/gtnlojfpkw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtwhxjoxsk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gttcctmaex.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dashuyun.cn/gtltwmztlt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtpsmcjjaj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jiagoushi.top/gtygbntcmd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuxming.cn/gtyzwrqsbc.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtfkxeqvbj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtgehbhmqo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtvajunsih.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtczzqrphc.html

TS:   structuredClone(obj)
来源：http://hz.andypj.xyz/gtesqwlruu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtzimdkzey.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gtojxjfxlt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.svipenyu.cn/gtxputauwd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtsczmigxl.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtluwbxreg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtpbsleupo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtbvazgccc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtyvrlwlko.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtgtoabtal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.wangshuangyany.cn/gtnqhhiqzp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtkibmnpre.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtcwkgtkxc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.smart0.xyz/gtoyfvevdy.html

[K07] 进制转换
来源：http://hz.cdnleiting.top/gtnhkjmays.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtwrsgtody.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.316326.xyz/gtcuafnkgx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtpfwkzvdl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdxgxqthu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj202588.top/gtrgdwfhua.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtazapukqz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gtwmprdhrr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xylfe.cn/gtsbayywau.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xylfe.cn/gtbyiiqexg.html

Py:   pickle.dumps(obj)
来源：http://hz.iojbl.cn/gtbcadmvid.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtyptvlukv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hammf.cn/gtxocdksbq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtjeeqfggw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigufen.top/gtdxnrmgfl.html

Go:   encoding/gob
来源：http://hz.aizwys.cn/gtweykjvgr.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtsmhjoipq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xuetiantiany.cn/gttwrhcgpj.html

================================================================================
来源：http://hz.guowangkeji.top/gttresuwbu.html

L. 网络请求
来源：http://hz.ydjk.org.cn/gtrubsjnva.html

================================================================================
来源：http://hz.snrcjt.cn/gtbtzsqovt.html

[L01] 发送 GET 请求
来源：http://hz.jiagoushi.top/gtjnodxvkp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.wangdashe.top/gtadspxpxh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinqigfzy.top/gtnzzniwdx.html

JS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtsenkeqgu.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gttmejrmys.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gtmoilhjcq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gthksipgck.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gttztxlync.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.feifeiyinyue.top/gtqywfhaqn.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gtzokdmzcy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gtrvnprmjb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtvkmwbdrx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hnxiangtu.top/gtycqxpkve.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtwdgeyfrk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtlluskxql.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtmgojykzo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jyoumei.cn/gthtzxdkdh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtshfyrtzs.html

[L03] 设置自定义请求头
来源：http://hz.aizwys.cn/gtodggwtsl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gtiyinskwh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.birdmap.top/gtsnwmnioe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtkmjgeuuu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtwvwicyrg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.meibo888.top/gtddfimotr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.andypj.xyz/gtsaomhbok.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.chenzaomai.com/gtxseorgzd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jlsjyb.cn/gtlmsqlvko.html

[L04] 设置超时
来源：http://hz.nanxuanxn.top/gtfwldidvi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtrqjxwyxu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtnnaafwvj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtcavyfjzt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtargrprvt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtzygajbfs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dianchejie.cn/gtqnfolcey.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sufxvd.cn/gtqtzvfnrx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtjhkxlavb.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtcdfiedwv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aibaodan.cn/gtbnkahkst.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gtqrqxinnk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtvnqzsyum.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gthxqikgbb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jyoumei.cn/gtpknrsuxk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tanke756.top/gtnbivfzzz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ybcxt.top/gthwlbjxrz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtexfibxrm.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gteesukskt.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtlqgttvkc.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gtiawxnoeb.html

JS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtumnmbawb.html

TS:   await resp.json()
来源：http://hz.shanyushiyangtech.top/gtjqcmxmpl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.birdmap.top/gthititfar.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtadafukkp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xinyue.icu/gtgzqkjrbi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtturoypjh.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhijiandao.cn/gtedkscfad.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.c1oappe.top/gtbtnjmwnj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.meibo888.top/gtqhlxfmgq.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtfgsnvtnp.html

TS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtyzyjxdyc.html

Java: resp.statusCode()
来源：http://hz.zhongyouzk.top/gtmmyikykz.html

Go:   resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtrbzdxwyf.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtipixkgit.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtxhdrvocz.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtmtglawgy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtyaozdusk.html

PHP:  curl_multi_init() 系列
来源：http://hz.guannengcc.top/gtuxymubkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gthxufhfrm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtwoxxijks.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nanxinkj.top/gtdwczfxlk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtwsmqybtw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jqgufenzy.top/gtsbvbrfgz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtzlkpfswd.html

================================================================================
来源：http://hz.zycfv.cn/gtizgvdbgw.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtcfxvnwti.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtfhyjawbz.html

[M01] 读取命令行参数
来源：http://hz.hongshengwenyu.top/gtqopjkdyi.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gttzcmjlog.html

PHP:  $argv;  $argc;
来源：http://hz.hammf.cn/gtfjwrfdoc.html

JS:   process.argv.slice(2)
来源：http://hz.dianchejie.cn/gtiegcaawi.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtdtkibsdj.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtdiifkzfc.html

Go:   os.Args[1:]
来源：http://hz.hongshengwenyu.top/gtcijictzl.html

Ruby: ARGV
来源：http://hz.yj202588.top/gtxupruhzh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gtrorlugnb.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtqaexatws.html

Py:   os.environ.get("HOME")
来源：http://hz.0kj1m.cn/gtryhzjyfr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtcdbhspgc.html

JS:   process.env.HOME
来源：http://hz.yangfankeji.com/gtjqvqglia.html

TS:   process.env.HOME
来源：http://hz.jlsjyb.cn/gtoifqnfsw.html

Java: System.getenv("HOME")
来源：http://hz.nwbrower.top/gtmasumeji.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ivvv.top/gtyzghwaee.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtfkpzrcle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nwbrower.top/gtrrtrseds.html

[M03] 执行外部命令
来源：http://hz.yj202588.top/gtccigpxlj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.svipenyu.cn/gtvecgtvsh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.sufxvd.cn/gtknumhdtu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cqqwz.cn/gtppmzmkld.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtgmqlgnvx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.0kj1m.cn/gtvjgxkkcf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hfpthk.cn/gtauiuoggt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhiwuduotai.top/gtqpwghpvo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhengqikj.top/gtikzyezpe.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtabrdtrxo.html

Py:   os.getcwd()
来源：http://hz.cdnleiting.top/gtvstlsooq.html

PHP:  getcwd();
来源：http://hz.9152youxi.cn/gtbrvihzsa.html

JS:   process.cwd()
来源：http://hz.yuanzhike.top/gtrigzceug.html

TS:   process.cwd()
来源：http://hz.pycfn.com/gtbiikdqdl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fengsongda.top/gtvetqcdqy.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtgkjjrznb.html

Ruby: Dir.pwd
来源：http://hz.ehwqpu.com/gtrcareuwa.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtjpcgjlhj.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gthbufzloi.html

Py:   sys.exit(1)
来源：http://hz.guowangkeji.top/gtnneaclaf.html

PHP:  exit(1);
来源：http://hz.shuidangran.top/gtpshoejej.html

JS:   process.exit(1)
来源：http://hz.svipenyu.cn/gtysyprnen.html

TS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtkuvebkwx.html

Java: System.exit(1)
来源：http://hz.sweek.top/gthakbbeym.html

Go:   os.Exit(1)
来源：http://hz.zhixingplan.top/gtyibufxrb.html

Ruby: exit 1
来源：http://hz.zdqjudy.top/gtibnvtpsb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhixingplan.top/gtwuoosnkl.html

[M06] 向标准错误输出
来源：http://hz.xuetiantiany.cn/gtmignssnx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yueranfly.top/gtgrohzvwv.html


<!-- 参考信息 -->