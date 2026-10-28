代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.birdmap.top/gtfwnoykyf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtazabxbhz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtcibvpcjg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtoziahrmf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gthxebvmwd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtxaqydmfq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtrspomqys.html

================================================================================
来源：http://hz.svipenyu.cn/gtumtbnzwd.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtexjlyhrd.html

================================================================================
来源：http://hz.chenlongwang.top/gtunmsnkcq.html

[J01] 获取当前时间
来源：http://hz.iojbl.cn/gtxnxehyrr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgufenzy.top/gtgjnbfbya.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtbckxzefb.html

JS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtzhixynuo.html

TS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtqlbxgsox.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtqupzwfck.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtnjnvawtm.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtognrwkas.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtbdxxuurx.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gtuxaqatpn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtitmryrgn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtclkbxhdm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtxnkrrbac.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtnqosnxol.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtpcdvbysx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenjidiqi.icu/gtogjoiday.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtrhsrfhde.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.vqdsnc.cn/gtllkdxptf.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gticwrdfbb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtftjovzei.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hnqzz.top/gtirtcdjqx.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtbymyloyj.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtpctmbqgq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtowvdsuav.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuxming.cn/gttpxpfhbc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtgaxaiazm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ybcxt.top/gtztemaxsj.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gtvwwnqijq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gttxqstnxn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtjkdhcgml.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gthyvjsosl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gtuixhrlvp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fzhhl.top/gtiqizwipx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtjdsxdtxi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtupgzrffg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtbkdysyhg.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gthsstgzqm.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtkprxzdli.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gttlkxhyqo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtauayrxyb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtffnkpfoc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangshuangyany.cn/gtcotehkec.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtqkydkbut.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtpkcghmbh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gteweahhch.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gthhmovtyq.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gttqbiknip.html

PHP:  $end->diff($start)->days;
来源：http://hz.aizwys.cn/gtfvzitmhx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtguqkndbq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtbadukxis.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gttejaoabq.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gthfegiakm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gtxkysdodr.html

C#:   (end - start).TotalSeconds
来源：http://hz.quarkkingdee.top/gtyzqsqdjp.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtscjfgslf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtbqcwplij.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cdnleiting.top/gtegooysbq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgfzy.top/gtrfyehoxi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtiirtdost.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhixingplan.top/gtlfgajdvy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.haohaochexian.top/gtfrftvrpp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtjapwflqq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtxpekmevp.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtylfwdeox.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtvfnoxisf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gthrzjjxkj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gtapucqxvi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtsnjlaers.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtwjxzdwzh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtkrmznrpn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258.top/gtxwkqsozv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xinyue.icu/gtmobgvrmv.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtquezcwwe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuxming.cn/gtckldburs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtidncgocl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtnoxdomcx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gttsuivluh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtgupfymyd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtbxbkuflc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtrlkxoqmy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtzdkjbnba.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtpepztssv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtupuifydg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daxiang520.top/gtswgojnpk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ywan-chungtsiang.top/gtlwaxoolx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtpyhvhluv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtegtqjwmu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gaohongyu789.top/gtcpjvneti.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtefxkycin.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtaabrtrkm.html

================================================================================
来源：http://hz.fengsongda.top/gtuzcuzxgz.html

K. JSON 与序列化
来源：http://hz.yuxming.cn/gtluebsrug.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtkfbbbqye.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gthloshwjk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtlbsuaqmg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtrovzxwvc.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtzosbokyv.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtxltrfxwh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nwbrower.top/gtdodzysck.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtbljpvzgc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtpaxjuesj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtmkybnbht.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtgrhosesy.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtlbfjdzha.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtskmnpqds.html

JS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtbpebuoea.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtvgjhtutt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtqvlubhui.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtjkitkbch.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtkkbsoemw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gtvvmjoabf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtvrotipkz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtburbzryn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtgiffbryc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtcmeeygvs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtmpwhbjir.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtgawsmghf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuetiantiany.cn/gtbtelmsdm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xziqi.cn/gtyecsjlqy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgfzy.top/gtefbopwot.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtfxgsztxq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.quarkkingdee.top/gtpsrgjifd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258888.top/gtwlmcvmff.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtntphltay.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.haohaochexian.top/gtmgvodfxx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtnaicuwxe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtzaofoyvi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtljiguigj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtbbxalsrv.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtgbjtntwm.html

Py:   copy.deepcopy(obj)
来源：http://hz.tian-w.cn/gteejgqowy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ybcxt.top/gthdmvwyuq.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtnchfgciq.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtsgconuyw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gtrxhchgqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.bjfxy.top/gtfvzyxkoq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zycfv.cn/gttaroeton.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtofnetjlw.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gtsmhcnunq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtvjzwnhst.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtuqqixbpi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtdelvghxk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtrpgmsjvi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gtdrgpliox.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtjdtpvyar.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtayvmrxxs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtkhczwqbm.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gtjcjefufy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gttoqvohga.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtcsjlptmg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtjttbrckt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yongpay.top/gtowzowtha.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yvedp.cn/gtsnyrgdod.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.redwolf501.top/gtsdgvqezc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xuetiantiany.cn/gtdqyjzlwj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtbkqasrgn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangshuangyany.cn/gtivxzprzl.html

Py:   pickle.dumps(obj)
来源：http://hz.hammf.cn/gtpfrhzpwx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtxzmzczia.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtrwbyvmsn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtlfkznnwe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ywan-chungtsiang.top/gtmyeunlqx.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtnmqtsacc.html

Ruby: Marshal.dump(obj)
来源：http://hz.tian-w.cn/gtyfvldedb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtyraaeoeh.html

================================================================================
来源：http://hz.sxryk.cn/gtlxuevnxh.html

L. 网络请求
来源：http://hz.chenlongwang.top/gttvtifysi.html

================================================================================
来源：http://hz.xuanzx.com/gticqkciub.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtkoelxrqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daxiang520.top/gtodfsjzjp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yuanzhike.top/gtteyhkxsi.html

JS:   await fetch(url)
来源：http://hz.kuanghao11.cn/gtzvqstkmz.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtuzbcekec.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtbnblvjds.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gthwrxecij.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuetiantiany.cn/gtzkoipgav.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtgbcgveeu.html

[L02] 发送 POST JSON
来源：http://hz.fengsongda.top/gtcidtumvw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xinyue.icu/gtmychelpd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuanzx.com/gtehmrhchy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtdaixdgbu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtddciyhnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtzplfrmyg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigfzy.top/gtvyxsikdy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aizwys.cn/gtsfobepsg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtukasbswf.html

[L03] 设置自定义请求头
来源：http://hz.nwbrower.top/gtsfpruldy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.feifeiyinyue.top/gtajpgbstm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtqxlniadq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtrmbeulvq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gttcazgaii.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtnruohsxd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtlsxefnsl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhiwuduotai.top/gtslyioggn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gthstzeoja.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtxiguyqnx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258.top/gtojchqqqr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gthjyxxosq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtdxsfnaef.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ehwqpu.com/gtazaxnhkg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtkvxfgdnv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtwgvilbzb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.daxiang520.top/gthlhewxks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gtgebzjsto.html

[L05] 上传文件（multipart）
来源：http://hz.zhoulong.xyz/gtyfqctovr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtdkehkwsf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.nanxinkj.top/gtuhvbfdvc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj202588.top/gtndqvyrpy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtfrwsndld.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtjggarzql.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtkvmwlkso.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yvedp.cn/gtiiilmmjy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zdqjudy.top/gtvekegejv.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtypkeqeai.html

Py:   resp.json()
来源：http://hz.yangfankeji.com/gtoxsihqtp.html

PHP:  json_decode($body, true);
来源：http://hz.iojbl.cn/gtxutzryis.html

JS:   await resp.json()
来源：http://hz.ydjk.org.cn/gtrbbjeqki.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtagybxlmw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtkhpydjho.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtfdbdlavv.html

Ruby: JSON.parse(resp.body)
来源：http://hz.birdmap.top/gtrtccrjgn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yvedp.cn/gtibhvpekz.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gthvnpifxx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenlongwang.top/gtkplncozr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gtuvlzasjt.html

JS:   resp.ok;  resp.status
来源：http://hz.52xcode.cn/gtnhfuejce.html

TS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtyptzapoq.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtgrpmxefh.html

Go:   resp.StatusCode
来源：http://hz.hysaishi.cn/gtgfyitoec.html

Ruby: resp.code.to_i
来源：http://hz.yonumen.top/gtfrhxkaxe.html

C#:   (int)resp.StatusCode
来源：http://hz.iojbl.cn/gtkfpfjynf.html

[L08] 并发请求多个地址
来源：http://hz.jinqigfzy.top/gtvuqdhxze.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtujmppddt.html

PHP:  curl_multi_init() 系列
来源：http://hz.birdmap.top/gtxtotiwmr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtxogtfsmg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zycfv.cn/gtobiwoauc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.wangdashe.top/gtzyuspdas.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.52xcode.cn/gtiqufhntp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.c1oappe.top/gtvanvjetj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.bjfxy.top/gtizdyvmzt.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrkpzvjqk.html

M. 命令行 / 进程 / 环境
来源：http://hz.gogol.net.cn/gtkozatgva.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwqfywcvy.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gtaydfvyca.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtrslxaviu.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtzlrfyqtq.html

JS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtagzvhxwc.html

TS:   process.argv.slice(2)
来源：http://hz.jinqigfzy.top/gtcznhfpsd.html

Java: args 数组（main 方法参数）
来源：http://hz.jqgfzy.top/gtuuewjfce.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtlkphduxm.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtlduiyqts.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtpkbvcdkq.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtqpzcvitl.html

Py:   os.environ.get("HOME")
来源：http://hz.chenjidiqi.icu/gtrbqncspg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtsbbxpblr.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtmskigjlr.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtlkawnbfd.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtqwavprzb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtrsliucra.html

Ruby: ENV["HOME"]
来源：http://hz.dianchejie.cn/gtcdhbsppy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dianchejie.cn/gtlxymxjyi.html

[M03] 执行外部命令
来源：http://hz.cashguo.top/gtxiybjejh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtlvfrovko.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtqyjfwyzu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydjk.org.cn/gtrynvgmgh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gteehfkura.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hnxiangtu.top/gtiojfgfpl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigfzy.top/gtlvkygadq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.smart0.xyz/gthzfhhhwx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtmbsuoytu.html

[M04] 获取当前工作目录
来源：http://hz.jinqigufen.top/gtlvsaxsvv.html

Py:   os.getcwd()
来源：http://hz.jinyuanbaomall.cn/gtzeqssvah.html

PHP:  getcwd();
来源：http://hz.yj20258888.top/gtiqxjxaru.html

JS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtkevebhwx.html

TS:   process.cwd()
来源：http://hz.dashuyun.cn/gtvfoiiwzd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtwwvzczre.html

Go:   os.Getwd()
来源：http://hz.chenjidiqi.icu/gtzgslqhxo.html

Ruby: Dir.pwd
来源：http://hz.tian-w.cn/gtdcezhrxh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtevjrfnlr.html

[M05] 设置退出码
来源：http://hz.zycfv.cn/gtdnhibwcq.html

Py:   sys.exit(1)
来源：http://hz.xuanzx.com/gtrahsaydc.html

PHP:  exit(1);
来源：http://hz.316326.xyz/gtgoqjawmj.html

JS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtcfekjxef.html

TS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtsrrmffng.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtkyujqjyo.html

Go:   os.Exit(1)
来源：http://hz.daxiang520.top/gtzikonmzw.html

Ruby: exit 1
来源：http://hz.kuanghao11.cn/gtogreighq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtywavecvy.html

[M06] 向标准错误输出
来源：http://hz.hongshengwenyu.top/gtacvxwttp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhixingplan.top/gttutptfjb.html


<!-- 参考信息 -->