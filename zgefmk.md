代发 wailian999

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qiilgixq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2szauhier.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2wwcfmysc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2loesffny.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2oaxbbpzz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2emfrheqc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2lmzpefmd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cjglfcdy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ykmmcvuh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2cjmugumq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2btuhzxyt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2bpctdcyf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2kggkmioi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgvhkdw.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wlrqnxju.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2qwrzvfop.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2qlhiskyp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fkihmaip.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zcamqdfm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vqadduuf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2psezjwlg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2lxrdqjbv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2zdsexshf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axbohpln.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pgdaqzek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knggbxam.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fmssmwmi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fartorll.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qygddwqu.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rideblpm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rtitboqr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oensecnv.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2yhbbfknx.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2zjskducv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2miauppjx.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmqrom.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ebmmjjru.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zelkttiy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2lzjqqztt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2alizdije.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2acxgepti.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2cbrhrssc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2krpmgeqb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2mjoenaqj.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bmxxqrwq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wncxqhos.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2qpealrps.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tgfscmmv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2adlnbjms.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cpqlrmxl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zlcazotu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2guqbbvzp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2nnuowkxj.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2gsafykwz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2zvhwurwq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2fgykvxnm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jalcilxz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gqaidaqj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xacneovz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vawnjdxu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pegwiduj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2grmuedqf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ssbkaivm.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2wnjaaxoe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2buifgizu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dirvdoba.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvzzjcs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nstdfdvf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2syulemzi.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2zlzlglgp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pqxnazry.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2gbbvvpid.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2enlylknc.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2tedhdith.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2mxukpvtf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2yfqsnfdf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vkjrodmk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hcpkafro.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2egjtfpci.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ghcmfzxv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2axvszrvh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zbwssdkd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2rvtckfcx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2yvwptjui.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rewdgmzu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xcndmppx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2jgnnjgva.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2akhgfzpu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uxkfwxtg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wpqnqiyi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2efrsgeci.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2mkqlehci.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2xdbtiljl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2arcwdnlr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2urdcsvto.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zulqjdos.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2iqmhewuc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2beozjfyc.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2utvbyhnh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2kesvlbox.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2udoduvgi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2liappxqm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2etzatmmb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ngwqihux.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hnygaajz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vdahronb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mggfmbqa.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ctzllpat.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kfrfsciw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2kjnhkubd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2efixiwra.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dvevvsxy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2elxftpsv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lexhqogj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2eeuzseen.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2awglhsru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afizmufi.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2caunodvs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lfevfolu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjonxj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgnkqic.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2duxpbpey.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xvswkzlx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aonkyxoz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gfaxdple.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hlyuflin.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2fxomzocd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wtgyiksa.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xxzfrbwt.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2iydewzzr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pvxynfkj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2mpmgtjba.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwvnople.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yvstlecf.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ufgzzjje.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ggfcmdtk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dattdhvz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2roqiojis.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2pitaugwh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wgefjrmt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzfdzmig.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mjtmhiub.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sapbcwho.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lhehbbbc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2skwflkwc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2dshmxkjc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2uzrpgslb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sccpeqxz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2smodprrs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vmbvgsrk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovpdsdpv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mwezluhn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2etvbwbkq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wweiitwp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxqerowv.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nzefzlzc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2dskyodof.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kjfkbsfo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bnastbjy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvtybnja.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2qzsgqxww.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2quqvaxga.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2qhthruwb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hhosymeh.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2naadmkae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mlgbmiqc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ovmeebwm.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gtarepqo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2klxjmmaa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ykfpqaej.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lbqvcmvy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fhcirebk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tuetshsm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ztmesvoj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kkqbzwvk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zsfjfbbv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2krdqqlro.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2btphxhyi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qryesacl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ieuzrowg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrnihtl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yuwsefwf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xobumsca.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2foqudeqi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hrswrseo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zvhwnprr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hroakvib.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2avyqploj.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dppjjcwp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gzgfkosv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2varwztsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogcwigta.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2pjrxcwnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgreeyzg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2dykfgfmr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tyfyfavd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2tbmnhfmk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jbrzbsjn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ojxdbquo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2syovimok.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kshbmecj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pgwktdwy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2xypihdjg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mlhetjcy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lqjyrreo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zgojzlby.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ljsrugih.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uhtaluss.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pipursfq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vhpplnyb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2iouncvww.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pjlepzqs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2olomoxnz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gricvbkc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ijvyqbzx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mdfjfmwo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2chvzdwhz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ndnjibnr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2czivkeha.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tgtajlnp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hqtkkbnl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2uhpzylaz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2conkndmv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pqyiotkz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hlybvczp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2myyjxwjr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gfpbxcae.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uglkdqjw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ymmmhfzo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2diqqsnqe.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2syapluez.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2paeeallu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qjawneqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zhtvauix.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2fkmnvwks.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hqiwgngn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzmzsson.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xqhwweqj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmoptkjw.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sblelzqi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yivxgell.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uvocisni.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sngrugqw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jnccdole.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xoysxjmr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vgyqrcez.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nrqnewoq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uhbvqoda.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2acdeognb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2funjrryv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2eqfukvga.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uhznomns.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hnryunre.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2stduojyt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ladsvvov.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2jvnewsnr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dbszespi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dnhnhnlj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pzmdajkk.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bkmivuzq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pizwhova.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2igeuurkv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2chahpncq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2onggssry.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2vjllwmnh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjwjczal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfnvtahq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hianfhvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ystpgrfu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xsuqwgto.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ekfwbgjj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2aynvskvv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bwoafuml.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tmxpiwsk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gzrgmoly.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mnfgwjkf.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2vqtcohkq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yvotrgce.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2lwycaosy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yeujasla.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ebidvgmq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qvvaxhcj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bctbrxba.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ylljokxi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aylmzjpa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2tqwbyzrq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qvbmrcfr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wqlbphge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jtjdsflj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qxspklcz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2eszncnlt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2khiwauxi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mqkumisi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2higwcbru.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hraclebr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sxgkrknd.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qzzxdjzi.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2rkrouere.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2offqoflr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ukpqcssd.html


<!-- 参考信息 -->