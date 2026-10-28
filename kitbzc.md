代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gthsdijpfs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtkzunnfqp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtlojxirgx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtavipvyda.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sysykeji.top/gtwecahsuo.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtkjzqzlln.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenlongwang.top/gtuvbyptog.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtahdjupbr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtafrhnfjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtuawhgmbt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.9152youxi.cn/gtelxhpjfc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtzwyfsprv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtxaykemos.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.redwolf501.top/gtaynarinj.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtcdqzcqsj.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtidywhsfv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtrgxszduv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gthtfolejg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtnemegktx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gteopzwuwi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gtmypgnxxd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cheryme.top/gtjasitvcr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtbpsoejte.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtxpvhlvdy.html

Py:   (end - start).total_seconds()
来源：http://hz.daxiang520.top/gtymanclda.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtufuendwz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtiuoielro.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gttjnmpgxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtfvuvrqcr.html

Go:   end.Sub(start).Hours()
来源：http://hz.xingfuxueyuan.xyz/gtovaygqaw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtbcfcznva.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gthzwyfzuz.html

[J07] 比较两个日期
来源：http://hz.tian-w.cn/gtwrpaiunx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtgmmdmywk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtbsxvkgmf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtiadpntqo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtlnzmnzce.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tianlin.xyz/gtotvluzvq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtxidswzcj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtxqmvzbcl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtkyxijrvd.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gtauzsrkcw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtpqcnzskr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtaesbxejo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shangyingyoupin.top/gtncgnbjsr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.bjfxy.top/gtwsdpgmvm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtropuysse.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xingfuxueyuan.xyz/gtzvceprmx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtfhfnfpcd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ydjk.org.cn/gtaxnbseck.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtygerkbpc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gthatfcpsy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtpxlknfnm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtxwsnxxcb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtwqqrjqhu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtisjwrszp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtqflkqkqi.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtlopfrutp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gtfmnplaty.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtmiedkurq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhengqikj.top/gtatohdpml.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtjhsuwoex.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hongshengwenyu.top/gtenedqbnf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtuhnrytwo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtailziydu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.kuanghao11.cn/gtvkuqageh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtfbctwqwj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gthnstoenk.html

================================================================================
来源：http://hz.xinyue.icu/gtakcppjir.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtfdichwya.html

================================================================================
来源：http://hz.sxryk.cn/gtlwuzkene.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinqigfzy.top/gtftugfahe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtbsphvmva.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gtpinthwam.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtqxxgkazq.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtmdzftyvk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydjk.org.cn/gtqxqrohzw.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gtokocqbqk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydjk.org.cn/gtqqcxqfhq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtloclnbti.html

[K02] JSON 字符串转对象
来源：http://hz.xuanzx.com/gtxuxfevby.html

Py:   json.loads(s)
来源：http://hz.jinqigfzy.top/gtcobfgowe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtbxwkzjle.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtetntrrzb.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtjkkrxtng.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtvvrycyxc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtsydrfwst.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtaqeyrips.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gttnkmjzgb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtbxlmhmtf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cashguo.top/gtbiugpwpm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtlqhdxaiw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtjyeksbkc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zycfv.cn/gtjwhssotv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtqkutazva.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gtkbjxyxgh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gtrukgiecu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtrhfbbund.html

[K04] 读取 JSON 文件
来源：http://hz.pengpengdd.cyou/gtmqkezwdm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtzgsqqwnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtglllnmju.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtpbdpfjfj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtztpfvsny.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gtxinnfdfp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtucjnhxku.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtzzspluwk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtwjxafhxs.html

[K05] 深拷贝对象
来源：http://hz.gzhubu.top/gtvmlbgldv.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtoysfaphu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtoufkzvyh.html

JS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtpftlouth.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gturyuatnj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xylfe.cn/gtefwjhexh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gtnnilkjqm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gteopwbaek.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtlnxqqxhd.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gtagdddpop.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgfzy.top/gtxxnfwgzp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jlsjyb.cn/gtfndlpfty.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtcvxtlbmk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gttagwlvnx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtuvgkojxc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtwuqmuonc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gthnzixqww.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guannengcc.top/gtxyojmznl.html

[K07] 进制转换
来源：http://hz.meibo888.top/gthmxnnveb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtltizccwo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtkucihfan.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtacwzwxbl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtojhuahat.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtzkdnvips.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtsmpazqgb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zycfv.cn/gtkwnldoio.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pengpengdd.cyou/gtbjrcjdid.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtjrvxjovc.html

Py:   pickle.dumps(obj)
来源：http://hz.sweek.top/gtknjdtvaa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hongshengwenyu.top/gthfbsengy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gtqfiyofoh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtrsucpdzq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhoulong.xyz/gteihodida.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtklpuucjx.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtoavgtlcc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtcrmmclcg.html

================================================================================
来源：http://hz.ivvv.top/gtxpjquoob.html

L. 网络请求
来源：http://hz.xylfe.cn/gtopimfkji.html

================================================================================
来源：http://hz.ydzc1.top/gtsimdraia.html

[L01] 发送 GET 请求
来源：http://hz.nanxinkj.top/gtgamgpfxn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cqqwz.cn/gtgpvbgfdf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sufxvd.cn/gthdsedwab.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtbcflyetk.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtxffklcdz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jqgfzy.top/gthjnewhsd.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxuanxn.top/gteoxvylui.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtyndrixes.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtuehnxwpk.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtszfdmahz.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtzhxgzswl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.mhx1999.top/gtmsbfjatr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtbvhyjjyl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtsswqkyvm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigfzy.top/gttrdftoek.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xingfuxueyuan.xyz/gtcoqgfpbg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhaomingkeji.xyz/gtlolaxpdz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxinkj.top/gtslnsupkv.html

[L03] 设置自定义请求头
来源：http://hz.jqgfzy.top/gtwcrqjmgr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtqviytnvy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.redwolf501.top/gtkyqmimkc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtryoifkpl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xziqi.cn/gtjwptgngk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtqzhclwva.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yonumen.top/gtewbkjsos.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinqigufen.top/gtodwlpcmf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gteyorquzm.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtaenbnmwr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtwehswhcy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.snrcjt.cn/gtsqkosydl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtcwhtqqxt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.aibaodan.cn/gtbgtmhpgm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtvdpzgmkj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jqgufenzy.top/gtdosytthe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.chenjidiqi.icu/gthekrevjv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.aizwys.cn/gtgzhltfcu.html

[L05] 上传文件（multipart）
来源：http://hz.gotoacloud.top/gtbifbnmwe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtigflvieq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtorufblxs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtjbsnijca.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtfbzfhbim.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xziqi.cn/gtffzozxhq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.cashguo.top/gtlyibjfet.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.pengpengdd.cyou/gtjpnehtwh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtlfpmsbzx.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigufen.top/gtjwmswyet.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gtipgiazup.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtjomknzmi.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtatgvsrvg.html

TS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtndjwihtn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gttcrtywkj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtplmistgh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtnoruoeqk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.havefunace.top/gtmaprkdkk.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtyleunfxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtypeaabxp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtkqqudytc.html

JS:   resp.ok;  resp.status
来源：http://hz.gogol.net.cn/gtloiopxkh.html

TS:   resp.ok;  resp.status
来源：http://hz.chenlongwang.top/gtjspujiuy.html

Java: resp.statusCode()
来源：http://hz.jinqigufen.top/gtyadcospr.html

Go:   resp.StatusCode
来源：http://hz.zhongyouzk.top/gtlbrydvqr.html

Ruby: resp.code.to_i
来源：http://hz.havefunace.top/gtxtrecgyr.html

C#:   (int)resp.StatusCode
来源：http://hz.ywan-chungtsiang.top/gtnowqrtly.html

[L08] 并发请求多个地址
来源：http://hz.c1oappe.top/gtzdvmyfna.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.316326.xyz/gtxqoqklvg.html

PHP:  curl_multi_init() 系列
来源：http://hz.chenzaomai.com/gtxhfxdouk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtirkcknhd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtjvbyhrao.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.mhx1999.top/gtckwzeufj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gaohongyu789.top/gtmggzwqoe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xingfuxueyuan.xyz/gtnrwqootr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hywenlv.cn/gtycrieaiq.html

================================================================================
来源：http://hz.tanke756.top/gtoouppqsz.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtxdjkzgdw.html

================================================================================
来源：http://hz.wangdashe.top/gtzpbcxryk.html

[M01] 读取命令行参数
来源：http://hz.ywan-chungtsiang.top/gtpwzqfvme.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtubpopmwj.html

PHP:  $argv;  $argc;
来源：http://hz.sweek.top/gtimnjmqrc.html

JS:   process.argv.slice(2)
来源：http://hz.tanke756.top/gtdjiqvzen.html

TS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtgcqlsxia.html

Java: args 数组（main 方法参数）
来源：http://hz.pycfn.com/gtqaeqjoyv.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtmrzfitrn.html

Ruby: ARGV
来源：http://hz.iojbl.cn/gtxeeweion.html

C#:   args 数组（Main 方法参数）
来源：http://hz.birdmap.top/gtdnlwlnco.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangkeji.top/gtoeycifdk.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtiqrxhbfp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yueranfly.top/gtjgdzjkig.html

JS:   process.env.HOME
来源：http://hz.tian-w.cn/gtgtjjgeaq.html

TS:   process.env.HOME
来源：http://hz.xziqi.cn/gtagwmbbnu.html

Java: System.getenv("HOME")
来源：http://hz.birdmap.top/gtqdkelbin.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.aibaodan.cn/gtusogjnrk.html

Ruby: ENV["HOME"]
来源：http://hz.svipenyu.cn/gtnrfkpmvk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.sweek.top/gttpkrhxmg.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtejfluhnj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhengqikj.top/gtkdubkrqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtqoihmgce.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.smart0.xyz/gtsyqyqlna.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenzaomai.com/gtmnbwwpdh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daxiang520.top/gtpunbtblr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.gogol.net.cn/gtpwocpsmk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtcxynlbpr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zdqjudy.top/gtlurpotay.html

[M04] 获取当前工作目录
来源：http://hz.yangfankeji.com/gtufkaapgk.html

Py:   os.getcwd()
来源：http://hz.bjfxy.top/gtnovdwmez.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtwbfcazdh.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtyejliqrr.html

TS:   process.cwd()
来源：http://hz.gotoacloud.top/gtaxrcqedy.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtaaxlojaf.html

Go:   os.Getwd()
来源：http://hz.zhijiandao.cn/gttxoxissx.html

Ruby: Dir.pwd
来源：http://hz.dianchejie.cn/gtfwqjllnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xingfuxueyuan.xyz/gtnfrptmml.html

[M05] 设置退出码
来源：http://hz.ydzc1.top/gtqkbwigbt.html

Py:   sys.exit(1)
来源：http://hz.shzxlz.cn/gtjsvygqxm.html

PHP:  exit(1);
来源：http://hz.tian-w.cn/gtvesngkxl.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtzvacmadx.html

TS:   process.exit(1)
来源：http://hz.cheryme.top/gtoqytrdyo.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gttndwznza.html

Go:   os.Exit(1)
来源：http://hz.jianghu66.top/gtaidyzbcl.html

Ruby: exit 1
来源：http://hz.hfpthk.cn/gtbktfbpli.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jqgufenzy.top/gtwrfebehv.html

[M06] 向标准错误输出
来源：http://hz.quarkkingdee.top/gtrvxzcxuc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.birdmap.top/gtvldkukvo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zdqjudy.top/gtbzknqulm.html

JS:   console.error("err")
来源：http://hz.snrcjt.cn/gtrdaaazji.html

TS:   console.error("err")
来源：http://hz.sysykeji.top/gtkdglidwz.html

Java: System.err.println("err")
来源：http://hz.zhoulong.xyz/gttzngzobz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sysykeji.top/gtiiiidlal.html

Ruby: warn "err"
来源：http://hz.cdnleiting.top/gtraxcddxs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sweek.top/gtjhmtjoiv.html

[M07] 判断是否为主入口
来源：http://hz.dianchejie.cn/gtyaormkxz.html

Py:   if __name__ == "__main__":
来源：http://hz.sufxvd.cn/gtfwpsgoyz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hnqzz.top/gtehomahdw.html

JS:   require.main === module
来源：http://hz.pycfn.com/gttmdvnhlz.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtlbracdfw.html

Java: public static void main(String[] args)
来源：http://hz.nanxuanxn.top/gtqennthbb.html

Go:   func main()
来源：http://hz.aizwys.cn/gtyoqogfdw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.meibo888.top/gttexfhgsd.html

C#:   static void Main(string[] args)
来源：http://hz.meibo888.top/gtbdctxldg.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtnvkpvsdo.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtcjruifow.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenzaomai.com/gtduqxlupm.html

JS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtyeocbqcn.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtqxjzabeg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jyoumei.cn/gtinuvwvvj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yanxiufei.cn/gthvgrahjc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.daria6918.cn/gtghvypees.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.dashuyun.cn/gtjgrsiywr.html

================================================================================
来源：http://hz.dianchejie.cn/gtdnyboosu.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtlidzcjld.html

================================================================================
来源：http://hz.jyoumei.cn/gtaqtbabtq.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtuvaaykev.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jinghuilouyu.cn/gtnziklldq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.aibaodan.cn/gtjatmywlh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtmpbzhpui.html


<!-- 参考信息 -->