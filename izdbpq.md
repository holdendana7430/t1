代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtwmyuvxwa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxuanxn.top/gtvjqsdncg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gthvlymuje.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtnzyjgqgu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hysaishi.cn/gtxiirknxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtnpthepwj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtypdzvqtn.html

================================================================================
来源：http://hz.dianchejie.cn/gttrkbhvzq.html

J. 日期与时间
来源：http://hz.iojbl.cn/gtwxkafrqd.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqabbiqme.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtypgiyegv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tanke756.top/gtmxrddhls.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtqvhqmwew.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtynegmmkh.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtlxcfmhva.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtjwaafhcx.html

Go:   time.Now()
来源：http://hz.hnqzz.top/gttjkhdbxw.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtzezrubud.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtnnpyxvxn.html

[J02] 格式化输出
来源：http://hz.mhx1999.top/gtcntonato.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtupeocemp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtezumissn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhongyouzk.top/gtkvuyadsz.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtjnahlube.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daxiang520.top/gtphttrbch.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtzuxhfcmb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtcbejsmkb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gteslmenhe.html

[J03] 字符串解析为日期
来源：http://hz.redwolf501.top/gtcpqjnlnk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cheryme.top/gtdzffjykk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhongyouzk.top/gttfqmtrew.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtzdtplhqh.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtqcsyveto.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gthwqtntnv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtldnrqaoy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtuhutmsag.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangtech.top/gtkpauocjg.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gthjyoloaz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtfkisprei.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtytqizeib.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxuanxn.top/gtfrefnabv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtevmwgvex.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtxgtvcifa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtcecwdzqr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtnztwjbyp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtisgdfzcg.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gtxjkishci.html

Py:   now + timedelta(days=7)
来源：http://hz.0kj1m.cn/gtkejkleig.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtjneoyuwb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gttpqqzzee.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtktxqoyjr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gttlwmretp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtyejalggw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258.top/gtamarofrl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtmqxzvqkr.html

[J06] 计算两时间之差
来源：http://hz.chenjidiqi.icu/gtluijhkte.html

Py:   (end - start).total_seconds()
来源：http://hz.wangdashe.top/gtcalfzvsl.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtoivjkdch.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtnexxomaf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtudumfyst.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtegzvbacx.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhiwuduotai.top/gtpeddbjxe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtsznsobwn.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtcgambdei.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gtwplcbjap.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtajtvaouc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ivvv.top/gtcdfrdwnb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtrhoymhiv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtzqycfcwk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtgjuvkvzq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtdlucmaqv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtczntlegx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtlnckgayl.html

[J08] 提取年月日与星期
来源：http://hz.cdnleiting.top/gtjbkxozup.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtfewnmerk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xylfe.cn/gtafcovqcx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xuetiantiany.cn/gtenmhdmor.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtqividnhs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtkelsnurk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtkfifcdni.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtisxardag.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtdybdgbxt.html

[J09] 时区处理
来源：http://hz.chenjidiqi.icu/gttcqufwha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gthfoqhjps.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtcimrgrmz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtaqpszdsn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtqpjkrxux.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydzc1.top/gtiehiblmt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtewedtoud.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtfuurunln.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtuvwmkjuu.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhiwuduotai.top/gttalrsleo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gtjcusnfzk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtmknxkfmw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtvvvmhgdr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gttczblkaw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gtfuubrnvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnqzz.top/gttkgwebem.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtujhfenar.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gthfkkjwfw.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtgsuzmcti.html

K. JSON 与序列化
来源：http://hz.zhixingplan.top/gtrbpkyzio.html

================================================================================
来源：http://hz.ppjwa.cn/gtcmxlhrza.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtbqqvsqbf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtkekmkswz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtpqmohgry.html

JS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtgynokaus.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtkgawxkbh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydzc1.top/gtddeahwuu.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtyrljrpew.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtwpnzlawc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtbttrdbxo.html

[K02] JSON 字符串转对象
来源：http://hz.zhiwuduotai.top/gtzjzqsadd.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtzoljphba.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtmtmodiwr.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gthngmhkwu.html

TS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtwampribx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtoinhszte.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gthdufisyi.html

Ruby: JSON.parse(s)
来源：http://hz.52xcode.cn/gtontgkyyq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yangfankeji.com/gtxlpkvaek.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sufxvd.cn/gtypxudzrs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtuktqygsa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtxfjcrdtv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtupeohgtr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtgcxhiieu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenzaomai.com/gtanhkhirr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtprytenup.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.havefunace.top/gtcrinlmgj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtrpuereyk.html

[K04] 读取 JSON 文件
来源：http://hz.sysykeji.top/gtsjszcpbe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cqqwz.cn/gthfnkdzzd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtnnoxihag.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tanke756.top/gthlgjmgpw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtmygttirw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xinyue.icu/gttaotdwvi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtfmrerfvp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtgldthpcl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhiwuduotai.top/gtbenuxjrb.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtbhnwflgj.html

Py:   copy.deepcopy(obj)
来源：http://hz.yanxiufei.cn/gtqfrtywnh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtdpqmscfz.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtadnivunt.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtfqptpvhl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtllxeqmbm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gzhubu.top/gtkxpeyxsw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuanzhike.top/gtytdlzxdu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtpijiarlo.html

[K06] 解析 URL 查询串
来源：http://hz.sxryk.cn/gttkemcgtx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gtqrqadwjy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtfrcgdsnm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtzcpirxla.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtigsjlnzg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.bjfxy.top/gtbehmpcze.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtdsmkhwuw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtylzyuoyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.316326.xyz/gtadqsevcb.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtfdwqckoq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtpqjopsqw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hfpthk.cn/gtsqtgjgur.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtnefjwodi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtslmkomfj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtjxgvhluf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangdashe.top/gtqmlgrlak.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtocgklumn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtostbnubz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtjdtkwtvb.html

Py:   pickle.dumps(obj)
来源：http://hz.quarkkingdee.top/gtioahqkck.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ywan-chungtsiang.top/gtcqhdzdgl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gthffzwxcw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtggthzxow.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daxiang520.top/gtikweuhtg.html

Go:   encoding/gob
来源：http://hz.nanxuanxn.top/gtoabmmbhx.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtnhzobqqg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangdashe.top/gtitqnmgvn.html

================================================================================
来源：http://hz.guowangkeji.top/gtjssvnhhp.html

L. 网络请求
来源：http://hz.kuanghao11.cn/gtzsezzsqr.html

================================================================================
来源：http://hz.chenzaomai.com/gtmfionsgn.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtwpxxkeke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtdyrxname.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtgcsuoiuo.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtibbxkkgu.html

TS:   await fetch(url)
来源：http://hz.sxryk.cn/gtgtmwqyqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtkzejydbx.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtkiznpqhq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtlmurkttp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtfxtagoyj.html

[L02] 发送 POST JSON
来源：http://hz.jianghu66.top/gtkevpfjnq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gtytxelgxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtyrjzgzbd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtalreiqpx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtdcsmfnke.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtvsegjhqs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gterqfggsp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.52xcode.cn/gtkiiximax.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtrjfpkxqc.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtnxbpahho.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nwbrower.top/gtppenzcui.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ybcxt.top/gtwhflkpdo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtmfoeubpz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtpbcvyicw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.fzhhl.top/gtoozbnvnk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtecdxnzml.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.c1oappe.top/gtiiszawpv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.aizwys.cn/gtkcznhcwo.html

[L04] 设置超时
来源：http://hz.hfpthk.cn/gtgoodrrfw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nwbrower.top/gtporxelkn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hnxiangtu.top/gtcjeozttt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gtadubdhda.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtulawlphk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtaiywknjh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zdqjudy.top/gtvvkfukkr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cashguo.top/gtmtplwmnr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtjjkurdta.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtqehuumkk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtolarezkh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.snrcjt.cn/gtnixskhca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtjsvyjmxv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gthksvwzsy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtixyseafz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtqbgveaey.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtajenwlxp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ywan-chungtsiang.top/gtqlescmsd.html

[L06] 解析响应为 JSON
来源：http://hz.jyoumei.cn/gtpxbufzlo.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtkqklnxgf.html

PHP:  json_decode($body, true);
来源：http://hz.jlsjyb.cn/gtpbjgrcta.html

JS:   await resp.json()
来源：http://hz.sweek.top/gtjtpyhodw.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtrhhtceyk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtbnksqvys.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shanyushiyangtech.top/gtdnkggrpj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtqlewymut.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtqbwkxcen.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtawmaouyd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.feifeiyinyue.top/gtgjgovjnp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aibaodan.cn/gthqqgjujn.html

JS:   resp.ok;  resp.status
来源：http://hz.c1oappe.top/gtovjoulcf.html

TS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtbkcwiqer.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtddbdiuwm.html

Go:   resp.StatusCode
来源：http://hz.guowangkeji.top/gtrszdogsn.html

Ruby: resp.code.to_i
来源：http://hz.smart0.xyz/gtvdmeedlt.html

C#:   (int)resp.StatusCode
来源：http://hz.sufxvd.cn/gtqscebamn.html

[L08] 并发请求多个地址
来源：http://hz.iojbl.cn/gtxwrvmlhk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yvedp.cn/gtpvhbujqb.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnqzz.top/gtsopdefjl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtvgweiany.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtastdxfht.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shangyingyoupin.top/gthjrtjosx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hammf.cn/gtfojpngma.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258.top/gtrilfobtz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.cheryme.top/gtffafubgs.html

================================================================================
来源：http://hz.yj20258888.top/gtsqhimnjt.html

M. 命令行 / 进程 / 环境
来源：http://hz.bjfxy.top/gtrmfgcfsd.html

================================================================================
来源：http://hz.gogol.net.cn/gtnuyihoxc.html

[M01] 读取命令行参数
来源：http://hz.yj202588.top/gttlwpfklz.html

Py:   sys.argv[1:]
来源：http://hz.hnqzz.top/gthunssayq.html

PHP:  $argv;  $argc;
来源：http://hz.jianghu66.top/gtihzqzqzv.html

JS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gtvvdaotsg.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtlejnphon.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtylllztua.html

Go:   os.Args[1:]
来源：http://hz.chenjidiqi.icu/gtnooxxuwy.html

Ruby: ARGV
来源：http://hz.aibaodan.cn/gtfihilctv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.chenjidiqi.icu/gtthjribcr.html

[M02] 读取环境变量
来源：http://hz.shzxlz.cn/gtuvadtihi.html

Py:   os.environ.get("HOME")
来源：http://hz.zhiwuduotai.top/gthutorurs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zycfv.cn/gtbbsuocea.html

JS:   process.env.HOME
来源：http://hz.nanxuanxn.top/gtthpwzkns.html

TS:   process.env.HOME
来源：http://hz.xinyue.icu/gtwcjyzmte.html

Java: System.getenv("HOME")
来源：http://hz.aibaodan.cn/gtrjduvvpn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.sysykeji.top/gtqkgzeugg.html

Ruby: ENV["HOME"]
来源：http://hz.jianghu66.top/gtomhgmxhi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.meibo888.top/gtsixpiwnc.html

[M03] 执行外部命令
来源：http://hz.xuetiantiany.cn/gtglzdoehh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shzxlz.cn/gtesmlzriq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnqzz.top/gtjhtgvkti.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtcnhgthrw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtbgnyprbj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.hammf.cn/gtnvxdfhtg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtbjmzussg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.iojbl.cn/gtrqozdphu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtehjhydoc.html

[M04] 获取当前工作目录
来源：http://hz.dianchejie.cn/gtedeeuyup.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gttqvwoznc.html

PHP:  getcwd();
来源：http://hz.meibo888.top/gtjigdpkmx.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtzlhtkpoj.html

TS:   process.cwd()
来源：http://hz.aizwys.cn/gtzibcpeqy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gttrwhmhyo.html

Go:   os.Getwd()
来源：http://hz.aizwys.cn/gtgbvskodb.html

Ruby: Dir.pwd
来源：http://hz.hywenlv.cn/gtejcpobuf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.feifeiyinyue.top/gtwkxtnbht.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gtcwdvpruu.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtfaacngzc.html

PHP:  exit(1);
来源：http://hz.shzxlz.cn/gtujutthje.html

JS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtzeferhhc.html

TS:   process.exit(1)
来源：http://hz.aibaodan.cn/gtjimjagun.html

Java: System.exit(1)
来源：http://hz.meibo888.top/gtgnemvzcz.html

Go:   os.Exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtxspgtfmo.html

Ruby: exit 1
来源：http://hz.jinqigfzy.top/gtufrwovtw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj202588.top/gtzpxzabhu.html

[M06] 向标准错误输出
来源：http://hz.hammf.cn/gtdqcuzbww.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sweek.top/gtjlsxrrgw.html


<!-- 参考信息 -->