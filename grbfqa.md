代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtegdiixid.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtesxxfonp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtdxqbrtjn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtuwyaqxpc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtofvjtpyx.html

[J04] 时间戳与日期互转
来源：http://hz.zhengqikj.top/gtcucstpod.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtikgtxbgo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.c1oappe.top/gtorhcnjyg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtmokeqgne.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtadbmjhsu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yuxming.cn/gtqbhigdln.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gthmlkerhz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj202588.top/gteiobhwkn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.andypj.xyz/gtztvnszwl.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtwvjffbwl.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtacdquczy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtyfhlgfcf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtziqhhohr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtklnlfddm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtmnznazjj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtqkqpswao.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sxryk.cn/gtnvebydat.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hywenlv.cn/gtkmxlblsv.html

[J06] 计算两时间之差
来源：http://hz.hnqzz.top/gtvmltdiix.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtgusbgtxb.html

PHP:  $end->diff($start)->days;
来源：http://hz.xuanzx.com/gttjdswuce.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.daria6918.cn/gtcergwewm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtejqavfxp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.iojbl.cn/gtartsrurt.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtqkzfrqwa.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtlutounih.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gthqhwuclb.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtgvmpzrft.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtkuvwafko.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtxtgiekxe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtikfvjpfw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtlarmlhvy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtygbokypk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtzcumunts.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtucqtkjbd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtahsypysk.html

[J08] 提取年月日与星期
来源：http://hz.yj20258.top/gtdbggdbkg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gthjipubuf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtmtshxnxf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtxvbtmgcm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtchprmfxt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtubsejjwb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtsjntzarb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtarocgvbk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtzgezobrc.html

[J09] 时区处理
来源：http://hz.sufxvd.cn/gtmxbjnvbg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtreumxqrr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gttmegrdmq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtfvbsrdxl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gttjpfkxax.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtlrkamcoq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gtqbyamqpl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtamtzltbb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jyoumei.cn/gtvysxbutt.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtjgmrsacb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.c1oappe.top/gtjgttexot.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gtuwopiehv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtrwrxbbyp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtyrfltjwn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tanke756.top/gtfazsqvlv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtxybwtmiz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gtyvrngvia.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gteqdcepmh.html

================================================================================
来源：http://hz.nwbrower.top/gtyjtezrgl.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gttoeudlho.html

================================================================================
来源：http://hz.shuidangran.top/gtiopyeyhf.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtyczuncsh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dianchejie.cn/gthyeoaxuo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtfwbqucfj.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gtqgkmlblf.html

TS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtmfbnzcfi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gttmqnotos.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtisguzgcb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtmyxjxmql.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenzaomai.com/gtfokzdvhq.html

[K02] JSON 字符串转对象
来源：http://hz.wangshuangyany.cn/gtjtcdliyr.html

Py:   json.loads(s)
来源：http://hz.tanke756.top/gtfhzzgjbb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shuidangran.top/gtegbvkdcs.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtqzybxpkw.html

TS:   JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtexvrqsur.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtcyklfiqc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtaqktqdlq.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtztpqrini.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtowikoabm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.dianchejie.cn/gtiwfajemg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtlulhehxl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtemxqfkxr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gthgmtdxhu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtxlqzpcaa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sysykeji.top/gtdgknfplt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gttwthmjcm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuanzx.com/gtqvwqnbpc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gtumtgikug.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtvjdlbwcd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.meibo888.top/gtnfomaywb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.meibo888.top/gtralruvgz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.daxiang520.top/gtnjvupzps.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtwqbslubh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sweek.top/gtosrkwpqw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtilmdwlcn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtxdrfyqlm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtevzynzsp.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtuspnmbbt.html

Py:   copy.deepcopy(obj)
来源：http://hz.gogol.net.cn/gtwgsbhlbb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtrxpnbvun.html

JS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtleeybyfu.html

TS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtxdibvgri.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gtmqxzrqom.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtusmheacl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtwyfiwsck.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtgaqbsbiv.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtnqyumseo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtklxfnztl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.bjfxy.top/gtyyvijxqf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtcptduixf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtknopftzh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtikgazoqt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtbhjjtqcp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtqnhrfluu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yueranfly.top/gtnymklkzv.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gthgvlblnw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yongpay.top/gtdvqenskz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.iojbl.cn/gttxcteapq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtcdoutmru.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtmqhsthag.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtilaheqon.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hywenlv.cn/gttkvjsvii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cheryme.top/gtrssvslwp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenlongwang.top/gtlaeqeizf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtpsohbomq.html

Py:   pickle.dumps(obj)
来源：http://hz.yanxiufei.cn/gtjcqzdyma.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sweek.top/gtegkpaulr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtdexfjthy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtyjjdfxbq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtdyyekwdw.html

Go:   encoding/gob
来源：http://hz.gzhubu.top/gtxsgtmimn.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gttkjudzqa.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenzaomai.com/gtzqmxwgco.html

================================================================================
来源：http://hz.cucudq.cn/gthafnsqmx.html

L. 网络请求
来源：http://hz.nwbrower.top/gtyixvuxpf.html

================================================================================
来源：http://hz.svipenyu.cn/gtcmrypofo.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtjoskrjcz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtiemuxobk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yanxiufei.cn/gtayspllas.html

JS:   await fetch(url)
来源：http://hz.birdmap.top/gtdgwhbwbj.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtrtqlofeg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtclvyzegd.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtwrcpexzt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtejyuuzdq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtsmrvwhsd.html

[L02] 发送 POST JSON
来源：http://hz.zycfv.cn/gtasosqcpj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.fzhhl.top/gtkkgnboun.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cashguo.top/gtnhhlkudl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.redwolf501.top/gtwauelaam.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtpzjncvwj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.iojbl.cn/gtsqtsemtx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shzxlz.cn/gtloxfpwwl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gtshvfbvgq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gteparbiax.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtniddbisl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhaomingkeji.xyz/gtibfzfyfd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.nanxinkj.top/gtqcbdrkas.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtsohizjlm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dashuyun.cn/gtrfyafcyy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhixingplan.top/gtpenvfzlt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtepskzffh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jiagoushi.top/gtbrjrrmzy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ivvv.top/gtcmqgiops.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gthzhzbwrj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gtqyltddrk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daxiang520.top/gtbqkhriei.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtnqcgdqov.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtadbvtjas.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.feifeiyinyue.top/gthdnwhgrw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtgvwwzmpc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtzylfbggf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtpvkdrcxc.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtfbauacyf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj20258.top/gttrhfuqjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.birdmap.top/gtkapwomjf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gttljdftob.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtrilkgcza.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtlxkqfdce.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtdgmwkbmq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtjnqrnbjv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtowkwjplx.html

[L06] 解析响应为 JSON
来源：http://hz.dashuyun.cn/gtuqwkbafk.html

Py:   resp.json()
来源：http://hz.tian-w.cn/gtgvdckzgq.html

PHP:  json_decode($body, true);
来源：http://hz.xingfuxueyuan.xyz/gtajxhlcgd.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtmxvwopfx.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtixxsavdp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtrycuihpj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.havefunace.top/gtewinpdub.html

Ruby: JSON.parse(resp.body)
来源：http://hz.vqdsnc.cn/gtiqpvsgnf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtvhazprrm.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtypopcfxy.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtfxidrftr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xziqi.cn/gtpiiqjrqz.html

JS:   resp.ok;  resp.status
来源：http://hz.bjfxy.top/gtegxlpbqy.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtvgxlhdsj.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtotdxxtuv.html

Go:   resp.StatusCode
来源：http://hz.hfpthk.cn/gtaaqetfkd.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtuhcnnwui.html

C#:   (int)resp.StatusCode
来源：http://hz.bjfxy.top/gtwhsepifb.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gttxmwwrbv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuetiantiany.cn/gtrpxqskpl.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtklbwbhld.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gttpkoprkd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hnxiangtu.top/gtneeegijd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gtrlkflhsc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtegmahafd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhijiandao.cn/gtpqebdfwi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gthjwubqrb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxjstsnxz.html

M. 命令行 / 进程 / 环境
来源：http://hz.jiagoushi.top/gtjwlnyzgt.html

================================================================================
来源：http://hz.snrcjt.cn/gtvfvtkesp.html

[M01] 读取命令行参数
来源：http://hz.gogol.net.cn/gtifwxtyvn.html

Py:   sys.argv[1:]
来源：http://hz.52xcode.cn/gtnygrquya.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtprszugys.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtsqkmprdp.html

TS:   process.argv.slice(2)
来源：http://hz.yongpay.top/gtxqbgeezh.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtbmpiuymd.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtaubbhkom.html

Ruby: ARGV
来源：http://hz.daxiang520.top/gtbrditoqh.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtdwnxwuwa.html

[M02] 读取环境变量
来源：http://hz.sufxvd.cn/gtlpytjeza.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258.top/gtoqixcsdk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gthnfndeec.html

JS:   process.env.HOME
来源：http://hz.meibo888.top/gtvacpvctx.html

TS:   process.env.HOME
来源：http://hz.daria6918.cn/gtevwvsoyb.html

Java: System.getenv("HOME")
来源：http://hz.yueranfly.top/gtxqmbhvcv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hfpthk.cn/gtcgmtnzfz.html

Ruby: ENV["HOME"]
来源：http://hz.hfpthk.cn/gtalgeovpi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigufen.top/gtrviterfp.html

[M03] 执行外部命令
来源：http://hz.jianghu66.top/gtsmggeoan.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.nwbrower.top/gtkcvxaoef.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xinyue.icu/gtcmwvjnya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtnsqgyjee.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtfdpfwncj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtfnoqkwnp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtbdzwuypt.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jyoumei.cn/gtlkzmsfow.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtfjkfefev.html

[M04] 获取当前工作目录
来源：http://hz.aibaodan.cn/gtgrjdsbqe.html

Py:   os.getcwd()
来源：http://hz.zhoulong.xyz/gtcjomjtze.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtmrqtjihd.html

JS:   process.cwd()
来源：http://hz.xuanzx.com/gtjghrqjjf.html

TS:   process.cwd()
来源：http://hz.shanyushiyangtech.top/gtgcjqepdg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gtbtxgfnzo.html

Go:   os.Getwd()
来源：http://hz.shuidangran.top/gtezwawbbv.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtbmpqlqgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtbojfrwdl.html

[M05] 设置退出码
来源：http://hz.cashguo.top/gtdknyxoma.html

Py:   sys.exit(1)
来源：http://hz.tanke756.top/gtdbtkqjyj.html

PHP:  exit(1);
来源：http://hz.yuanzhike.top/gtynplrxkr.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtefmgccsm.html

TS:   process.exit(1)
来源：http://hz.pycfn.com/gtfuucqfkl.html

Java: System.exit(1)
来源：http://hz.cqqwz.cn/gtoqflxlhs.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtbnrbjizg.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtdusqdzpu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gttmrlprpj.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtnkkzddyp.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yanxiufei.cn/gtiaesofvq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtuztvyeej.html

JS:   console.error("err")
来源：http://hz.fengsongda.top/gtxvbtouma.html

TS:   console.error("err")
来源：http://hz.zhijiandao.cn/gtpfuwkzgm.html

Java: System.err.println("err")
来源：http://hz.hnqzz.top/gtsevarute.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.cdnleiting.top/gtjjbjknnh.html

Ruby: warn "err"
来源：http://hz.sweek.top/gtktandtkw.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.9152youxi.cn/gtkpjbzfor.html

[M07] 判断是否为主入口
来源：http://hz.316326.xyz/gtppueyyll.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gtaiwgbndg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xinyue.icu/gttnbahzzk.html

JS:   require.main === module
来源：http://hz.aibaodan.cn/gthxwhhffo.html

TS:   require.main === module
来源：http://hz.nanxuanxn.top/gtgdarwhwo.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gtpeemcvkb.html

Go:   func main()
来源：http://hz.hnxiangtu.top/gtdiqfmufx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhaomingkeji.xyz/gtquypjftr.html

C#:   static void Main(string[] args)
来源：http://hz.gaohongyu789.top/gtbvqgimwj.html

[M08] 获取系统与运行时信息
来源：http://hz.xziqi.cn/gtsoiaerzl.html

Py:   platform.system();  platform.python_version()
来源：http://hz.gaohongyu789.top/gtttujxfmi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hnxiangtu.top/gtfgzrqyhj.html

JS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtopwaeowp.html

TS:   process.platform;  process.version
来源：http://hz.ydzc1.top/gtdezhohjt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtshadrcaj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.meibo888.top/gtfypiegzt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gtfcapvxcv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtpnyiwmxu.html

================================================================================
来源：http://hz.aizwys.cn/gtqdltqfad.html

N. 数据结构与算法
来源：http://hz.zycfv.cn/gtadfvrtgu.html

================================================================================
来源：http://hz.ehwqpu.com/gteztkakmr.html

[N01] 二分查找（有序数组）
来源：http://hz.ydzc1.top/gtwcklnmwy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xinyue.icu/gtehwgpzqw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258.top/gteyisddjo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtawhwxwjq.html


<!-- 参考信息 -->