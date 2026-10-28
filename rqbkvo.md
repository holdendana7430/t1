代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.316326.xyz/gtwnpvmqqs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gteprihsxy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtyoyemxzh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.svipenyu.cn/gtydglhjhq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtijlaontl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gtspzutrdf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtikzvrloh.html

[J06] 计算两时间之差
来源：http://hz.nwbrower.top/gtfzibvuyo.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtzmwmjrrb.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtwahemhre.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtxcnitxgr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtdurvmbbn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtmneglgdh.html

Go:   end.Sub(start).Hours()
来源：http://hz.gotoacloud.top/gthinhgfsn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.iojbl.cn/gtxdyrwile.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtrkhwuhjx.html

[J07] 比较两个日期
来源：http://hz.chenjidiqi.icu/gtwnptpiar.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtbceeodos.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuanzhike.top/gtsejdnhxd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtvqvpzuue.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtntgvljrr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtesxnfojr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xingfuxueyuan.xyz/gtswywnuax.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtiyqlukiw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtsvymjezi.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtckhhdqle.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtegrrewed.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hammf.cn/gtzfywpyzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtunpnrety.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shuidangran.top/gtpbrrpwwj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258888.top/gtqiwafwtg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtejkmmujo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtlvocxspa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtyphykvub.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtwhzerkgi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtydmfazji.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnxiangtu.top/gtueyvapym.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtstdtdkee.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtucpcvipw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtighdndbh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtfodtzibn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtjuknefst.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtcrdlfmhj.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gttmcxikgq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtaytmucrf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtkihrqspu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtvwzrasbi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hnqzz.top/gtzrmnhkwc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtqcqbkltc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtyosbwemw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtpcyhkzch.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tianlin.xyz/gtyutytxrh.html

================================================================================
来源：http://hz.zhengqikj.top/gtbjmtskyv.html

K. JSON 与序列化
来源：http://hz.dashuyun.cn/gtlsrtwxyc.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpdkmvhkb.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtaqtrtoun.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtvktibkgm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gttutlbmrx.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gthvrivvds.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtgbjkendo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gthhuloupk.html

Go:   json.Marshal(obj)
来源：http://hz.cqqwz.cn/gtyvuxchac.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtewjwehqv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xinyue.icu/gtpewzbadk.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtmqchtnab.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtiwpkbctv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtrqczzyoc.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtplxywqkd.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtjwsbdnfv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtyukaihuu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtlxdgfnvx.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtnixwinqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtlcvxlzvk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtophdscqs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtvadtiyri.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangtech.top/gthqtbfttv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jianghu66.top/gtrstfttrw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtsxbdoxrg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtublbtirr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gtciyfafsa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtzvqmxesu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sufxvd.cn/gtatxpgeaz.html

[K04] 读取 JSON 文件
来源：http://hz.fengsongda.top/gtrwiwyyon.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ywan-chungtsiang.top/gtdacvtsly.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtunebrtzq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtynaauuss.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gttkvfrxwz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtgpatobij.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuetiantiany.cn/gtxrjqnfjd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hammf.cn/gtzwqxziav.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtlhdnbazy.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtmsmozpqi.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtsdqxeoju.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xziqi.cn/gtcrkxugqg.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtnuxiixsq.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtankdtzbw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtvxrweajh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pengpengdd.cyou/gtxsavcmjj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtmfrgjfmu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtshrfndgz.html

[K06] 解析 URL 查询串
来源：http://hz.cashguo.top/gtfpxbcpkl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtdtxuovfv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gtoyhexrha.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gthsndncgd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtjxnzofkb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtxoqfomgm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtjoseppuw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtcpawwyfr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtmwevvoht.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtdsghuwnt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtspmvsqux.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.c1oappe.top/gtbddipuxz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtjghmkzsq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtmikvzdmm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtkuryrpdp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jianghu66.top/gturkpzrgu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtrsasjbee.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daria6918.cn/gtestrciwt.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinghuilouyu.cn/gtfhphqklp.html

Py:   pickle.dumps(obj)
来源：http://hz.9152youxi.cn/gtzuqggugv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gtulyfwctc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtrumrkana.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtcusfeqdf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nanxinkj.top/gtstaqqvxe.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtbzmidfpz.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtjjobofgk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gotoacloud.top/gttywnxrxc.html

================================================================================
来源：http://hz.fengsongda.top/gtuctgcuaq.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtrsmmdbne.html

================================================================================
来源：http://hz.ehwqpu.com/gtsqycfqld.html

[L01] 发送 GET 请求
来源：http://hz.zhijiandao.cn/gtfgzifocp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gteofifvny.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtdhndpvyf.html

JS:   await fetch(url)
来源：http://hz.cucudq.cn/gtgksaqytx.html

TS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtnviloywz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtgzailmml.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtqbrzjmld.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cucudq.cn/gtqszlflkl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtixsognma.html

[L02] 发送 POST JSON
来源：http://hz.dianchejie.cn/gtxfxutrgh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ydjk.org.cn/gttpuuqbms.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sweek.top/gtqnerecxi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shuidangran.top/gtuapkytzx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtdrgmyrot.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fzhhl.top/gtnaxnqlfc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtgfeacbtb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtjltfnlzc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenzaomai.com/gtlitmfzpt.html

[L03] 设置自定义请求头
来源：http://hz.tian-w.cn/gtsvxikkci.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cqqwz.cn/gtzuaiobdi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgufenzy.top/gttxgrudmk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtxwmvljwt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtxkfzhrvr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gttnssaowz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shuidangran.top/gtiwhuezxd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gthdztvgle.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtpezzujey.html

[L04] 设置超时
来源：http://hz.gotoacloud.top/gtipvgbgza.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtxnxhnicj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ppjwa.cn/gtofyctddm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zdqjudy.top/gtuwpgxcxa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.daria6918.cn/gtkhwvipyq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtjaynrejl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtgymnqojk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gtzeujgtgn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gaohongyu789.top/gteojsgwzb.html

[L05] 上传文件（multipart）
来源：http://hz.sysykeji.top/gtsaucrryt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gthpzzjwek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtjcwguzzc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jlsjyb.cn/gtvadcbcyq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gteluvbdrv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ehwqpu.com/gtowullyvy.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jiagoushi.top/gtjphzhtpj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dashuyun.cn/gtbhndbkhi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.wangshuangyany.cn/gttmpveznj.html

[L06] 解析响应为 JSON
来源：http://hz.shangyingyoupin.top/gtqucvhpbc.html

Py:   resp.json()
来源：http://hz.zhijiandao.cn/gtucejucfp.html

PHP:  json_decode($body, true);
来源：http://hz.gogol.net.cn/gtkjetcffe.html

JS:   await resp.json()
来源：http://hz.hfpthk.cn/gtmwovnevw.html

TS:   await resp.json()
来源：http://hz.sufxvd.cn/gtfuxuwpqp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yuanzhike.top/gtqirupazi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.dashuyun.cn/gtcyjukujr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtokweiopu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.andypj.xyz/gtrocvqvib.html

[L07] 处理 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtgiiztugr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gthwbjjtfq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ppjwa.cn/gtyscpeazx.html

JS:   resp.ok;  resp.status
来源：http://hz.zycfv.cn/gttxdyxvov.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigfzy.top/gtoxabdxub.html

Java: resp.statusCode()
来源：http://hz.cashguo.top/gtdkrnlbqf.html

Go:   resp.StatusCode
来源：http://hz.zhoulong.xyz/gtcawkhdbc.html

Ruby: resp.code.to_i
来源：http://hz.cqqwz.cn/gtcyfvymxa.html

C#:   (int)resp.StatusCode
来源：http://hz.c1oappe.top/gtqzywbexm.html

[L08] 并发请求多个地址
来源：http://hz.aizwys.cn/gtngsxcyyi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yanxiufei.cn/gtuzyfufhi.html

PHP:  curl_multi_init() 系列
来源：http://hz.tianlin.xyz/gtubrunrkb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gteptfcsyu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gtnmffiwpt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.shzxlz.cn/gtuvtvqkmb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhiwuduotai.top/gtexbisrhp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.dianchejie.cn/gtmoyepuya.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtjjmmawfv.html

================================================================================
来源：http://hz.fengsongda.top/gtxjjvnxjo.html

M. 命令行 / 进程 / 环境
来源：http://hz.kuanghao11.cn/gteurhojid.html

================================================================================
来源：http://hz.mhx1999.top/gtmdyfdfxg.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtzqikxpjd.html

Py:   sys.argv[1:]
来源：http://hz.yj20258888.top/gtmmurtfcn.html

PHP:  $argv;  $argc;
来源：http://hz.yanxiufei.cn/gtwmqmgyqo.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtvndkankw.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtgaykdeys.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxinkj.top/gtahvrunwy.html

Go:   os.Args[1:]
来源：http://hz.jiagoushi.top/gtqzkyrwwf.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtliwudval.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jyoumei.cn/gthwrigwgn.html

[M02] 读取环境变量
来源：http://hz.sysykeji.top/gtmyyforei.html

Py:   os.environ.get("HOME")
来源：http://hz.yanxiufei.cn/gtqxaqsuro.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtlxeoirsj.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtcjzvdxjk.html

TS:   process.env.HOME
来源：http://hz.xuanzx.com/gtqczsdcyg.html

Java: System.getenv("HOME")
来源：http://hz.yonumen.top/gtcrnvupgv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.svipenyu.cn/gtctarelsf.html

Ruby: ENV["HOME"]
来源：http://hz.tanke756.top/gtgdtkmhvr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.vqdsnc.cn/gttoojsvyo.html

[M03] 执行外部命令
来源：http://hz.jinqigufen.top/gtzggynbxf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jiagoushi.top/gtninsutog.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.xuanzx.com/gtexssnqdo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.316326.xyz/gtkzhdevic.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.pycfn.com/gtnfraczvh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xylfe.cn/gtfvuvjqyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinyuanbaomall.cn/gtxpbcseua.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.hywenlv.cn/gtameywequ.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ppjwa.cn/gtnpqcisic.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtqurgdcpp.html

Py:   os.getcwd()
来源：http://hz.feifeiyinyue.top/gtrjjzhyay.html

PHP:  getcwd();
来源：http://hz.yj20258.top/gtiizpstuz.html

JS:   process.cwd()
来源：http://hz.c1oappe.top/gtfsmysmgf.html

TS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtlrzcevnw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.gzhubu.top/gtbihcxxeg.html

Go:   os.Getwd()
来源：http://hz.hywenlv.cn/gtubuqrgpg.html

Ruby: Dir.pwd
来源：http://hz.zycfv.cn/gthvechonx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhijiandao.cn/gtyhlvkfzd.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtobnkxtbb.html

Py:   sys.exit(1)
来源：http://hz.shangyingyoupin.top/gtdrqbywhh.html

PHP:  exit(1);
来源：http://hz.zhiwuduotai.top/gtmdcvrrhj.html

JS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtlbtytsif.html

TS:   process.exit(1)
来源：http://hz.dashuyun.cn/gtagleokeo.html

Java: System.exit(1)
来源：http://hz.feifeiyinyue.top/gtnmhdbgpq.html

Go:   os.Exit(1)
来源：http://hz.havefunace.top/gttkgacgrv.html

Ruby: exit 1
来源：http://hz.jyoumei.cn/gtvawegzoh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.wangshuangyany.cn/gtbdaznvth.html

[M06] 向标准错误输出
来源：http://hz.feifeiyinyue.top/gttunhzqym.html

Py:   print("err", file=sys.stderr)
来源：http://hz.tanke756.top/gtedllevji.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtvkluzmsn.html

JS:   console.error("err")
来源：http://hz.jinqigufen.top/gtbjqfvelv.html

TS:   console.error("err")
来源：http://hz.yangfankeji.com/gtbloudgcv.html

Java: System.err.println("err")
来源：http://hz.guowangkeji.top/gtpmusscef.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.quarkkingdee.top/gtsexjuzyl.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtqlynolvs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtzdralhev.html

[M07] 判断是否为主入口
来源：http://hz.xingfuxueyuan.xyz/gtibwcgmss.html

Py:   if __name__ == "__main__":
来源：http://hz.dianchejie.cn/gtjdjlptfe.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.hfpthk.cn/gtwzwuadea.html

JS:   require.main === module
来源：http://hz.zhijiandao.cn/gtammctakn.html

TS:   require.main === module
来源：http://hz.xuanzx.com/gtigpitzff.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtxkkjhbjr.html

Go:   func main()
来源：http://hz.gotoacloud.top/gtfljroazi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cqqwz.cn/gtzjhbpfmb.html

C#:   static void Main(string[] args)
来源：http://hz.0kj1m.cn/gtpubqhmep.html

[M08] 获取系统与运行时信息
来源：http://hz.316326.xyz/gtgcwkdtly.html

Py:   platform.system();  platform.python_version()
来源：http://hz.wangdashe.top/gtijxbmxne.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.wangdashe.top/gtianenviu.html

JS:   process.platform;  process.version
来源：http://hz.sxryk.cn/gttrbyhffw.html

TS:   process.platform;  process.version
来源：http://hz.pengpengdd.cyou/gtsngpcbgd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.meibo888.top/gthkeqazbg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.316326.xyz/gtudejngae.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.smart0.xyz/gtvlfnkbuw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nanxuanxn.top/gtlxznuayq.html

================================================================================
来源：http://hz.chenzaomai.com/gtrasippwh.html

N. 数据结构与算法
来源：http://hz.dashuyun.cn/gtwfyskaps.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtcshuocgl.html

[N01] 二分查找（有序数组）
来源：http://hz.snrcjt.cn/gtdqfqovsh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.316326.xyz/gtqeymtmsv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.ywan-chungtsiang.top/gtmcsqojpe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gteuyoqsdl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtsfqyonoa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.daria6918.cn/gtkmklhunv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj202588.top/gtylcporiw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yueranfly.top/gtxvestvef.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.316326.xyz/gtfokrbets.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cheryme.top/gtjklcdzqj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtbutxmtnj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.kuanghao11.cn/gttvwflnbk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.wangshuangyany.cn/gtdutqokzs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gthcfkdlsl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtzwwidztq.html

Go:   slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtkegynntq.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtxeozwlkt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenjidiqi.icu/gtshmdvbwc.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtdzvazhyv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.andypj.xyz/gtyrwhmafs.html


<!-- 参考信息 -->