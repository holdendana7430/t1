代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtxiabriiq.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenzaomai.com/gtahxszljx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtpftbflvj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtcpsgcztk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtmpxnisfc.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtijqjszxr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtseybrzuw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtxkroeclw.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gttmyirihr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtkbqayhad.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtwweogomt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtxmewuduy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinghuilouyu.cn/gttrzgsbmm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtrgtjqboi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtdewklldb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtipliuxwr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtjchokxdc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtksjzvqej.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtaucbrwvo.html

================================================================================
来源：http://hz.9152youxi.cn/gtsvaqedff.html

J. 日期与时间
来源：http://hz.cashguo.top/gtrmyfqayx.html

================================================================================
来源：http://hz.yonumen.top/gtsvdiwvdz.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gtyjeelbdi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gturkgixmb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtsllvvhfq.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtztmkkuya.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gttlvuefgy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtyybjsust.html

Go:   time.Now()
来源：http://hz.ydjk.org.cn/gtxwitbvfp.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtrdxbtipy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gotoacloud.top/gtohtllrog.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtywsdjikf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtosgbnwsc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gtforgqsiy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtutjmbxbh.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtyldlkgvl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.redwolf501.top/gtgawomkhk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtraslzqov.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtvgduahsr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtbzfktbbn.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtwlvtbqlm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtuzmnynhp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gttdmssiug.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtoblkbobv.html

TS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtztokamrw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtcyvyclmx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtcidawhcq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtnmiaplwg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtvqfwpirv.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtcokmogdx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtucbmatfe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtpptzzerz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtnxfhpcrv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gttznsonrb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gtqhoklmni.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtwwedxhlo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangkeji.top/gtddkpidjt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fzhhl.top/gtsqoejzko.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtkvcinrcr.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtkyjvgawk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtffjxmkxb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtbzmeulhu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtxzjizfdw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gtyofuvnva.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dianchejie.cn/gtflfunxzt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.52xcode.cn/gtfbpznddk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtaptmsaxa.html

[J06] 计算两时间之差
来源：http://hz.xingfuxueyuan.xyz/gtefeusucy.html

Py:   (end - start).total_seconds()
来源：http://hz.nwbrower.top/gtpihfyuxy.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtqxfberbi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zdqjudy.top/gthspcvykc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gticojhney.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtkgshmkzk.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtjlvhyckk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtcuxfoziz.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtvobxsxej.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtrqocoxrh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtfayojnry.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtvotaxxsk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gttzjfdxvp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtdjqshdky.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydjk.org.cn/gtgnjiyvnt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gogol.net.cn/gtnllocvbo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtuecgbdyy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtosreqned.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtsnowfsye.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtqcjorqhq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtfimcoqpy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtimqzcgey.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.andypj.xyz/gtkzzbggbq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtdcupnwig.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtgbsgveno.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tian-w.cn/gtufardgkm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtlxmmbxda.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtyjfxatpw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cheryme.top/gtigxktmwy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gteesxzrtm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtdiwfzowm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtiosqymbb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hammf.cn/gtibxomzkg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aizwys.cn/gtwqsluiii.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhoulong.xyz/gtmpgynuhz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtwueodelg.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtsswkkylp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtjsacnyuq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cashguo.top/gtmerbmsgx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtgvkznylb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtbwjvnrhx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yonumen.top/gtttojsnlk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtsvkmhsxw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtoqrlvsjp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hammf.cn/gtgpwuwulb.html

================================================================================
来源：http://hz.sxryk.cn/gtalybnizg.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtaocdcuko.html

================================================================================
来源：http://hz.xuanzx.com/gtszyplomm.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtywlqcicw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtibefzkbk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtmrxkfklr.html

JS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtzvuimzvn.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtnlbulrci.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.smart0.xyz/gthvcmomup.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtwrqqtftq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtxhilvlfg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtwjdpjzij.html

[K02] JSON 字符串转对象
来源：http://hz.sufxvd.cn/gtuwawrjiz.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gtxffqnkbr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.52xcode.cn/gtnwjchbzm.html

JS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtwsjqmeyr.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtabeuivay.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gthcpryfhc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtjmceaeni.html

Ruby: JSON.parse(s)
来源：http://hz.guowangkeji.top/gtbphnitsi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pengpengdd.cyou/gthxqkaogj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydjk.org.cn/gtuevrvtjd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guannengcc.top/gtcmenkhhb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtqdspwydl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtwbhyfpfs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtlqebvbcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtuixogmai.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fzhhl.top/gtwztvxgmv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.andypj.xyz/gttqqkjvjt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.smart0.xyz/gtbbicygmb.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtzuighfmm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtwdtcgqmf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhijiandao.cn/gtnojcbzgt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtovolrvml.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtclyplgzx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtzepyspje.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtfwnqjxlh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnqzz.top/gthvmexzsm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yvedp.cn/gthvfaopoj.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtlunfpkkp.html

Py:   copy.deepcopy(obj)
来源：http://hz.ehwqpu.com/gtmuzdcpya.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtibmrtmfa.html

JS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtgizdhvxn.html

TS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtxsdhiivu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shangyingyoupin.top/gtpwtnzxgs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtnszoduxd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtqpfpiqhu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtmxvfvsba.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gtokozbmph.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtyxxowhwc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gthjxkctqn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtbejduyfb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gttwenjzbl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtendbisfi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gttpvtuykg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtpgipnmyp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtibpdghhs.html

[K07] 进制转换
来源：http://hz.nanxinkj.top/gtdyzuicnn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtlivozalp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jianghu66.top/gtgbuwoacp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtqsukzuef.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtkhzawsoz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gthavgyqvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtjygiiham.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtdsooadfo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gtyvsicrhh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtrnqrpvno.html

Py:   pickle.dumps(obj)
来源：http://hz.pycfn.com/gtajcxdtut.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinqigfzy.top/gtqbsmnohb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtownnqdsm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtlkhrpzot.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gthewnkjbb.html

Go:   encoding/gob
来源：http://hz.haohaochexian.top/gtkxbyemmu.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gtijfeqdgh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cashguo.top/gtndgaigxz.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtsrzglooy.html

L. 网络请求
来源：http://hz.fzhhl.top/gtcjewvsfe.html

================================================================================
来源：http://hz.aibaodan.cn/gtyzvuouad.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtxdcskejy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtxkhsjkgt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.tianlin.xyz/gtavxvligp.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtajaierak.html

TS:   await fetch(url)
来源：http://hz.ybcxt.top/gtdqvrspfp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtxdkreile.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtuddotlrh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtbggmwgbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nanxinkj.top/gtewwcovxo.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtvpbacuhc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgufenzy.top/gtmktejiyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtcsfwvpxi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtswyarkxq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtyylgwxkb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.feifeiyinyue.top/gtizcrexmp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtoufqxuxy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtqvvfheas.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gtnsoeqklf.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtjbpzvqls.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.vqdsnc.cn/gtjikyopvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.smart0.xyz/gtvsnwmdec.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gtgyqcttmw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jiagoushi.top/gteeohybqb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gtlsxovvnb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gthqtsysfy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gthytiamyr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daria6918.cn/gtghdxldcl.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gtvmixlmxo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtjwraaeyz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtykbczong.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtudepiagq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtxsgfdxtn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gtwvuyaiiv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ybcxt.top/gtfmjlrwai.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.haohaochexian.top/gtufleyucs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sxryk.cn/gtfqqlbsku.html

[L05] 上传文件（multipart）
来源：http://hz.gzhubu.top/gtvricrnot.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.aibaodan.cn/gtbgcvtsya.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtkoubgnmt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinqigfzy.top/gtprddolkr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tianlin.xyz/gtolkzgmuo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhongyouzk.top/gtwoekvclm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtsbwxgahm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.andypj.xyz/gtkuprqgky.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.andypj.xyz/gtnpbohfnr.html

[L06] 解析响应为 JSON
来源：http://hz.wangshuangyany.cn/gtkrmbatrl.html

Py:   resp.json()
来源：http://hz.yueranfly.top/gthonmtppx.html

PHP:  json_decode($body, true);
来源：http://hz.zhaomingkeji.xyz/gtsxbveowi.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtgpqvpyxj.html

TS:   await resp.json()
来源：http://hz.svipenyu.cn/gtoayhumas.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtcnkgflpt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hysaishi.cn/gtuqpprnco.html

Ruby: JSON.parse(resp.body)
来源：http://hz.aibaodan.cn/gtmcaywbpz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.sweek.top/gteyvbsght.html

[L07] 处理 HTTP 状态码
来源：http://hz.aibaodan.cn/gtjmvxxsil.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gthyenfwdn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj202588.top/gtjzjfykbn.html

JS:   resp.ok;  resp.status
来源：http://hz.ivvv.top/gtcvhdccps.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtxntwxsml.html

Java: resp.statusCode()
来源：http://hz.zhaomingkeji.xyz/gtigqnbvan.html

Go:   resp.StatusCode
来源：http://hz.zhiwuduotai.top/gtfebqqxbc.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtbnvofham.html

C#:   (int)resp.StatusCode
来源：http://hz.jianghu66.top/gtyhfstdvg.html

[L08] 并发请求多个地址
来源：http://hz.redwolf501.top/gtfingkzhu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xylfe.cn/gtixxjmavy.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtjqhvgdeq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xinyue.icu/gtwigwwbhv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gaohongyu789.top/gtabjpodip.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenzaomai.com/gtsbhmevvq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ybcxt.top/gttiljurek.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cashguo.top/gttilvrgni.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cucudq.cn/gtbjqzuzcu.html

================================================================================
来源：http://hz.cqqwz.cn/gtaxqgkhtq.html

M. 命令行 / 进程 / 环境
来源：http://hz.yangfankeji.com/gtjwzshzdj.html

================================================================================
来源：http://hz.xylfe.cn/gtuyldhaax.html

[M01] 读取命令行参数
来源：http://hz.yueranfly.top/gthcywnfqk.html

Py:   sys.argv[1:]
来源：http://hz.zhijiandao.cn/gtbutswmvd.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtqsxsngpx.html

JS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtfvpywutp.html

TS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtcmljgulv.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtqfjndqgb.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtjryorbpn.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtlxbppsbu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hysaishi.cn/gtvgxjddsw.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtutvfnpxw.html

Py:   os.environ.get("HOME")
来源：http://hz.xinyue.icu/gtxflrfmdk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhongyouzk.top/gtxajngrnu.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gttpuxeoml.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtspuwagzh.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtsskzgjdc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gttwbjybei.html

Ruby: ENV["HOME"]
来源：http://hz.9152youxi.cn/gtbtilkvyg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gtyvnpvqzp.html

[M03] 执行外部命令
来源：http://hz.fengsongda.top/gtbcbcsrdb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenlongwang.top/gtmjavlybp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.c1oappe.top/gtkqtjtqqb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jiagoushi.top/gtxvsiuojd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhijiandao.cn/gtbkekglkf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sxryk.cn/gtzelzbjbk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.snrcjt.cn/gtujctepbu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hnqzz.top/gtejnppywi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.snrcjt.cn/gtmpytxlww.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtqasmxpcl.html

Py:   os.getcwd()
来源：http://hz.zdqjudy.top/gtewidvqcn.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtutmygtmw.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtxsapvolf.html

TS:   process.cwd()
来源：http://hz.tianlin.xyz/gtldgxcyqf.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtsgeyykho.html

Go:   os.Getwd()
来源：http://hz.kuanghao11.cn/gthxfawdyj.html

Ruby: Dir.pwd
来源：http://hz.ywan-chungtsiang.top/gtkuqgdjaz.html


<!-- 参考信息 -->