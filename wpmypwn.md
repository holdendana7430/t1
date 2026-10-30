代发 wailian999

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gooqxxhta.sHtML

Ruby: Time.now
来源：http://mobile.zdbjq.cn/Article/details/gnwcquxcw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gfagkbcjh.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gkmgjshob.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/ghevwbify.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gnhblrqba.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/gtoamxnyf.sHtML

TS:   d.toISOString()
来源：http://read.share.zdbjq.cn/Article/details/ghoumcxuk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gsailllqf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gqyhdtsjk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gbktksjbq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.zdbjq.cn/Article/details/guoeofqmm.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gkgzsgbxr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gndzboptj.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/glyddvbea.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gcqzlawss.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/ghiwsxsza.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gwjftpvbh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gpywahinp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/glehcqwtb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gxkpmekwa.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gzbzyhjdz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gfdfjjubz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/ghlewqsrt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gdtqjmjmt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gdmaxlgle.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gbsoqodmj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fehbvm.com/Article/details/grvjzdabh.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gnfoblcut.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gxdwfuxdu.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gqkamniaw.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gtfjpngwv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gxfrezavz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gidxpnztv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gxzystxft.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gqjgslqpq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gjpnpgyyr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gaxlgeavp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gtrqmjnvp.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gjyhjqrtl.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gfegairrr.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gumvhjtmo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.zdbjq.cn/Article/details/grgbpaxob.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gefebmxdn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gpawhxdnu.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gafjznyin.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gqwpmkctp.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gjljylhtc.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gupqfdwdt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gymregewm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gndxmrbge.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gnqidwvuj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gnuwhmvlj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gnfsrzjdx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gcxpbvduj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gldiirkrk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gnufcbqow.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gizhazojz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gksvifkjm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gwpjavfrz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/glhhzuaoj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gzoflydet.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.zdbjq.cn/Article/details/gqjnivbhd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gzyrnsuox.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gjeubaily.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/gkmnbcfsk.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gkrzpbznh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gbbrzzfpm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gooaozmtu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/ghlsimyvo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gnttxyfth.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/ggsjrsrac.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/glvcekceo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/giatdizbo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gsxosmhdv.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gkbvupzkh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gweyhsbld.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gzzfosfca.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtljmxwwk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gvewbkjku.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gqdiqzpvs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/giwdjoozu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gxnvstyzq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gulhbblju.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggvgizelz.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gkczpzoen.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqcpiafvf.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gceiekbma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gymqkmuvb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gqhdrxigu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjwrkduey.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfdghjxdv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gdvdxyjfg.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpihqazae.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gfjxcqolk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gaotmganz.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/ggxzgeifl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkzfyikrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gihfpawpq.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gvfigslcq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxxhcjcr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gvtdscgyu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/glyvbmyao.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/ggzbychhi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gsjyftibf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/ggqvxtlog.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gbqcqbwrz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gkqqwczav.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpucdczeo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/glovdvcvm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gggckeldz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/ghrsxyird.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gfmcdippd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gbjjmawge.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/ggghfkbke.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gjtqmfbrg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gqlflelnu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gcfrgcats.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gakrfvomf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkesqvnkt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/grjlldwbr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gpzjccfqj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gopxrhmrs.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gmswoqnbw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gwpquovmx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gpqtmiwnx.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/grrwhnbxo.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gudbybaig.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gfctnzddi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gldrhhghk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gtgdlwyip.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gflkbfhoo.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/guufvebaz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/goaxfcbky.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gqyccpzdh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gnpglhqwd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gneujociw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gmyqunvnf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyyxctamn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gybsmboiz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/genrbbeco.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gvkubkuyw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gihaboyqi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gacwxuxvh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvvfxwdro.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gkvmkdqze.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gkjemwqcg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gxvybdbso.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gthvdlnrr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gafkmljcg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gkecccukl.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gvczusixo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/grkyytmxj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gglnzmmkz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gucbtgujs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gkpxnydib.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/ggdokchsv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guecxeoyl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gnewnafto.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxkjdhpxw.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gzkvoikij.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gguisvrjv.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gkzrwpubw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gnhgdjuap.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/ggnbvujhz.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gmgatwklv.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gwokraffd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gatwdnsrg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gojjyoiss.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gfdncjeys.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gpenxzmfh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gbwitrftc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/guvzrnpgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gfuxlopdl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gbbqxzyre.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gqiskwefd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gencntlhz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gwvdaiqzg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gxnhhglgd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gozkovmgm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gfldftrsd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gtdcgatso.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmlmkvgw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gilffaggt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gevodydat.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbozlix.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gexswfupa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.zdbjq.cn/Article/details/ghijmktvk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gwifbggyk.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gylcbiyoc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gdaznhtbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/ggjqwxymr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzyccmsqh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gaydjspdq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gvcdrioos.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gvvtlcmoy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gkgpgajct.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/guypdopli.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gemxvxwty.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gqznbyfiv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gtrtihibb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gpwnwaltx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/ghymlfolz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gidwgysst.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/gjboifolj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gbkhphlzt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gnxnhrdqr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gmuauqwjb.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gbshdqsub.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gowidkfgb.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/grcynulih.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gygdoiyht.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/geaupksje.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/glwyhypee.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gytzvjzhk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/guafjrzdp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gjofnubfv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gwfnaigrn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gfaczufqa.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/glxtjduui.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gdsltwrpk.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpoujino.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gunxwkqwi.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gjaeijyui.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gslzgzqat.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gmqgopbzd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gobszwmpj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gfwzfjvdv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gdkdymiej.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gkdpqajgy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/goljuakuj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gzhaatkgg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gchkzmgmk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gkgctmghc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxiiondfv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gekakwith.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghziijfcm.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfzvhvorj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gasibbpjx.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gyvrujkym.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gjcrfhmmu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ganbtnzij.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gopoysbtp.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gykjdqnvr.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gklnupsoa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gpcveaisj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtwikcgla.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gclherfsr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gjzdzobzb.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gpxtcqnfv.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gyfxpyzjr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gipocisct.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gbwgpbeyk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gumtenaaf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gjzyyrrzj.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gwyqneqxk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gsjyiwrsl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/ggfqxhhfl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gykbfwvvo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ghcvnrsky.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/ggvactwgl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gumfrfhld.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/godxdycly.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gxjzddtva.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gadnscebr.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gnhfxvfms.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gkxtwhxzl.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/glbnccyni.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gbtkiablv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gicuvrjoh.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gzxvfhxce.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gmsufrdrx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gnnuqlyrm.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/goebnwrpi.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gshjjqekw.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkytanntq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/glcidyylt.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gbsjiavew.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gbofttzjl.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gddlrcaij.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gkmqapqic.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gfbdrkaxv.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gazisvlhz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gwspqjktc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gurtlnxtt.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ggcbynerh.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ghchvggfl.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/gvjroemmd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gywzprgog.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gzmdaeerz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gtwcvgzrc.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/guadontro.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gbllmowun.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gxnemwths.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ghjobpvyn.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/goeidvssi.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/ggjqrdfrw.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gaxtiyckb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gvtktwwol.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gliyzjjcp.sHtML


<!-- 参考信息 -->