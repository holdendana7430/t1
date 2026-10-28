代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhongyouzk.top/gteclxeeeu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gthscnktbl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtpcnrufuq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.haohaochexian.top/gtrjncqjst.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtkfkjphfl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtxayprxji.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gtwtkrpvrk.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtmgqbaiby.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtutywylim.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtqdfncqec.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258.top/gtbjrkdird.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtvunftqje.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtgnkjdial.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtwigzqsol.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtedrnirnm.html

C#:   (end - start).TotalSeconds
来源：http://hz.xziqi.cn/gtvaagslqp.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtukqahgxm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gthnkghygs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtlnoeaetn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtsvcnjuxr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtqnulehgh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtrlblkhvw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yongpay.top/gtqnfinjbp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtpsnzvbll.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtordhauep.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtnabolqio.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtdghrqyby.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtlsvgwqmf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtxeymgoyp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtsrgdbecq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shuidangran.top/gtdkseozyd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.9152youxi.cn/gtnyhggscw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtcmflwqph.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtjvprkpob.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gthvxifisy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtjiaqezvx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtewmybfek.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtduwvqbhx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtbrsgaiil.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ywan-chungtsiang.top/gtslshsddi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtzsilvnes.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtfnrfgbtk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtqtjbizyg.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtyrloeuye.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gtqdflkqja.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gteuxnmofs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtmitlzhyy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtbvouqfrq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jiagoushi.top/gtorsfhvji.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtyurodhin.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sysykeji.top/gteosetavj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gttrrdtrwm.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtaidkzjig.html

K. JSON 与序列化
来源：http://hz.wangshuangyany.cn/gtqcguqtdz.html

================================================================================
来源：http://hz.jinqigfzy.top/gtcvufjorr.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtonqowcxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtstjhadbz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtasvpaeqt.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtqluskeac.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtnaamkahk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shangyingyoupin.top/gthfedhzho.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtcezcgpme.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangtech.top/gtgpgimien.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtvartknxw.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtisgiozat.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtfkefovbx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.havefunace.top/gtjlrgtbyr.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtcyqkqdaw.html

TS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gteuaagpfk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtjpftoevd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtmqmcqhpd.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtmmalwwrm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtnotgxaei.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtjjhtysqz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtqjbweafw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtheuaxazp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ppjwa.cn/gtihdxwokn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtuqltqxmq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.meibo888.top/gtkkrnnxue.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nwbrower.top/gtqgilmvak.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtjqdtmojk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtcxjrwvjc.html

[K04] 读取 JSON 文件
来源：http://hz.ivvv.top/gtmejkcxyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shanyushiyangtech.top/gtfmwckief.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtnvikjidi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtuiwlpuuf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtnqlehrks.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtphuzsdss.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtbespscal.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hfpthk.cn/gtpjquywpa.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtgwomabxa.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtbvhywcqt.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gtqwuehbpi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtsiglxujx.html

JS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtlpixnltm.html

TS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtpurkpuzo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtuoeipuyf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtrpvtosmi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhixingplan.top/gtqlgzsppl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtcsgtgbyx.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtbguqhkej.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guannengcc.top/gtiejuaffs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenjidiqi.icu/gtqchmfqeg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gttgvaxmmh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtnopsgjdf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtmrnynepj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtrfimysoc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daxiang520.top/gtydymoznm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.daxiang520.top/gtwzksivzn.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtsnxyjwqi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtprwgkpth.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gtzscstlzr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtzspwepum.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtvtfovhbl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gttqcqofwz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ehwqpu.com/gtcwgrzcog.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtilvtdoza.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.snrcjt.cn/gtbqvknrwo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtbwewusrh.html

Py:   pickle.dumps(obj)
来源：http://hz.jinghuilouyu.cn/gtlrqzrbbx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gteczlmcus.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtsvjjinsx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gteuxbfyef.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aibaodan.cn/gtaqtjwjsy.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtrukhfdti.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtxskihypz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pycfn.com/gtxmcszdey.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbqdmlqqp.html

L. 网络请求
来源：http://hz.yj20258888.top/gtzfsrrdfp.html

================================================================================
来源：http://hz.daria6918.cn/gtanafmhqi.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtyqlkewvv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nanxuanxn.top/gtcphepdps.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gttsbcjgxy.html

JS:   await fetch(url)
来源：http://hz.ivvv.top/gtcmttzkwy.html

TS:   await fetch(url)
来源：http://hz.yonumen.top/gtpumtelfq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.meibo888.top/gtxlgdvzpc.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtrcnolheg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gtzqmmnxji.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gtbcxppyec.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gtxdqbaxkc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.daria6918.cn/gtftyijppj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtgxgsuxlz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtrfnifsfd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtmlpozpls.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenjidiqi.icu/gtoiroqmbm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gterhrkhpo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtwiodxhof.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gtultgkipq.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtbnnutcoj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.pycfn.com/gtrnhvabca.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cashguo.top/gtyxsmwxkb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gteexqbohk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtrlmimafx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxuanxn.top/gthyxmbmrc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtplecslsr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtovrlnlvx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtvskhupgd.html

[L04] 设置超时
来源：http://hz.hammf.cn/gtdryxnjpv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.iojbl.cn/gtpvwoqllz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xingfuxueyuan.xyz/gtlnjvqipo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtpgwkigpl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtsduldbmi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yanxiufei.cn/gtqqpxvjjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.mhx1999.top/gtganmdjjz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtqudlmvtl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.snrcjt.cn/gtajacbxyr.html

[L05] 上传文件（multipart）
来源：http://hz.yj202588.top/gtoueytjxv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtkmfezvae.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtxositpsi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinghuilouyu.cn/gtlfwwbeyl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gthfhpmsug.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhoulong.xyz/gtsaeglljo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.guowangkeji.top/gtgisxltyx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zycfv.cn/gthtgqmmdq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xinyue.icu/gtnpwpwnzu.html

[L06] 解析响应为 JSON
来源：http://hz.yj202588.top/gtpamfffna.html

Py:   resp.json()
来源：http://hz.yanxiufei.cn/gtoftmltbh.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtektqegrf.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gtysbwhzqa.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtucmqjmps.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtwrwzshpb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxuanxn.top/gtzzhymkpc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangdashe.top/gtvcgrpebs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.svipenyu.cn/gtwudjrhzf.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtdxxmverq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.andypj.xyz/gtkewngbge.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.aizwys.cn/gtelgfrxww.html

JS:   resp.ok;  resp.status
来源：http://hz.yj20258888.top/gtvoaocauf.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtixkykglk.html

Java: resp.statusCode()
来源：http://hz.xingfuxueyuan.xyz/gtjgllhqpg.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtakioffpm.html

Ruby: resp.code.to_i
来源：http://hz.nwbrower.top/gtgzyoqstq.html

C#:   (int)resp.StatusCode
来源：http://hz.jiagoushi.top/gtrhgdxupj.html

[L08] 并发请求多个地址
来源：http://hz.jinghuilouyu.cn/gtkoewhazr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtovoxqxbk.html

PHP:  curl_multi_init() 系列
来源：http://hz.c1oappe.top/gtcjsrxolr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtnhhvwdqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinqigfzy.top/gtrvauawzp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hnxiangtu.top/gtzscxcjvo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtbbeufgaz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.redwolf501.top/gtkackjibq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xinyue.icu/gtberfdokj.html

================================================================================
来源：http://hz.ivvv.top/gtcwuhmxjz.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhaomingkeji.xyz/gtgbtncchx.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtekljgdjw.html

[M01] 读取命令行参数
来源：http://hz.zhixingplan.top/gtshlzgslv.html

Py:   sys.argv[1:]
来源：http://hz.shangyingyoupin.top/gtyrrbodub.html

PHP:  $argv;  $argc;
来源：http://hz.jlsjyb.cn/gtbtcktkbb.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtlbywdpvt.html

TS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtlzybewjz.html

Java: args 数组（main 方法参数）
来源：http://hz.chenlongwang.top/gtcrilbzpq.html

Go:   os.Args[1:]
来源：http://hz.meibo888.top/gtfawekvmh.html

Ruby: ARGV
来源：http://hz.sweek.top/gtktwikfeg.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jiagoushi.top/gtgiudmqfl.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtnosvgncp.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gtakutopzn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.andypj.xyz/gtlpeuztdg.html

JS:   process.env.HOME
来源：http://hz.316326.xyz/gtxswtsfwq.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtoedidqzt.html

Java: System.getenv("HOME")
来源：http://hz.guowangkeji.top/gtpzwplbbm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yonumen.top/gtkrojzabr.html

Ruby: ENV["HOME"]
来源：http://hz.gzhubu.top/gtmqbyahin.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuanzx.com/gttruxfhex.html

[M03] 执行外部命令
来源：http://hz.zhongyouzk.top/gtiwqytabc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.andypj.xyz/gtdatsnuvb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtlovljoow.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gtiygzqtma.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigfzy.top/gtycoffcdj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtgrbcxcpi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.sysykeji.top/gtvkbcvdks.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jqgufenzy.top/gtndvdrrgk.html

C#:   Process.Start("ls", "-l");
来源：http://hz.andypj.xyz/gtnnxqsniu.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtwedtbigp.html

Py:   os.getcwd()
来源：http://hz.yueranfly.top/gtjyadlhqf.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtfhabyfpj.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtiyaasmml.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gtpebxhhnj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.c1oappe.top/gtcppmvnvz.html

Go:   os.Getwd()
来源：http://hz.ehwqpu.com/gtiigdijqt.html

Ruby: Dir.pwd
来源：http://hz.xinyue.icu/gtfhkierej.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gogol.net.cn/gtovhurmkg.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtoitnguli.html

Py:   sys.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtyubpyezs.html

PHP:  exit(1);
来源：http://hz.havefunace.top/gtdfaggkeb.html

JS:   process.exit(1)
来源：http://hz.fengsongda.top/gtbslbilwa.html

TS:   process.exit(1)
来源：http://hz.cashguo.top/gtqhtgoxek.html

Java: System.exit(1)
来源：http://hz.cashguo.top/gtzvdvyubc.html

Go:   os.Exit(1)
来源：http://hz.jinqigfzy.top/gtnejfkfaf.html

Ruby: exit 1
来源：http://hz.ywan-chungtsiang.top/gtxyofvypt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sufxvd.cn/gtaikwxvnt.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtwcuvyhpc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.guannengcc.top/gtgvjtkvgb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtxjqfybpl.html

JS:   console.error("err")
来源：http://hz.aibaodan.cn/gtuegsiwzx.html

TS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtzftxgldd.html

Java: System.err.println("err")
来源：http://hz.0kj1m.cn/gtjgxogejc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtbvoumrpu.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gtdsssniyv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ppjwa.cn/gtluoldvzs.html

[M07] 判断是否为主入口
来源：http://hz.jlsjyb.cn/gtxnqtfbqv.html

Py:   if __name__ == "__main__":
来源：http://hz.ehwqpu.com/gtohxppxfu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gtjarqelnw.html

JS:   require.main === module
来源：http://hz.redwolf501.top/gtdzqvjnfv.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtxhtosxfw.html

Java: public static void main(String[] args)
来源：http://hz.hnqzz.top/gtkievmbyc.html

Go:   func main()
来源：http://hz.pycfn.com/gtxjtlhgkw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtomerbwku.html

C#:   static void Main(string[] args)
来源：http://hz.9152youxi.cn/gtdosvynnf.html

[M08] 获取系统与运行时信息
来源：http://hz.xuetiantiany.cn/gtbzazhfjw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yonumen.top/gtauymsygk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ydzc1.top/gtieobfktg.html

JS:   process.platform;  process.version
来源：http://hz.zhixingplan.top/gtxtdsgpdb.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtxpsthvnv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.ybcxt.top/gtguxrkohd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shanyushiyangkeji.top/gtnhxxhztr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.meibo888.top/gtcigggmap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gtbontuqru.html

================================================================================
来源：http://hz.smart0.xyz/gtfwkdmnej.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gturqlnddm.html

================================================================================
来源：http://hz.zycfv.cn/gtzltzgzdm.html

[N01] 二分查找（有序数组）
来源：http://hz.iojbl.cn/gthkmojoza.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hfpthk.cn/gtcnofgetc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jlsjyb.cn/gtgnwbpwpw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.316326.xyz/gtmmcutlfh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtbkmjakdf.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtkvlkvbej.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtzctgliwn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtscnvyvgq.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.cashguo.top/gtybybnwde.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.hywenlv.cn/gtsqksldml.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuxming.cn/gtpwzpawyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.hnxiangtu.top/gtthmtclpz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.guannengcc.top/gtguzpksfc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtqtonmrho.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtspjckbok.html

Go:   slices.Sort(arr)
来源：http://hz.zhixingplan.top/gtxzhergow.html

Ruby: arr.sort
来源：http://hz.jinyuanbaomall.cn/gtaxeuwspd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtfldqxzme.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtahkltqjz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ydjk.org.cn/gtfqyjyfwx.html


<!-- 参考信息 -->