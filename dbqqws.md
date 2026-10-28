代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ywan-chungtsiang.top/gtudknhigr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtonzpudyd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtgmmrcuqa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtsenmmmad.html

[J03] 字符串解析为日期
来源：http://hz.smart0.xyz/gtdgszsgnr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gtxbytcxpq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtfscysfrw.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gthnrsilpi.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gthlxgqssb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtbnscjszm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtlxycvtzd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtlqzybyjl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gtqjyiuwsl.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtuygvnikd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtrelejbue.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sufxvd.cn/gtvwootpaf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtdhoejvol.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtbjuzwxnp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtfylqfbkp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtunmrwpta.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtuulcgznj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtugsigcje.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtsatepjnu.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtuevcebul.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtqeqmtxlm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtzzaahzwm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhoulong.xyz/gtuupeclaj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jyoumei.cn/gtpbvhyltc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtjpbdlqxk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cashguo.top/gtrgkiutvn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtjmnqvdbu.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtyjgawczk.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtajwcscfp.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtcisgwpcn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtzjyaxpuc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhongyouzk.top/gtfnlbhafx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtldegbobm.html

Go:   end.Sub(start).Hours()
来源：http://hz.gzhubu.top/gtqslykmjo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtwsiavrsi.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtlcfvimty.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtgyimuvzb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtoufseoxd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtlhlwzabx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.smart0.xyz/gtozjjlrli.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gttqkvvnnf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gttgtvikfc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jyoumei.cn/gtdeykjbyp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtplswlknz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtzoikddsz.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtwubtgngm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtzxlvpeiy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtfpyotumu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtslpcmzfs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.52xcode.cn/gtfueqbxhz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtctjpiudg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gthcunavvk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aizwys.cn/gtevsnelxn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtppptbumi.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtysqozxee.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtncktnbei.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ywan-chungtsiang.top/gtfskxcipk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gthkftwohs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtupahtsue.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pycfn.com/gtfuabozlq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtbfuqjsth.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtodvdrkkv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtnrirdleo.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenzaomai.com/gtlzxzbteg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hongshengwenyu.top/gtkxfoovkf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydjk.org.cn/gtbmdxuzll.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenzaomai.com/gtpzxegzkj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtktdbheum.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ywan-chungtsiang.top/gtkhqsmarr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtfvjeowbr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtlhxgfrop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtldtsolou.html

================================================================================
来源：http://hz.hnxiangtu.top/gtvddjdllg.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtcptezowj.html

================================================================================
来源：http://hz.gogol.net.cn/gtdxppmssx.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj202588.top/gtwtixbgpc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gttwdniwnz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtkebodypz.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtlkwmrccj.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gthukwlcut.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.meibo888.top/gtbtibyehe.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gttmdpvppq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtgnniqjvg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtbsngoaty.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtybdxoiek.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtapqvtatb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xingfuxueyuan.xyz/gtbnjnmavo.html

JS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gthqbanaqd.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtspvhbhfz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtrpbzdpvi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtlbvoapik.html

Ruby: JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtybxgcprw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtmwyensto.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtuzrnkcrx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtoadaoaqv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtudckchak.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtkrpvmjgm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtcrrquvse.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gttojybecw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtgxvljjxx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtblhktguz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtsdzkwbkl.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtbvxzixqr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.bjfxy.top/gtjhpyyaox.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gthoxhxprc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtwyyviaxh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtzvxaarvr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtwcnhaoeb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtyylixhpq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuanzhike.top/gtircqxpsj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shzxlz.cn/gtcoltdsqx.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtstehnzzx.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtmhvbgtle.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dianchejie.cn/gtdkmhyove.html

JS:   structuredClone(obj)
来源：http://hz.gogol.net.cn/gtfgztcoyr.html

TS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtiqisfidu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gtjkpwbxqh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtplgzwnpe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtirudzivn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtmdafpwoj.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtmzadbker.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtirrzzgda.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtbltfxpek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtmezwhnzc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtxhqycbnh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtugfdxjbg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtjunwtecz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.0kj1m.cn/gthxfnolif.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yonumen.top/gtigbfasji.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtjxltxish.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hammf.cn/gtjooamsjf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.nwbrower.top/gthblbqvle.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtpgfxycgi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtwapswukd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtdpkrkfwz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinghuilouyu.cn/gtyfmivtid.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yangfankeji.com/gthxmqjzxx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtdjteajtr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xziqi.cn/gtmytisjky.html

Py:   pickle.dumps(obj)
来源：http://hz.mhx1999.top/gtwrbzggck.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sysykeji.top/gtvhfzifoa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtxygkxmxg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtijjvgska.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xinyue.icu/gtgowunyrt.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtpqvxyrqi.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgfzy.top/gtfshchatd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtuhakumpq.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgcphkqhu.html

L. 网络请求
来源：http://hz.mhx1999.top/gthnphlbez.html

================================================================================
来源：http://hz.ivvv.top/gtijtcperx.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtvetwyhdy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hfpthk.cn/gtgrlorxnr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xziqi.cn/gtfcxkkrsd.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtjsjysjgw.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtqsstzetd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangkeji.top/gtzlkosveg.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gthwdmfiwj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xuanzx.com/gtdiwvtjlq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtwycffgld.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtzljvrmgy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtwcyfffeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.andypj.xyz/gtwmmriphr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pycfn.com/gtvqapdtjp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxuanxn.top/gtwqptlpni.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenzaomai.com/gtkokkwbrw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gthreyjgsp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtauvuczrc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sufxvd.cn/gtqhsxijpc.html

[L03] 设置自定义请求头
来源：http://hz.ppjwa.cn/gtorhhcgws.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hammf.cn/gtqoclnptm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.daxiang520.top/gtpnunaoch.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtruuuetmg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hongshengwenyu.top/gtyzfbmcjd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.0kj1m.cn/gtgiryohuy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gteakoxwbz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daxiang520.top/gtodeiigyg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gtjznktzzz.html

[L04] 设置超时
来源：http://hz.sxryk.cn/gtldetrxnf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtbtohsodr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guowangkeji.top/gtndpgpqgz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtrarfuios.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.c1oappe.top/gttvxhmtgt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgfzy.top/gtuzudpfxa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jiagoushi.top/gtjiiumffu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtwwwlamfs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtdvvsbosx.html

[L05] 上传文件（multipart）
来源：http://hz.daxiang520.top/gtgsuhaqym.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtkqcorpbq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jianghu66.top/gtgpyenpav.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtawouijil.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtsjqpltqa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.tanke756.top/gtugkqvhsn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.hammf.cn/gtdbugxzdp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtfwbkvnac.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ybcxt.top/gtnffsktfp.html

[L06] 解析响应为 JSON
来源：http://hz.tianlin.xyz/gtlikazalh.html

Py:   resp.json()
来源：http://hz.cheryme.top/gtxekhoqhx.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtjdzgpavp.html

JS:   await resp.json()
来源：http://hz.chenzaomai.com/gtzaauukvo.html

TS:   await resp.json()
来源：http://hz.xylfe.cn/gtifxbbfrj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.aibaodan.cn/gtcwvioksx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cqqwz.cn/gtkcqgxnjc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtfelbzmdw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.c1oappe.top/gtcnewdcln.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtfonhyray.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cdnleiting.top/gtkqbwyhga.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pengpengdd.cyou/gthuholgpg.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtvnmuspsi.html

TS:   resp.ok;  resp.status
来源：http://hz.zhongyouzk.top/gtgfgdgspx.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtbwwizkqw.html

Go:   resp.StatusCode
来源：http://hz.xziqi.cn/gtappetgzq.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtelfytqwk.html

C#:   (int)resp.StatusCode
来源：http://hz.hnxiangtu.top/gtcunpezsb.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtuuhmcbhh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.meibo888.top/gthwtkwzkr.html

PHP:  curl_multi_init() 系列
来源：http://hz.hnxiangtu.top/gtrfsiufja.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtegozsefq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.sufxvd.cn/gtoouawgjf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtgkghvjak.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hnxiangtu.top/gtmnqmacki.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtfqnonckt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtclkeiama.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtgznatsjl.html

M. 命令行 / 进程 / 环境
来源：http://hz.wangdashe.top/gtwolkfxtc.html

================================================================================
来源：http://hz.redwolf501.top/gtcvddqets.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtrsgoekyy.html

Py:   sys.argv[1:]
来源：http://hz.0kj1m.cn/gtfqbkypko.html

PHP:  $argv;  $argc;
来源：http://hz.nwbrower.top/gtdrchcurj.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtznoriyld.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtcpwcdpot.html

Java: args 数组（main 方法参数）
来源：http://hz.tanke756.top/gtepmoxfni.html

Go:   os.Args[1:]
来源：http://hz.jinyuanbaomall.cn/gtuagzcghf.html

Ruby: ARGV
来源：http://hz.havefunace.top/gthmpnbqlb.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtmbykpodl.html

[M02] 读取环境变量
来源：http://hz.hnqzz.top/gtrkjwziud.html

Py:   os.environ.get("HOME")
来源：http://hz.cqqwz.cn/gtbzyjzqee.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gtzpzvnqmz.html

JS:   process.env.HOME
来源：http://hz.xinyue.icu/gttgehvyts.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtkjlmwwsi.html

Java: System.getenv("HOME")
来源：http://hz.shangyingyoupin.top/gtydykanvt.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gttefotvhq.html

Ruby: ENV["HOME"]
来源：http://hz.shzxlz.cn/gtphvqnnwt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nwbrower.top/gtcwcvgvmj.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtaqckkqgi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhoulong.xyz/gtlfuqzmcp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gzhubu.top/gtarjwypxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtcyvtkglm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtiebvfjnw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhijiandao.cn/gtxhnlytpx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtmsyxemwj.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ydjk.org.cn/gtztfeoouj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtecamldsa.html

[M04] 获取当前工作目录
来源：http://hz.jqgfzy.top/gtrlbpzqnn.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gtxaeuqxts.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtuntcgkog.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtqqxroupx.html

TS:   process.cwd()
来源：http://hz.gzhubu.top/gtskazusmc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.feifeiyinyue.top/gtbkbfaaad.html

Go:   os.Getwd()
来源：http://hz.jinqigufen.top/gtfyrwurhe.html

Ruby: Dir.pwd
来源：http://hz.xingfuxueyuan.xyz/gthrqkdnmf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ydzc1.top/gtqggjixgt.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtyifuwpdn.html

Py:   sys.exit(1)
来源：http://hz.guannengcc.top/gtdagrqjyu.html

PHP:  exit(1);
来源：http://hz.wangshuangyany.cn/gtlqumtvnp.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtcyadsgrf.html

TS:   process.exit(1)
来源：http://hz.daria6918.cn/gtzsrurbpk.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtxwosolkz.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtbovqhpnw.html

Ruby: exit 1
来源：http://hz.ehwqpu.com/gtqzzgoodj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhaomingkeji.xyz/gtckfjgxai.html

[M06] 向标准错误输出
来源：http://hz.dianchejie.cn/gtdkkbxxes.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtdcwnlycj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhixingplan.top/gtgulaznou.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtsojcjchn.html

TS:   console.error("err")
来源：http://hz.sufxvd.cn/gtxpethbof.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gthstgvtlb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtufgkulhk.html

Ruby: warn "err"
来源：http://hz.xylfe.cn/gtyjksreoa.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtsbuxxhnp.html

[M07] 判断是否为主入口
来源：http://hz.mhx1999.top/gtovxmsngq.html

Py:   if __name__ == "__main__":
来源：http://hz.nwbrower.top/gtyjtexdzd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.tanke756.top/gtoefcpizx.html

JS:   require.main === module
来源：http://hz.jinqigfzy.top/gthocplvzv.html

TS:   require.main === module
来源：http://hz.cucudq.cn/gtmzpwerfi.html

Java: public static void main(String[] args)
来源：http://hz.gotoacloud.top/gtmosohgzf.html

Go:   func main()
来源：http://hz.yangfankeji.com/gtmechtcij.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.0kj1m.cn/gtlguyqxif.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtbicppnzg.html

[M08] 获取系统与运行时信息
来源：http://hz.ehwqpu.com/gtslrirvji.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jqgufenzy.top/gtyapuhpuk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.tian-w.cn/gtmpddqirh.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtvmmrggnp.html

TS:   process.platform;  process.version
来源：http://hz.aibaodan.cn/gtdltdemdd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zycfv.cn/gtcvauinzz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cashguo.top/gtvegzovyk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gtreycumlw.html


<!-- 参考信息 -->