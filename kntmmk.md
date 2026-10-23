代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bueyhluo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qsclpmsa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xmnrywkb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dhduebfe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3fhxyhotv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3odsjwdgq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3bnnnagnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bflooqli.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3krqnxjli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwqsaxun.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3dcjeyktb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3bzwhayhc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3hrqndwnf.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3mxwrxupb.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3yeqqbsts.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3dfkfzcsy.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3uiiutacf.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3jbblaqbt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3rminmtkg.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jfztzvjp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ecydpwhh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3lfphsztj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3jsfaoeux.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xdxsvztp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3cmbbizzy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3gekedctm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3eiqfowue.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3lyumhdhk.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3invfxabj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3zjlxtmkr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3ezheuvdi.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cbrtaqhe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kxcpxxeu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qweawxvy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3whijhiqy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nbangqri.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmrxtfq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3vguebslq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lqsooelo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3hkbayezo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdecwzb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3eqpppqsg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ezdcaabz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ofbalujp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3jaapfiin.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3thbdiiwq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zfyzgbsb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3mhmwhmhg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3lhrymbvn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3uonckrzb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3snppoetc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jeehquhi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3idpkjsiv.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3laqmrqig.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zsbynouk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3xafkrtxz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jgmafwtr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3clmyskpe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3vyrjowax.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rylhtttr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3topfuqyo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ngfpqesg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ectppfps.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3tvjlhyjp.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dbleaagz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qzmamvwf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3yyhncqla.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3qthdcnhz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3xvuxqacs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuspohoi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3twxzuger.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3sewymbjm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ooumkaut.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3pztugosj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3tqfeoabr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pqmfkpod.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3efpuowkn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ahlvucrk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ftekivhi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lbqiduax.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3tiisqxql.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cconxtcy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xmxueasg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mupfbnlr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3wxngeakx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dhqohxbi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsqbuce.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3murljcog.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkfkmg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3lyswcdbs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3wixdnvez.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3xqubosdf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3cdufqyea.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3kkwymlxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ekbxjvjj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3drmaijrl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ilhqqzhd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3oddqikld.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3fsistfxf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3uvlxxxmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erkhdghv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rtvemihc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgqblios.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3sbbcbgwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jqitjulf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3umcmodrk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3npoemvtr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twrsfgwa.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3xceyfavh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jfvndgnk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3sefbcgbj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqjzpzuu.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3unwrpujg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3nkvwzmzn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3olyexcup.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oadbwgxv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnxwvdp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3knthdhcr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3vgjenmxp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nozxxkgx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gbjvqtkd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ezkzazzg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3afomlqpu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ulphgcby.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qkuovbic.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjvyjxyo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kbctalhb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3tofrohxx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kcabxzol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hlgnslvn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3fdyuklul.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnlnabui.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3jobdrxan.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qixscpkb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jbjwguaf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lqqkjtdn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3xobavbdf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cpkrbgyb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbybbffk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3mnadauov.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjyvjwbj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3htjhxkds.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjnnvouh.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdrapbno.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3fedteocm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3umuthbnu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ngvyqvkv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3jdikwxus.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3vvkldagj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mjybdbtt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3grmnnuys.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kwmbdynm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vvheqbzk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3hrbttjij.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gllgiccw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hsiohotp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zsadbfvf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3zkhmiewt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mpxypecw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3dfhhmayv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ragtbvdt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hanljonl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qcotharh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3squzawrl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ddxvohke.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wrcywmhb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xkfyxjhw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjlckoaw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3rwzcjphg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3dznvzmvq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wnmlwnum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gouxyvem.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hcwehars.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qbunxirf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ijksfown.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iugkmwtk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ubtoybgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymyegbjs.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3gevtleng.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tscheuan.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3frlykoqw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vexpoblp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ceczfemi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3yversidh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pprkyeco.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gqqidabp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qizpykhd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jjccnyvy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3uhhlbreo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3arojvuog.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ssfmhfnk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jnlsjugh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3amxxoakm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zvmoxjwe.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3olwlvgle.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3pvcdcnfx.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3myekjihd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bxiojrvq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlzurccq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3sccpdsbj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ponjrjiv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3dsmnesap.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cervtsgx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3pfqubhtb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zpdowicg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3dfbewpuv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3eepsijoj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ympslyky.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mctrpldq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3otilggws.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pynmyrtu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3whyeylhm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3mjtjcnvr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aoygwxbf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fkvxvgbe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tiujnwot.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcbhxmwr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mmpievye.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qiwekvgq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tvhpwbwn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvjcguyh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sdbsandx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3caroqirz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wlpwrier.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3myemkewj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3qmodzqte.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dywyfxsd.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jalnqrhh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3imgftwea.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rdvhpfqg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xlzcydrs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tvyyberd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lwkbrabz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3gemcizcc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jclokpok.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mcezwbdm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vmwdfwux.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uuhgpuds.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3relyvgrx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ccuxnqfc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dzsupikj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mfvfeluj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3wcwucdvg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3wjyhlqdy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uajtwcap.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3crfznxzq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xzmdvpia.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wxvhoggn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xoqgelbc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dlkvtzwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agztqggb.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ldfjaqhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufnkpokv.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrhoobzk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cqzlknpb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pdgkngfc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qorqegnw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxjthwe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tivflgif.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bsjzupip.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3cjkwqiea.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gijdmwxb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iqhznntl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zlkciiaf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xngqdtkr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sklrpwqs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3dkhtavbs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pzsqutha.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jzsogoar.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ddgtggrh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xfliciok.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nbffdrpj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lsondiql.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jtegbrja.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lddivydg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jnjkguwe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3tahytovw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3eqkimhqw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rvzbikso.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oedhpovp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3eiqnxxcc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3iurovfaj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xddvzjqq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fanvzitb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iymhbhnn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uvkdfoks.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vlzkuqod.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sodtneyg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3adqxrcpv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ogxsmwxv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dudszcvj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jxkbtrhi.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3faggvvxy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bhgwanko.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qumvyvkz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdyztcbv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zcajtkku.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bpmfodig.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hufqcwvj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3iwkiapms.html


<!-- 参考信息 -->