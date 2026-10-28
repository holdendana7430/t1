代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtxbrjagmp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinyuanbaomall.cn/gtyfmcisbi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xingfuxueyuan.xyz/gtudgpxhgj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtplvnvnjv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtnthqknxm.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtnagarejb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtprvqdrhy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.vqdsnc.cn/gtyudmjjow.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhoulong.xyz/gtdochyjyd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnxiangtu.top/gtrhmmiznr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tianlin.xyz/gtymdjgdke.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gthncpznln.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhongyouzk.top/gthnlyczgg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtnhnjywiv.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gthcylbatn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtcacmjczo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtazdljzux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtvmrgrhyk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gzhubu.top/gtnosupyxu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtdacbnqie.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtheeksxwp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtuczrrjni.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gttxyezjow.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gtxrkxzybn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhaomingkeji.xyz/gtealujjxz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yvedp.cn/gtlooiwrgc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.andypj.xyz/gtbgdvekzu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zycfv.cn/gteffklmlu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gtquluropj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tianlin.xyz/gtogcajyzq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtburbiwkc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtirgkjlyj.html

================================================================================
来源：http://hz.zhongyouzk.top/gtijewsuhr.html

K. JSON 与序列化
来源：http://hz.zhijiandao.cn/gtjzwgimfj.html

================================================================================
来源：http://hz.sxryk.cn/gtfuhewlcz.html

[K01] 对象转 JSON 字符串
来源：http://hz.redwolf501.top/gtxsqflopw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtwasdekca.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtndkzdqbj.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtoaizdmbu.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtnzrzcrii.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtvrcjyrgz.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtvictaxzz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtwmqvxicz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtwcekijbc.html

[K02] JSON 字符串转对象
来源：http://hz.wangdashe.top/gtlbaplfzu.html

Py:   json.loads(s)
来源：http://hz.zhengqikj.top/gtxbwasvhe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtxpzjhjnw.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtqqbbevef.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtuzqklbzi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtvppyxwil.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtkfmknmmc.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtsxkgjcbk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gttowqvmht.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtahdapssc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtqbkhntaa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gttkkjnfqg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtdzbxehxu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtvffmvhof.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtowbspnqu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtvfureqbe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258888.top/gthltwywfy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtrjhwbjdg.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtccuobwuc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtbgblcgtk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gtfxguijib.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtnkekltnt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtebxrkjpa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtrxoetumm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtrvfafoql.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.guannengcc.top/gtunkhxiot.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.vqdsnc.cn/gtiqmdllsb.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtucffghoq.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtrafvvcfu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtqjfhbmlq.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gthqoohuwl.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtlefeizmn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.havefunace.top/gtdbxckdee.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.daxiang520.top/gtxkpcwdce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtaueslhdb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtxlyiwwtf.html

[K06] 解析 URL 查询串
来源：http://hz.svipenyu.cn/gtnlixbshn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ivvv.top/gtrfzpfyhp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtobzqgvkn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yanxiufei.cn/gtweunzfrv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gtcpgmctdv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtqbjyztsi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.bjfxy.top/gtzpobpnvu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtkpxheoat.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtscurbhjd.html

[K07] 进制转换
来源：http://hz.mhx1999.top/gtcsvmwkmx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj202588.top/gtqgjmvuoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hywenlv.cn/gtscuhfqjj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtrtyksajh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtxmndmggx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtfweagtcw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigfzy.top/gtyymwudso.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gthvfovuga.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtfoancvma.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtggxukdca.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtrnfgfvzg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hfpthk.cn/gtjgzizmon.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtwexoqgls.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sxryk.cn/gtadkimevn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.bjfxy.top/gtllfmfiqs.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtgucbhtpf.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtathxiyqb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gtfwfhsygh.html

================================================================================
来源：http://hz.smart0.xyz/gthkzzryue.html

L. 网络请求
来源：http://hz.cucudq.cn/gtyqpwkfnq.html

================================================================================
来源：http://hz.hywenlv.cn/gtepyirqkk.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtrdlcvdhf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj202588.top/gtryucdlex.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.birdmap.top/gtlmmhrkgv.html

JS:   await fetch(url)
来源：http://hz.zdqjudy.top/gthorozkng.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtccsmtuwo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhoulong.xyz/gtkrrzdjml.html

Go:   resp, err := http.Get(url)
来源：http://hz.svipenyu.cn/gtjdfolnpz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtrwnpaxiv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gtiosmjaoh.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtkhveqbyq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtmkjdasuj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtyvhsatab.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtbrptpvbz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.iojbl.cn/gtyefangcp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtiidqjpvb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.iojbl.cn/gtqxyeluso.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtomhxrauz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gtrvsfrwnr.html

[L03] 设置自定义请求头
来源：http://hz.shzxlz.cn/gtlvfmwkmo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtjrbvwfkg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtxpwdiqts.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtemoxbjsc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtpodgpqgs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtwezwozvs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gotoacloud.top/gtgikjhmvg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtmryzovzm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.svipenyu.cn/gtlsvzkugu.html

[L04] 设置超时
来源：http://hz.hammf.cn/gtbuykbtgj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtesmkazvj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtfxwrawrs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gteiymdhqw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtzbgthgwb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jqgufenzy.top/gthgweuwju.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gtsoqmnkdz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cheryme.top/gtlrgemcxo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.pengpengdd.cyou/gtnuwktyqe.html

[L05] 上传文件（multipart）
来源：http://hz.chenzaomai.com/gtcjoupywd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yanxiufei.cn/gtzwifcrdq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yvedp.cn/gtmurnkans.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtvkrrxjxy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xuetiantiany.cn/gtwmoyycnb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yueranfly.top/gtbbksbllx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xingfuxueyuan.xyz/gtsxwppsme.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.fzhhl.top/gtopdyugof.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yanxiufei.cn/gtahupfibs.html

[L06] 解析响应为 JSON
来源：http://hz.quarkkingdee.top/gtkbbmkjbu.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtcaxousmf.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtrgonhdhz.html

JS:   await resp.json()
来源：http://hz.daxiang520.top/gtoadlqyzw.html

TS:   await resp.json()
来源：http://hz.fengsongda.top/gtlbokhvzm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jiagoushi.top/gtqdhzvjig.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.haohaochexian.top/gthddnhzji.html

Ruby: JSON.parse(resp.body)
来源：http://hz.snrcjt.cn/gttuqcejqh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zycfv.cn/gtddhuyjzh.html

[L07] 处理 HTTP 状态码
来源：http://hz.shangyingyoupin.top/gtmpubzqvn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jqgufenzy.top/gthsyxwdhs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ivvv.top/gthdhgeafl.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtdltzubkb.html

TS:   resp.ok;  resp.status
来源：http://hz.cheryme.top/gtjyljuvje.html

Java: resp.statusCode()
来源：http://hz.meibo888.top/gtwhbonwlk.html

Go:   resp.StatusCode
来源：http://hz.tianlin.xyz/gtiskuclmf.html

Ruby: resp.code.to_i
来源：http://hz.shangyingyoupin.top/gtgqjjpeha.html

C#:   (int)resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtdypdtvys.html

[L08] 并发请求多个地址
来源：http://hz.shuidangran.top/gtljnoqiwk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yuanzhike.top/gtouzrzttj.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtppgdzzrh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jianghu66.top/gtfiwotovn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenzaomai.com/gtrdavwurr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jyoumei.cn/gtxtmfwvro.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yvedp.cn/gtjcfbsxmp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.cucudq.cn/gtdiccwwqr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.chenlongwang.top/gtslcqojfd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkxiqpwjc.html

M. 命令行 / 进程 / 环境
来源：http://hz.xingfuxueyuan.xyz/gtfnnsnbgj.html

================================================================================
来源：http://hz.birdmap.top/gtkpxhxfeh.html

[M01] 读取命令行参数
来源：http://hz.hnxiangtu.top/gtsegohtkk.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtbzlztvds.html

PHP:  $argv;  $argc;
来源：http://hz.hnxiangtu.top/gtzlljieoy.html

JS:   process.argv.slice(2)
来源：http://hz.tianlin.xyz/gtbyqwkzaf.html

TS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtvfzvjwtx.html

Java: args 数组（main 方法参数）
来源：http://hz.fengsongda.top/gttanburcs.html

Go:   os.Args[1:]
来源：http://hz.yj20258888.top/gtnczfeghm.html

Ruby: ARGV
来源：http://hz.snrcjt.cn/gtyflicrln.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtbjpupnaz.html

[M02] 读取环境变量
来源：http://hz.hywenlv.cn/gtkfxjubth.html

Py:   os.environ.get("HOME")
来源：http://hz.tian-w.cn/gttferuaur.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yangfankeji.com/gtrbndtfzg.html

JS:   process.env.HOME
来源：http://hz.xziqi.cn/gtfacqezdk.html

TS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtjboxdsuv.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtzrbzpwgg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ybcxt.top/gtsujtemil.html

Ruby: ENV["HOME"]
来源：http://hz.vqdsnc.cn/gtqvklrsdc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xuetiantiany.cn/gturdscvhi.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtvfvhxofp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sufxvd.cn/gtxumzcgsd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.fengsongda.top/gtxfvecxsy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.guowangkeji.top/gtcnnpqtik.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhixingplan.top/gthtsqotjd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.nanxuanxn.top/gtnrearpde.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jinqigufen.top/gtcxgdbrqo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhijiandao.cn/gtdifjavdy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.cashguo.top/gtdrgjrdth.html

[M04] 获取当前工作目录
来源：http://hz.hywenlv.cn/gtgcalmkua.html

Py:   os.getcwd()
来源：http://hz.c1oappe.top/gtztxncgrf.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtvipilnnj.html

JS:   process.cwd()
来源：http://hz.iojbl.cn/gtogbkvkce.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gthfkpnuby.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jianghu66.top/gtkgilygab.html

Go:   os.Getwd()
来源：http://hz.redwolf501.top/gtkiwfddgb.html

Ruby: Dir.pwd
来源：http://hz.cdnleiting.top/gtvcutdcrt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.iojbl.cn/gtcffdxmhd.html

[M05] 设置退出码
来源：http://hz.kuanghao11.cn/gtwebuvyqn.html

Py:   sys.exit(1)
来源：http://hz.cdnleiting.top/gtpyeqolry.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtvqgmpbcf.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtabqhzddk.html

TS:   process.exit(1)
来源：http://hz.c1oappe.top/gttpyhuumz.html

Java: System.exit(1)
来源：http://hz.jqgufenzy.top/gtjlsjbngv.html

Go:   os.Exit(1)
来源：http://hz.redwolf501.top/gtfopheubc.html

Ruby: exit 1
来源：http://hz.xinyue.icu/gtzrrartwy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.0kj1m.cn/gtaeoanuib.html

[M06] 向标准错误输出
来源：http://hz.hnqzz.top/gtsnclpfbg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.iojbl.cn/gtrsjwhusa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtnetludfn.html

JS:   console.error("err")
来源：http://hz.ivvv.top/gtppfauxqi.html

TS:   console.error("err")
来源：http://hz.jinqigufen.top/gtgewnoveo.html

Java: System.err.println("err")
来源：http://hz.sweek.top/gtlppwlbku.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtybtmuuna.html

Ruby: warn "err"
来源：http://hz.gzhubu.top/gtrxdchzol.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtzcxvjzoa.html

[M07] 判断是否为主入口
来源：http://hz.guannengcc.top/gtuamhmkmt.html

Py:   if __name__ == "__main__":
来源：http://hz.52xcode.cn/gtnjzwnyvp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.feifeiyinyue.top/gtqkljtgzc.html

JS:   require.main === module
来源：http://hz.0kj1m.cn/gtqzpsxayk.html

TS:   require.main === module
来源：http://hz.yj20258888.top/gtbbjqypjq.html

Java: public static void main(String[] args)
来源：http://hz.wangshuangyany.cn/gtckxcwawz.html

Go:   func main()
来源：http://hz.jiagoushi.top/gtzzzwbdnv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.sxryk.cn/gtiougmtol.html

C#:   static void Main(string[] args)
来源：http://hz.jqgufenzy.top/gtufgzsxhr.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtackzbccq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuanzhike.top/gtlhlgghfw.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xinyue.icu/gtxrxwsvar.html

JS:   process.platform;  process.version
来源：http://hz.guannengcc.top/gtlixcgnbp.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtvywpofas.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.yj20258888.top/gtdlpriszy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigufen.top/gtkrksmxhv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtnrqixziu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtlaqnzksu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtgucortag.html

N. 数据结构与算法
来源：http://hz.yongpay.top/gtdqgdrvsf.html

================================================================================
来源：http://hz.cashguo.top/gtuworsmbr.html

[N01] 二分查找（有序数组）
来源：http://hz.wangdashe.top/gtwixqnjwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtkwqtwugs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cashguo.top/gtxuqfiigc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ppjwa.cn/gtnvkpqhdn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.pengpengdd.cyou/gtxzhirepn.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.cdnleiting.top/gtftgqyajx.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtgbsbunyq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ehwqpu.com/gtmvobtqxc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtjojkkjta.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.aizwys.cn/gtkckfzgca.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zdqjudy.top/gttqaufzfn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.haohaochexian.top/gtflgjiskb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtrvawqstl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.daxiang520.top/gtbxepuwpz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydjk.org.cn/gtfheqwokb.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtlkivmwzc.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtpilwsgdk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ehwqpu.com/gtbxgepvkm.html

[N03] 快速排序（分治示例）
来源：http://hz.chenzaomai.com/gtvfkdbfbb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yueranfly.top/gtyyjxyfhf.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xinyue.icu/gtgrqclxcc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtgmlsekrr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtopeoidwe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.gogol.net.cn/gtsuazmvbh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.ywan-chungtsiang.top/gthshfzrgj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yongpay.top/gtwjgqruix.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hysaishi.cn/gtxennmdmr.html

[N04] 斐波那契数列
来源：http://hz.smart0.xyz/gthmocopru.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.shangyingyoupin.top/gtgyljenzr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hammf.cn/gtfyzvalmd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.nwbrower.top/gtynjfefqy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtkylzwbqz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.daxiang520.top/gtinfytljr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ivvv.top/gtlpqwzbyy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.cashguo.top/gtvlsvpuxi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shuidangran.top/gtbeaocyld.html

[N05] 最大公约数
来源：http://hz.aizwys.cn/gtvftovxwg.html

Py:   math.gcd(a, b)
来源：http://hz.ppjwa.cn/gtekanpxnq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.cashguo.top/gtthykydmy.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.ybcxt.top/gtsjhutcwq.html


<!-- 参考信息 -->