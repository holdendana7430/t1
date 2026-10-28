代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtaxsdahhx.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtysiduwbk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pengpengdd.cyou/gtamduddkk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ydjk.org.cn/gtbkyfdhjq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gtxfksuiak.html

TS:   /error/gim
来源：http://hz.zhaomingkeji.xyz/gtmlhgjnrq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtqlgodfmg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtvobsqgih.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtdycrkdjd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gtefgculwb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtpacflkve.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtnwdkawqf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtudixbujj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtuwqzcvrg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtdecwyzdl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtawpdmntw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtelrdevqm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtdvxktjqt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtfxyqadei.html

================================================================================
来源：http://hz.guowangkeji.top/gtbtjqmafc.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtvskdluyx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtpfxjmwvr.html

[J01] 获取当前时间
来源：http://hz.ybcxt.top/gtsefgxmam.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fengsongda.top/gtbcjmffra.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtghjpmpls.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtklladtvn.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtanuytzso.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtdamhunzd.html

Go:   time.Now()
来源：http://hz.kuanghao11.cn/gtyhymkoyz.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtqwjrrnbc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtqftgjnyj.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gtqorsffnm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtrivvzzwj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtocypgehi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtnbcckakz.html

TS:   d.toISOString()
来源：http://hz.sufxvd.cn/gtylinlevp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtqlzenqza.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtlnolsvhw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtglznwkoe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.c1oappe.top/gtsvbbnhtr.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtspjponkj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtoktpwuji.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtwbrtrpgi.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtjmfvxyzh.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtbgilfgqm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtcvnimjgb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gtxlitolcv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtjszhlfmx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtvtpzoxhb.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtawebodbz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtmbrcifua.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtwqyumebr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtmczpryde.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.bjfxy.top/gthskwgzlh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gtibkqmfym.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtmcgnordv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtoodaxtgc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtvvqjztsy.html

[J05] 时间加减（加 7 天）
来源：http://hz.havefunace.top/gtqtlpilfx.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtsepbkoap.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gotoacloud.top/gtfhzsfgvd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtzcgxfxli.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtneipfoqt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yonumen.top/gtzpqiidey.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtbfmejsai.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sweek.top/gtbtvgfpyl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtclzmziyk.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtjareodfl.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtegpovhgs.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtrpjevlsh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtprdqlfha.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtupepzoar.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtalkilvvm.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtnmeexord.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuetiantiany.cn/gtkscbbzew.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gthslqnqph.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtvhkckseq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtewuuvboh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtvixonrkn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtpsowlinz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtuqtjkovj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtzerfkynb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gtdukwhdhb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtxxrydjtj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtkobuztii.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtoksbvivn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtyubvgrvw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtzynbwrqg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuanzx.com/gtvyqxiqfk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtskhgdhsw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtruzrngpq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtputzlvcj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhengqikj.top/gtwxwrsars.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtjrocwcdr.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtpyicuwxq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.mhx1999.top/gtdjxezhqm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guowangkeji.top/gthstdfnac.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtmgyecfju.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtndvqxhyw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtcnrakgtt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daxiang520.top/gtqfdgzddu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gthkgzypcx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangdashe.top/gtxxgkgtwv.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtuvasfswt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.quarkkingdee.top/gtsfmzgybz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtdeeolysd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtughtmmka.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtwmzbolxp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gaohongyu789.top/gtdbwrgwzh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtvcyizxkn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.meibo888.top/gtkrkolshh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtjpruuaae.html

================================================================================
来源：http://hz.fzhhl.top/gtypoabomf.html

K. JSON 与序列化
来源：http://hz.bjfxy.top/gtoahmjdfr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gttvjjwnxg.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnxiangtu.top/gtiuxacwqf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtswmewuih.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtsbjovtpx.html

JS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtbcoltvko.html

TS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtkvulmwfv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtoflfcjlj.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gthylcpckx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtqcouacgz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtkwahizzf.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtjdsvqttg.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtodsiptqa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gtlcaxbkuy.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtioaiytdo.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtxpxnzgjd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gttqzuieup.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtqdxrdyur.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtmquqdoft.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnqzz.top/gtvadbxusz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtthqmybwb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtqjtkgzui.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtbdsgkfwh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtibkozjdz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtcxqyzaxe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hywenlv.cn/gtneaczzgr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cucudq.cn/gtvczluzgw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gtcxrvuzro.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtdiueggrs.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtcuuhqdzn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gtxwdeoecq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tian-w.cn/gtjdvxfvlo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtknekkjea.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtoaroprfk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtqjifgzwn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtulaxtslj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtlqztmzkn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.quarkkingdee.top/gtqmhtnkbq.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gtkspaaryz.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtcfbrzraj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shanyushiyangtech.top/gtxzdjjlun.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtzqnpmwwo.html

TS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtiplarovv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtekedjpjf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtsvwsebua.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dashuyun.cn/gtqxezesye.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jlsjyb.cn/gtsslcewmp.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtlykhluom.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtxyqddegm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtwhnqbhge.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtcrogyoqx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtfkxuhhen.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtaqyslnjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtohcvwkco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtiavtbwud.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuanzx.com/gtgziqunpr.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gttencnzso.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtbghycvhg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.smart0.xyz/gtpprdnvnk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtvyjwtifj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gthwqfakdw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtldsxjlwt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shzxlz.cn/gtiyvwoedc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tianlin.xyz/gthdadsyxq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gthzmtadrf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtipnadsqr.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtvzypdooz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.meibo888.top/gtegcadqup.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtzcdghqaj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtuqxrpuwd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtiwuxwach.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtqrwghiqm.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtihkykeas.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtjtgblrty.html

================================================================================
来源：http://hz.gogol.net.cn/gtcmbdtpyt.html

L. 网络请求
来源：http://hz.nanxuanxn.top/gtqmkozexe.html

================================================================================
来源：http://hz.ivvv.top/gtnowhzcif.html

[L01] 发送 GET 请求
来源：http://hz.yj202588.top/gtforczorr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenjidiqi.icu/gtbhdmtjgn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.meibo888.top/gtwilsgndb.html

JS:   await fetch(url)
来源：http://hz.tanke756.top/gtahcfaizm.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtljayyxnb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtcqdctdyu.html

Go:   resp, err := http.Get(url)
来源：http://hz.sufxvd.cn/gtuuitkhut.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gtppilgifj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenlongwang.top/gtwzgqrlgi.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtywhawumf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtyxgzszak.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtjvcbhexv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtukzmcwhn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gthkbxpptw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtwxpnxmrr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.vqdsnc.cn/gtzewqbjdz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtupofzzzz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.9152youxi.cn/gtudtuopap.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtltbxkmzx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gtokjgrflu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtmaxesfwy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinghuilouyu.cn/gtrmkfmcvn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gttdydvipk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtugltwtqb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guannengcc.top/gtbncxgzkv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtmkwkmgoi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zycfv.cn/gtqmcjhjku.html

[L04] 设置超时
来源：http://hz.c1oappe.top/gtocohovmh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtrphldhwr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgufenzy.top/gtzilnqwxh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtadygmsrl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgfzy.top/gtafdiumio.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtfhhtxocj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yangfankeji.com/gtsspuonin.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtdqzfotam.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhoulong.xyz/gteizwdsma.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gthmqiiwkt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.redwolf501.top/gtyjxvwepn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtefzfmuax.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gttgrlvhem.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtmtorkyhb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtcckilncf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtjesstbdn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtnwhmtrla.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtgcpvgadz.html

[L06] 解析响应为 JSON
来源：http://hz.cucudq.cn/gtjbwtmbyf.html

Py:   resp.json()
来源：http://hz.shangyingyoupin.top/gtrxjarpue.html

PHP:  json_decode($body, true);
来源：http://hz.jlsjyb.cn/gtqbpzapav.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtpuegaayd.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gtrkokttpj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtslssragj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gthmffrled.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ydzc1.top/gtewlleqwa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuanzx.com/gtveqdsnxe.html

[L07] 处理 HTTP 状态码
来源：http://hz.jqgfzy.top/gtlehwzzsx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yuanzhike.top/gtrwhyijlq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sufxvd.cn/gttewzbowq.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtpugtdbwd.html

TS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtytyiycgo.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtgghywdmt.html

Go:   resp.StatusCode
来源：http://hz.yj20258.top/gtonjofuum.html

Ruby: resp.code.to_i
来源：http://hz.pengpengdd.cyou/gtzddzigii.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtkhawphrq.html

[L08] 并发请求多个地址
来源：http://hz.tian-w.cn/gtmkqoszxw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yueranfly.top/gtxovuleuw.html

PHP:  curl_multi_init() 系列
来源：http://hz.sysykeji.top/gtgplyfhsy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtnqceismf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtwfydrgzi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.0kj1m.cn/gthckiaqab.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtqiirinki.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangtech.top/gttwwkfdbg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gtqwvqlams.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwoupucjr.html

M. 命令行 / 进程 / 环境
来源：http://hz.quarkkingdee.top/gthclxnryl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtozcefawq.html

[M01] 读取命令行参数
来源：http://hz.iojbl.cn/gtskuqjuua.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtaijrpuzj.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtkgekksik.html

JS:   process.argv.slice(2)
来源：http://hz.guannengcc.top/gtfvkunbyu.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtyrbapryo.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtqrtndbtw.html

Go:   os.Args[1:]
来源：http://hz.daxiang520.top/gtpazbhkxk.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtibtpcgjg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sxryk.cn/gtxqbehkaw.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtnicnxpek.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtecuvftqu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtvlawvloj.html

JS:   process.env.HOME
来源：http://hz.ppjwa.cn/gtxqcvfrdh.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gtshdcgcru.html

Java: System.getenv("HOME")
来源：http://hz.jlsjyb.cn/gtmttygphd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.bjfxy.top/gtyffkados.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258.top/gtfvivtwps.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtefbtawsg.html

[M03] 执行外部命令
来源：http://hz.316326.xyz/gtzpgtxrrd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtliffjqtb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shuidangran.top/gtsstzkgnx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenjidiqi.icu/gtffvdsfcj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtvtikkuch.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xuanzx.com/gtdduefmnf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.iojbl.cn/gtlnatatmz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jianghu66.top/gtrcicnpmw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtqkdljzos.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtuqcqesca.html

Py:   os.getcwd()
来源：http://hz.hnqzz.top/gtigvxbinp.html

PHP:  getcwd();
来源：http://hz.yueranfly.top/gtpzfhmqqu.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtbkzbprkp.html

TS:   process.cwd()
来源：http://hz.fzhhl.top/gtyprtbxfu.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yuanzhike.top/gtrdkadoou.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtybmbmgsk.html

Ruby: Dir.pwd
来源：http://hz.yj20258.top/gtvtqasecn.html


<!-- 参考信息 -->