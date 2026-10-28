代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtcwvpcqxq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sufxvd.cn/gtdfttosdc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nwbrower.top/gtzwufzgjx.html

================================================================================
来源：http://hz.fengsongda.top/gtgjgzggcq.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gttkltdizg.html

================================================================================
来源：http://hz.jiagoushi.top/gtppdezsen.html

[J01] 获取当前时间
来源：http://hz.iojbl.cn/gterdgjixv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtpvxsqiwi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtaoddautj.html

JS:   new Date();  Date.now()
来源：http://hz.jqgufenzy.top/gtfhbiaoed.html

TS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtpyzyugxv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtyguvnrgh.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtqdhtbyld.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtnvfpaxce.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtpszrghcy.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtxoolowda.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtsyfhksza.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtczisttor.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtvehsursi.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtdzfhshml.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtvqslsqml.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinqigfzy.top/gtefdzqttq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtiwyvpodc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pycfn.com/gtclwojdfi.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtjjdrdrfi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtsnjuzffp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtppyvhiue.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtpovcmiyg.html

TS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtcewdttjx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtndyhdfkl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtzlihrirm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtufnorgtd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtgbgcjuar.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtluunzplf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gzhubu.top/gtgdsizpbl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtsnohukxj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtdhohtndj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nwbrower.top/gtthdukpqe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.9152youxi.cn/gtegvsmlas.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yongpay.top/gtrljfemcz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtkzfovylj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guannengcc.top/gtaawfjzrc.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gtbdugozor.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtazkkmooc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.svipenyu.cn/gtitjkcmxa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtdrzwgloz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtqexearpv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtziyowuuz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtroerzvus.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtcanqvhnp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gttrhcrdom.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtcdsofkig.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtkatqcohd.html

PHP:  $end->diff($start)->days;
来源：http://hz.ppjwa.cn/gtsvdmjwed.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shuidangran.top/gtdyvvqadg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtsdxvujmu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtzdrlwihm.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtbzqwckez.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtrydiuvbg.html

C#:   (end - start).TotalSeconds
来源：http://hz.gotoacloud.top/gtietrogvg.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtoolygmgx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtjlroclth.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gttbcrbdul.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtydcibfse.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtaafrzrjy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtftpyolds.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtvnpybwnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtvedvpsik.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtvkmmglcw.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtrwbmfjec.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtkrfqtwvm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtajlztzks.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtxqaqpxxm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtjfjaadno.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenzaomai.com/gtojeizwaw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.snrcjt.cn/gteiqfzxgk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhaomingkeji.xyz/gtwehmkpai.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gthqniiiim.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtlsrilelx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gteejtfxyx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gttuggijjb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtroauluqn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gttqtriife.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ywan-chungtsiang.top/gtpialgjgp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gthtirjymx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtxxfqtynp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtuopfimbq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gthxdlsqra.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gttarnjidv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangdashe.top/gtxtnxylzv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cheryme.top/gtatuztzul.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gotoacloud.top/gtapreqlbe.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtuptaewri.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gteluwtihh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gtysbmocwl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtyjngwtje.html

================================================================================
来源：http://hz.birdmap.top/gtxsubxzdt.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gtpzdepwnc.html

================================================================================
来源：http://hz.cdnleiting.top/gtnegrwoap.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtkbfzenuq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtsnnrwxcb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gttchlndqo.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtqgoegnuw.html

TS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtdhxrpykq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtznwrtjfo.html

Go:   json.Marshal(obj)
来源：http://hz.nwbrower.top/gtqpwpjire.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtmuwntcff.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhaomingkeji.xyz/gtiakwcqzt.html

[K02] JSON 字符串转对象
来源：http://hz.zycfv.cn/gtoqvrwelu.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtittdyfli.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtzgspfcae.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtnkyxsgfb.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtbgudsjee.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuxming.cn/gturiglbtj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gteoakudtk.html

Ruby: JSON.parse(s)
来源：http://hz.ydzc1.top/gtcqwhqhdz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtiffdcxmh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtpoqkrpbb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtrbbgrxse.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtiwkutlsw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtlewhurpd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtauiftupk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.vqdsnc.cn/gtdlephisf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtnnmkcazr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtxxxvzonn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtjyexxksy.html

[K04] 读取 JSON 文件
来源：http://hz.yj20258888.top/gtkmveqpgg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtrtsozslk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.snrcjt.cn/gtglmwbexc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtpqsavtpw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.c1oappe.top/gtpvoyrncb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.feifeiyinyue.top/gtilwpszle.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtoeblxrgb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtfvcooqkm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hnxiangtu.top/gtkhnwmoov.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtmrurjseh.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtsbndjfpy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gtwjgbfkse.html

JS:   structuredClone(obj)
来源：http://hz.yj20258.top/gtailprngb.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtuuejmfyg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtuztjogkr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtjhyaqwnm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtkqqrwqll.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258888.top/gtwbnaacvc.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtlsllvnaq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtttjxlipc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtqvkokmiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtnxstgute.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtcvasnilo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shuidangran.top/gttefooqet.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtrsycxzea.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtawxfftob.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtsvzjlhwe.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtkkbxeyvq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtfznnanmm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gtymtuzzst.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtzffmlixw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtgefpahub.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtynnxvihr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtlxjgusgq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shanyushiyangkeji.top/gtdqcfzwib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.wangdashe.top/gttgprlkpl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhixingplan.top/gtdnmthcon.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtphmvnflz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gthwcaaqty.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtgtbasvgr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xinyue.icu/gtnnmzrgmn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtuciuxycg.html

Go:   encoding/gob
来源：http://hz.52xcode.cn/gtykndqxrv.html

Ruby: Marshal.dump(obj)
来源：http://hz.bjfxy.top/gtgdbcbayo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtpcoqarau.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxsbfafwc.html

L. 网络请求
来源：http://hz.cdnleiting.top/gtaaiespki.html

================================================================================
来源：http://hz.jiagoushi.top/gtqaqigphv.html

[L01] 发送 GET 请求
来源：http://hz.haohaochexian.top/gtniefrarh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gthcdltnru.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtektyodxy.html

JS:   await fetch(url)
来源：http://hz.tanke756.top/gtidasdwbt.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtexetligj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtitoybmzn.html

Go:   resp, err := http.Get(url)
来源：http://hz.gaohongyu789.top/gtmdnegjzl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenlongwang.top/gthgygkngr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtvztjvdxb.html

[L02] 发送 POST JSON
来源：http://hz.tanke756.top/gtmallbkiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yuxming.cn/gtflhspmkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangkeji.top/gtjzmuqpme.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtuudgpyoa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtwbpehjaw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hongshengwenyu.top/gtpftxhgop.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gttcwgkluo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtwjulrcrh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.52xcode.cn/gtiwwgjnjh.html

[L03] 设置自定义请求头
来源：http://hz.nanxuanxn.top/gtuqfdlodj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtsghkrtll.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.vqdsnc.cn/gtbasyslbh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gthykpqilz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtlirjofkw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xuetiantiany.cn/gtadwqeefa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yanxiufei.cn/gtzkgubtce.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jqgfzy.top/gtmubhrrfa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.sxryk.cn/gtambackya.html

[L04] 设置超时
来源：http://hz.zhongyouzk.top/gtvbnxsbmb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tianlin.xyz/gtyghrdbit.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtjfjbqnzf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtzlaaiewx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtrlbsloxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtzyvogfvt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hysaishi.cn/gtflekrjrn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhengqikj.top/gtplabtukt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtdjdwbibg.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtxpvrkrfk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.snrcjt.cn/gtjgxtbpag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cucudq.cn/gtmaqpntdx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtaiwrcvzi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtxgauncgd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtyeehqxaz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtgnjlhvvz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.feifeiyinyue.top/gtsknabkft.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shzxlz.cn/gtxkxdkryu.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtwsnrezrc.html

Py:   resp.json()
来源：http://hz.hnxiangtu.top/gthohjminx.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtipzkukdo.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtwmrplawi.html

TS:   await resp.json()
来源：http://hz.kuanghao11.cn/gtdmmjazmw.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daxiang520.top/gtybomcxdx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtxsfhedwi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jlsjyb.cn/gtlgxwevzr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yuanzhike.top/gtmnhwzwby.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtgnhhqgyc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.gotoacloud.top/gtxwzyxebo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtkatiixyv.html

JS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtleyxlntv.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangkeji.top/gtqvnhxbvf.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gttlvutrqk.html

Go:   resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtjdzedpjl.html

Ruby: resp.code.to_i
来源：http://hz.jqgfzy.top/gtwvrfwkzw.html

C#:   (int)resp.StatusCode
来源：http://hz.xinyue.icu/gthpcwngjp.html

[L08] 并发请求多个地址
来源：http://hz.fzhhl.top/gtsuqyqynm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtoelxbnse.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhengqikj.top/gtvvdtriqw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gteorelyyd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtikhzyasz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shanyushiyangtech.top/gtrrfliwpt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.quarkkingdee.top/gthgumdgqp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gtdmqnyaol.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhengqikj.top/gtbmryyfpw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtngddttex.html

M. 命令行 / 进程 / 环境
来源：http://hz.c1oappe.top/gtrjahchmy.html

================================================================================
来源：http://hz.vqdsnc.cn/gtseviemto.html

[M01] 读取命令行参数
来源：http://hz.pengpengdd.cyou/gthalowpio.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtmkhpnnbc.html

PHP:  $argv;  $argc;
来源：http://hz.nwbrower.top/gtlfqcetrk.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtjprskawf.html

TS:   process.argv.slice(2)
来源：http://hz.kuanghao11.cn/gtkechconi.html

Java: args 数组（main 方法参数）
来源：http://hz.hysaishi.cn/gtwtdewilp.html

Go:   os.Args[1:]
来源：http://hz.zycfv.cn/gthvbaeodx.html

Ruby: ARGV
来源：http://hz.9152youxi.cn/gtittfcmnm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yvedp.cn/gtjivyyylq.html

[M02] 读取环境变量
来源：http://hz.zhaomingkeji.xyz/gtqqxqznme.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtfjdswboa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cheryme.top/gtmsbskskh.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtbuvlxabg.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtywcatlmd.html

Java: System.getenv("HOME")
来源：http://hz.hammf.cn/gtgthasmxx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.iojbl.cn/gtwpbttrba.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtdhsuudtg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.yangfankeji.com/gtpqcmmbjr.html

[M03] 执行外部命令
来源：http://hz.hnxiangtu.top/gtdwlpecek.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258888.top/gttjltleth.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.guowangkeji.top/gtevgtfisu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.wangdashe.top/gtmwnzwkju.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtrxpdvbyl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cashguo.top/gtsyyupudj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhengqikj.top/gttsenqcrk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenlongwang.top/gtnzjrdmwd.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sufxvd.cn/gtmvhccrwr.html

[M04] 获取当前工作目录
来源：http://hz.jqgufenzy.top/gtlnmvkddx.html

Py:   os.getcwd()
来源：http://hz.quarkkingdee.top/gtwokwjlyw.html

PHP:  getcwd();
来源：http://hz.hfpthk.cn/gtpaukcayy.html

JS:   process.cwd()
来源：http://hz.shzxlz.cn/gtzddtwqed.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtejkepmen.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtasomfyrq.html

Go:   os.Getwd()
来源：http://hz.tian-w.cn/gtncavfbnw.html

Ruby: Dir.pwd
来源：http://hz.zhijiandao.cn/gtenamgvju.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydjk.org.cn/gtwdtgfntf.html

[M05] 设置退出码
来源：http://hz.jiagoushi.top/gtlgednvjq.html

Py:   sys.exit(1)
来源：http://hz.jiagoushi.top/gtocsjnxdn.html

PHP:  exit(1);
来源：http://hz.cheryme.top/gtgnmdhfmz.html

JS:   process.exit(1)
来源：http://hz.ybcxt.top/gtfoedcyri.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtibnlzqkj.html

Java: System.exit(1)
来源：http://hz.hnqzz.top/gtjrozrnyd.html

Go:   os.Exit(1)
来源：http://hz.hysaishi.cn/gtckcrqieu.html

Ruby: exit 1
来源：http://hz.sxryk.cn/gthhvzwija.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yangfankeji.com/gtoynwupmp.html

[M06] 向标准错误输出
来源：http://hz.redwolf501.top/gtysssgwqo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuanzx.com/gtojdctkji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtlpcvetxo.html

JS:   console.error("err")
来源：http://hz.sweek.top/gtutnlnmte.html

TS:   console.error("err")
来源：http://hz.zdqjudy.top/gtioregyaj.html

Java: System.err.println("err")
来源：http://hz.chenzaomai.com/gtyteeazfb.html


<!-- 参考信息 -->