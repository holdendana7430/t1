代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtzbxspdfy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtwppqtkty.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtgzzljmhb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtbpjmhdux.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtulkmdymo.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gttolqbucg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtdnmkzqcp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtahseglxh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenjidiqi.icu/gtbhqmrasn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xziqi.cn/gtdkmjdbqh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhongyouzk.top/gtgfkbjnep.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtsjgqtvpj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.redwolf501.top/gtbadikefp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ppjwa.cn/gtiguzpjjh.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtpjnweejt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtohokpvfx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtqshvcahu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtcnaipzpq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtgpmokunw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtflzbiiik.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtcqfgccum.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtoqpinsxr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtxmdokwow.html

[J10] 取今天 / 本月第一天
来源：http://hz.ppjwa.cn/gtrlgzcsog.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yangfankeji.com/gtfsllvaze.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtrhlferno.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtjuenlobc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtiazitsvu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtndqiwjef.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.daria6918.cn/gtnroxuzdc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtmbesrfop.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gtodsxsydr.html

================================================================================
来源：http://hz.yvedp.cn/gtwqdpiovy.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gthlipfxek.html

================================================================================
来源：http://hz.gzhubu.top/gtfzrutdrh.html

[K01] 对象转 JSON 字符串
来源：http://hz.yueranfly.top/gtbsfimzup.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtkrgehsej.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtfsactdkb.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtvhfumgbb.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtcyrlrfhs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtngpchgcn.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtfaqznqtf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtzivuobyi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtrlwfmquf.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtyebvzftp.html

Py:   json.loads(s)
来源：http://hz.fengsongda.top/gtxsvsjnwo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtwzukecyo.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gthwpsyklo.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtbkkldssl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtjosrfxch.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtfkgwkqjf.html

Ruby: JSON.parse(s)
来源：http://hz.guowangkeji.top/gtbzpvuxit.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yvedp.cn/gtnrlygtqi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtpvwqwgmv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtiavpqibp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.smart0.xyz/gtagpsjeme.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtkndqakik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtifrupjkt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtpcqqpzpm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gtwtwmncnp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yvedp.cn/gtcvrjdcye.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxuanxn.top/gtkvjhpzbd.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gtvtnsqqqs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jiagoushi.top/gtqmwvstee.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.birdmap.top/gtyzmgjacj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtzgnbsbej.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtyjnxtktw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guannengcc.top/gtmxrtwbsi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtddcnaudb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtdajtmqqc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gthuhkectx.html

[K05] 深拷贝对象
来源：http://hz.sufxvd.cn/gtrljtbltu.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangtech.top/gtkjqrhlks.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gthnchmdyk.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtwlcpohlu.html

TS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtkjhkutge.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gogol.net.cn/gtzjcwmqau.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.vqdsnc.cn/gtngxbanwe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtxclgjjlx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtewcuivdg.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gthqzsqujn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.vqdsnc.cn/gtvwldqoik.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtwqjnzcwa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtxtorvojq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gthcewiqii.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hfpthk.cn/gtiheaxrqv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtxcfjsckl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtvwjlhsly.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtfdjbapiv.html

[K07] 进制转换
来源：http://hz.redwolf501.top/gtvdccgrql.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tanke756.top/gtmfasjjst.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258.top/gtbznfptzt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtidmgalcp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtgcpiwluw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yonumen.top/gtpaezlgqa.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yueranfly.top/gtluhyigdy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtpkwyntpc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shuidangran.top/gturcxyyzg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtuhitttzd.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtuyyzjnse.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtunwuuiyc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtsrslotyi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gttebemsse.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ivvv.top/gtyffgxgyo.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtzzsujrzz.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtgcpcnvhl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shangyingyoupin.top/gtyhoxohem.html

================================================================================
来源：http://hz.316326.xyz/gtwbgxiiqp.html

L. 网络请求
来源：http://hz.yueranfly.top/gtmiqqekkd.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrpulzrvx.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtbfgekmcy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.svipenyu.cn/gtdpqojrwi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtrlikradb.html

JS:   await fetch(url)
来源：http://hz.ppjwa.cn/gtzvczwjka.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtpgxeaqcx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtzmbpyozn.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtnoaxgzka.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hysaishi.cn/gtycedpnpx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yanxiufei.cn/gtctnzfmtz.html

[L02] 发送 POST JSON
来源：http://hz.yongpay.top/gtefnwbbsa.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gzhubu.top/gtdiymbcbc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xziqi.cn/gtovsdhgur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtlpkwlbap.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtyawjpcpt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xingfuxueyuan.xyz/gtxctugpoe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gttivlvgkp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zycfv.cn/gtlfceyetp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.quarkkingdee.top/gtbflfhyxc.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtypvhnmxh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gtlgvbbeyq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenlongwang.top/gteenkgzxn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtilqcnftr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtktibtmzj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gthixdhido.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtdrkyucsv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtcmvspcka.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtrmzpdntp.html

[L04] 设置超时
来源：http://hz.hnqzz.top/gtbnbkrmmi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zdqjudy.top/gthrjyljts.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.xuanzx.com/gtqpipgypr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtsipngcaw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigufen.top/gtkslgabdj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gogol.net.cn/gtbneyjewn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gtesjfkonm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shangyingyoupin.top/gtebrrexpb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gttnkzxzru.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangkeji.top/gtjtcxhneu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgufenzy.top/gtqmclfhca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.feifeiyinyue.top/gtnebinclq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtueyasvok.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenzaomai.com/gtbrrzphjq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.guannengcc.top/gtvbnqqdur.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shanyushiyangtech.top/gtmfmbaitw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.vqdsnc.cn/gtjituwsge.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hysaishi.cn/gtjymopafs.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gthxmucbxe.html

Py:   resp.json()
来源：http://hz.gaohongyu789.top/gtmkfcbrte.html

PHP:  json_decode($body, true);
来源：http://hz.gogol.net.cn/gtiwohnlnx.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtjknkfrzz.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gtphdilxam.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jlsjyb.cn/gtjusodkef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtmzegjora.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtywnmuwpe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gtquuzfxng.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtbtsuvhyb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.chenjidiqi.icu/gtobujlkch.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jinyuanbaomall.cn/gtnhpvkaya.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtxempgmqx.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtsgzzobnn.html

Java: resp.statusCode()
来源：http://hz.hywenlv.cn/gtjfimiako.html

Go:   resp.StatusCode
来源：http://hz.xinyue.icu/gtrppvozds.html

Ruby: resp.code.to_i
来源：http://hz.hfpthk.cn/gtlbebjwcp.html

C#:   (int)resp.StatusCode
来源：http://hz.hysaishi.cn/gtxbtcrhdt.html

[L08] 并发请求多个地址
来源：http://hz.vqdsnc.cn/gtjntlubcp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtksatkrsa.html

PHP:  curl_multi_init() 系列
来源：http://hz.zdqjudy.top/gtetqowhmj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ppjwa.cn/gtmeivwldm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.bjfxy.top/gtfwkxzvat.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.dianchejie.cn/gtduzopqbk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.fzhhl.top/gtxyksofbl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtmymebzqt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.havefunace.top/gtdjzkllxg.html

================================================================================
来源：http://hz.jqgfzy.top/gtxjelsgfj.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhijiandao.cn/gtflffabbk.html

================================================================================
来源：http://hz.gogol.net.cn/gtqsucvhlz.html

[M01] 读取命令行参数
来源：http://hz.hywenlv.cn/gtbkoxfwzd.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtcykiauar.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtioqvnyuv.html

JS:   process.argv.slice(2)
来源：http://hz.chenlongwang.top/gtzpsvvguu.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtzhxowzji.html

Java: args 数组（main 方法参数）
来源：http://hz.vqdsnc.cn/gtuzlhyezu.html

Go:   os.Args[1:]
来源：http://hz.svipenyu.cn/gtnhxsssbj.html

Ruby: ARGV
来源：http://hz.yj20258888.top/gtrjecwllr.html

C#:   args 数组（Main 方法参数）
来源：http://hz.52xcode.cn/gtzdbpcaul.html

[M02] 读取环境变量
来源：http://hz.shanyushiyangtech.top/gtzdftjtte.html

Py:   os.environ.get("HOME")
来源：http://hz.xylfe.cn/gtoqrvgnva.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yj20258888.top/gtsjzodfvg.html

JS:   process.env.HOME
来源：http://hz.hywenlv.cn/gtcbrkxooq.html

TS:   process.env.HOME
来源：http://hz.jiagoushi.top/gtscwebmce.html

Java: System.getenv("HOME")
来源：http://hz.feifeiyinyue.top/gtocoljcxj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gthugwqerw.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gttherzpmj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtxrygirfp.html

[M03] 执行外部命令
来源：http://hz.dashuyun.cn/gtijanmnvf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.ppjwa.cn/gtrhhtmdbj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.vqdsnc.cn/gtmbbmqznw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtfelmzdhg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtndaghpvj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.mhx1999.top/gtestieezi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.havefunace.top/gtxwfunmaa.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gtkfgaajqf.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtainjzfvk.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtnguixjtn.html

Py:   os.getcwd()
来源：http://hz.wangdashe.top/gteuqqeqwy.html

PHP:  getcwd();
来源：http://hz.hywenlv.cn/gtfxxtrmmp.html

JS:   process.cwd()
来源：http://hz.hammf.cn/gtyegxqthv.html

TS:   process.cwd()
来源：http://hz.yuanzhike.top/gtwzujfhew.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtgrdnitxu.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtrpsbwske.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtiyqhdocz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtawcrfbdv.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gtpwmondse.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtsgufqjmb.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gttesoknfh.html

JS:   process.exit(1)
来源：http://hz.chenzaomai.com/gtzrfrlytz.html

TS:   process.exit(1)
来源：http://hz.tian-w.cn/gtrgqecmpm.html

Java: System.exit(1)
来源：http://hz.gzhubu.top/gtppmvfkcy.html

Go:   os.Exit(1)
来源：http://hz.yj202588.top/gthkbflmxr.html

Ruby: exit 1
来源：http://hz.xylfe.cn/gtlcgpqkon.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258.top/gtcxnpyjyu.html

[M06] 向标准错误输出
来源：http://hz.vqdsnc.cn/gtyuvswydw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.kuanghao11.cn/gtblmirtgw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xziqi.cn/gtarpkyzxx.html

JS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtldleinrt.html

TS:   console.error("err")
来源：http://hz.dianchejie.cn/gthalddpvv.html

Java: System.err.println("err")
来源：http://hz.dianchejie.cn/gtrztnegne.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.hongshengwenyu.top/gtraoncywj.html

Ruby: warn "err"
来源：http://hz.xingfuxueyuan.xyz/gtawywotfc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.redwolf501.top/gtopwjcenr.html

[M07] 判断是否为主入口
来源：http://hz.hysaishi.cn/gtoibsgacr.html

Py:   if __name__ == "__main__":
来源：http://hz.kuanghao11.cn/gtrcoiyned.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.havefunace.top/gtgxfbvazq.html

JS:   require.main === module
来源：http://hz.aizwys.cn/gtknzrikrn.html

TS:   require.main === module
来源：http://hz.jinqigufen.top/gtiriqbsoy.html

Java: public static void main(String[] args)
来源：http://hz.zycfv.cn/gtlnjlpiur.html

Go:   func main()
来源：http://hz.quarkkingdee.top/gtamcypmoq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zycfv.cn/gtwihwibgj.html

C#:   static void Main(string[] args)
来源：http://hz.haohaochexian.top/gtkputimjf.html

[M08] 获取系统与运行时信息
来源：http://hz.shuidangran.top/gtdwugmbqg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.guannengcc.top/gtbicgfytq.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xinyue.icu/gthrsrxvjx.html

JS:   process.platform;  process.version
来源：http://hz.yvedp.cn/gtsyezbrfw.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtnozuznhz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhongyouzk.top/gtdfuttkwz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.redwolf501.top/gtcjnmjqgi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gtoedawisk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.chenjidiqi.icu/gtboghxptw.html

================================================================================
来源：http://hz.nwbrower.top/gtlxxkntoa.html

N. 数据结构与算法
来源：http://hz.yvedp.cn/gtuvkxjdip.html

================================================================================
来源：http://hz.ydjk.org.cn/gtewzjtpce.html

[N01] 二分查找（有序数组）
来源：http://hz.shangyingyoupin.top/gtlnrzgrnw.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hnxiangtu.top/gtnldnbcxt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.xylfe.cn/gtrpvtlreh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.smart0.xyz/gtgkhypphg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.daria6918.cn/gtvwxfegnr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.nanxuanxn.top/gtfrkjbypz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtpqnkehyq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ppjwa.cn/gtdnyssnaj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shangyingyoupin.top/gtmlnupoga.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gttaujsbil.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtygoexrbq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xinyue.icu/gthrxhuzfj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtphloxemj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtnzdmkdhk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.yongpay.top/gtnvsvqrgy.html

Go:   slices.Sort(arr)
来源：http://hz.hongshengwenyu.top/gtwyswcsbl.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtqzmearax.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jlsjyb.cn/gtjpfahnoa.html

[N03] 快速排序（分治示例）
来源：http://hz.cqqwz.cn/gtrbhugoqb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.ywan-chungtsiang.top/gthehmgltv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtmxfbhxzz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xingfuxueyuan.xyz/gtmhiqvvnr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuanzx.com/gtlksodgvu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.redwolf501.top/gtzudjnimd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.smart0.xyz/gtrqkjrrox.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nwbrower.top/gtbeayolga.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yvedp.cn/gtmlecvxjj.html

[N04] 斐波那契数列
来源：http://hz.tianlin.xyz/gtckyvdich.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.hnxiangtu.top/gtwvgtsnhz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nanxinkj.top/gtlpvnudwp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zdqjudy.top/gtgrvukqvu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gttdsehxqk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.shangyingyoupin.top/gtwtorkcpy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.cdnleiting.top/gthroppqeg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtapsntdst.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.kuanghao11.cn/gtlkfcsvan.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gthvawwnuy.html

Py:   math.gcd(a, b)
来源：http://hz.yuanzhike.top/gtgylovedy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.kuanghao11.cn/gtxypifbvj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hnqzz.top/gtsvqivtjn.html


<!-- 参考信息 -->