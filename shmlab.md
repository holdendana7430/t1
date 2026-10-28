代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtstkcpjgm.html

[J08] 提取年月日与星期
来源：http://hz.zhongyouzk.top/gtlyoffuih.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtonsdbyxe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhixingplan.top/gtphyltzur.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jianghu66.top/gtdofutkgr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj20258888.top/gtenywvwqi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtqamytsma.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtbjjyoenf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tianlin.xyz/gttobovuug.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yuanzhike.top/gtmthwjmfw.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtzysfkdie.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtxzehytss.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtuxepbigh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtjwoxkcnu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtidwpdnjr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtptkdgayc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtztncmxtx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtsgteyhte.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtltctzipe.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtcmbtzpys.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtshhcsmnm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtbkhloexr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj202588.top/gtfysyujst.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jyoumei.cn/gtlqgtmwed.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtovfbbdnk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gthcezyrim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gttyhlzrwr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shuidangran.top/gtyugmhvwo.html

================================================================================
来源：http://hz.havefunace.top/gtsdzzgtty.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtmhvqzouj.html

================================================================================
来源：http://hz.yongpay.top/gtjlaibcwe.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gtwyzjksbb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtjvewrqar.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtbuontzwr.html

JS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtcbjlxghp.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtjfpxnqnl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtcigckvvl.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtprxgnose.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtfrgcwoay.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.meibo888.top/gtdsnqekgo.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtmbczyjgi.html

Py:   json.loads(s)
来源：http://hz.yangfankeji.com/gtnycvacat.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtwqmgkoty.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtbminuaom.html

TS:   JSON.parse(s)
来源：http://hz.snrcjt.cn/gtebmunjhh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuxming.cn/gtobszgbtc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtotfohylx.html

Ruby: JSON.parse(s)
来源：http://hz.zhengqikj.top/gtjfzxnhmu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258.top/gtkohgbfho.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtwaofwynf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtvoudtxes.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtucsihirs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtqmtioodo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtmwtchyuw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gtyajqlhvg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.316326.xyz/gtlgjesgab.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtfpuggxrg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shangyingyoupin.top/gtcdnvunoz.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtmgnediza.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtsgdktlgf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gthltzcwdb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtwrkldmcr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gthgnyzpfi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtsaozwwre.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtnwwojcng.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sysykeji.top/gtzjtwjygf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.9152youxi.cn/gtddzhruhz.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gteyfyprzl.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gtlnhvshul.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtaohnpcsw.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtnvgxuchf.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtwrokkoxh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gttfawubqf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtxlkjrdnv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tianlin.xyz/gtryootdni.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cheryme.top/gtfniwfgud.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gttifnflii.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtjkcdbnbz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtufmwlpna.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtummyczwf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtjgpscbig.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhongyouzk.top/gtapmmpkjd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtkjuvqxtx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.316326.xyz/gtwoggcikw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yj202588.top/gtssawxnak.html

[K07] 进制转换
来源：http://hz.chenjidiqi.icu/gthdwrjwwk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtxyhqvlir.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yuxming.cn/gtyhwanykz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtlwbtkbso.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtwlkogabs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtcmdxnfxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.vqdsnc.cn/gtuehlrbuv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gtkbnkavkb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gtfgmpqmoy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtemgesbpw.html

Py:   pickle.dumps(obj)
来源：http://hz.dianchejie.cn/gtvsyydnnk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.svipenyu.cn/gtilhrrrvv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtfvstafdf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtnihuxvrn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtusgolagr.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtbgxtgyfv.html

Ruby: Marshal.dump(obj)
来源：http://hz.ppjwa.cn/gtqsgixnqo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sufxvd.cn/gtimgpqums.html

================================================================================
来源：http://hz.316326.xyz/gtkpxmkryt.html

L. 网络请求
来源：http://hz.birdmap.top/gtvpqehuzw.html

================================================================================
来源：http://hz.redwolf501.top/gtdymxbixa.html

[L01] 发送 GET 请求
来源：http://hz.0kj1m.cn/gtsufjfqyd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtauoapdpc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtrzfhiozq.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtcqcewkvm.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtmvbgttji.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dashuyun.cn/gtfrsmihpf.html

Go:   resp, err := http.Get(url)
来源：http://hz.gogol.net.cn/gtiamuejmo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtzsxiephq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yanxiufei.cn/gttccsznoq.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtfhjhgdig.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.feifeiyinyue.top/gtmzgvlluf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtuqdrnlvw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xingfuxueyuan.xyz/gtburrtldz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtrrwiyrtr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtunfvnugc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guowangkeji.top/gtvdmvqkab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yanxiufei.cn/gtkxakyrmh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhiwuduotai.top/gtcyeivotr.html

[L03] 设置自定义请求头
来源：http://hz.gogol.net.cn/gtttsegfrv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.shanyushiyangkeji.top/gtqqbbvsvk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.havefunace.top/gtplaxkbmh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtmeodjglr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtnndpymcc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gtgcwatuwi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gteglqdxql.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ehwqpu.com/gtxubfzmjz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gthqpnqlgk.html

[L04] 设置超时
来源：http://hz.cucudq.cn/gtuqvnwkks.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sxryk.cn/gtyrhxqhya.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuxming.cn/gtusjcakct.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtnnreaftb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtjmzqrkid.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ywan-chungtsiang.top/gtvfmibgxm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yueranfly.top/gtjtplhils.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shangyingyoupin.top/gtzgkzbzej.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtaskjdztz.html

[L05] 上传文件（multipart）
来源：http://hz.yuanzhike.top/gtevzbxxwj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtmofhmpgh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtiigotzfa.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yj20258.top/gtoqqrxfzd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gteddcezwm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shuidangran.top/gtqsvizflx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yj202588.top/gtohvqeupj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangshuangyany.cn/gticcibtgu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtlmpucpra.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gtdlreavmd.html

Py:   resp.json()
来源：http://hz.cdnleiting.top/gtsagyrwag.html

PHP:  json_decode($body, true);
来源：http://hz.yj20258.top/gtpymmfdbb.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtcwnzdkdx.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtufzcftbv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtolqdqcsf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtksyhdepa.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnqzz.top/gttzlzyrll.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.daxiang520.top/gtzvvvnkys.html

[L07] 处理 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtwestdxwp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yonumen.top/gtofrmxauw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yanxiufei.cn/gtelzopaut.html

JS:   resp.ok;  resp.status
来源：http://hz.yongpay.top/gtdlsonjao.html

TS:   resp.ok;  resp.status
来源：http://hz.shzxlz.cn/gtvsrctloq.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtfoghzgoh.html

Go:   resp.StatusCode
来源：http://hz.nanxuanxn.top/gtirekzxng.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtzvspordy.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtabuajwcu.html

[L08] 并发请求多个地址
来源：http://hz.zhongyouzk.top/gtymliztqm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xziqi.cn/gtpxrbqjjx.html

PHP:  curl_multi_init() 系列
来源：http://hz.guowangkeji.top/gtyrwpfbpc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cucudq.cn/gtfqpbgbdx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtjxwsvgzc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yvedp.cn/gtbiprkfzs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtmntyvpej.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtheyqyvhi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtudciybav.html

================================================================================
来源：http://hz.jqgufenzy.top/gtcfxuykhw.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenzaomai.com/gtjyonejou.html

================================================================================
来源：http://hz.ybcxt.top/gtgqjboxnw.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtnreiyjeb.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtodjnyftx.html

PHP:  $argv;  $argc;
来源：http://hz.316326.xyz/gtmegrjxno.html

JS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtvnypvbmm.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtyquvkjkx.html

Java: args 数组（main 方法参数）
来源：http://hz.jianghu66.top/gtsrjvxuwm.html

Go:   os.Args[1:]
来源：http://hz.sxryk.cn/gtqzdkkkkh.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtiyyrfidi.html

C#:   args 数组（Main 方法参数）
来源：http://hz.shzxlz.cn/gtkodjgqpk.html

[M02] 读取环境变量
来源：http://hz.sxryk.cn/gthtpnyvpn.html

Py:   os.environ.get("HOME")
来源：http://hz.ehwqpu.com/gtybmzdgnr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtthlwzwib.html

JS:   process.env.HOME
来源：http://hz.mhx1999.top/gtzqdyxmxd.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtxluberpx.html

Java: System.getenv("HOME")
来源：http://hz.dashuyun.cn/gtbkhosqnu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhaomingkeji.xyz/gtmoxkyhip.html

Ruby: ENV["HOME"]
来源：http://hz.yonumen.top/gtntiucovo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.aibaodan.cn/gtbemhvkna.html

[M03] 执行外部命令
来源：http://hz.zhiwuduotai.top/gtvncqjhrl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.chenzaomai.com/gtdydofypw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hnxiangtu.top/gtpwnjzbsr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtzpgmtlaq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yueranfly.top/gtrkqgpqvk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtkksggiev.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.c1oappe.top/gtmqpazzfr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.guannengcc.top/gtiqtotscr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ywan-chungtsiang.top/gtsosoykjx.html

[M04] 获取当前工作目录
来源：http://hz.cashguo.top/gtqsylaoip.html

Py:   os.getcwd()
来源：http://hz.fengsongda.top/gtlhqrvlzz.html

PHP:  getcwd();
来源：http://hz.dashuyun.cn/gtxitelkvl.html

JS:   process.cwd()
来源：http://hz.pengpengdd.cyou/gtqjhaffde.html

TS:   process.cwd()
来源：http://hz.hammf.cn/gtnnryxwld.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sufxvd.cn/gtehqaqcll.html

Go:   os.Getwd()
来源：http://hz.tianlin.xyz/gtxydzaltd.html

Ruby: Dir.pwd
来源：http://hz.birdmap.top/gtginmjxnd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtvssymuxg.html

[M05] 设置退出码
来源：http://hz.hnxiangtu.top/gtpmsmprhz.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtsmbqehyt.html

PHP:  exit(1);
来源：http://hz.mhx1999.top/gtbpscedth.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtkegghrtx.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gttossfrat.html

Java: System.exit(1)
来源：http://hz.xziqi.cn/gthqgvavyw.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtownsnwaz.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtsnoadesp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gtwvxlabqh.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtbciycudo.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ydzc1.top/gtqfsgbkyk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.kuanghao11.cn/gtnbmpqppq.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gtbnxbgjzj.html

TS:   console.error("err")
来源：http://hz.xinyue.icu/gtekjjtdqo.html

Java: System.err.println("err")
来源：http://hz.ppjwa.cn/gtvjozbkdc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gttelzwqsn.html

Ruby: warn "err"
来源：http://hz.hywenlv.cn/gtodpbkxne.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtwsqygddq.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtvhhachlc.html

Py:   if __name__ == "__main__":
来源：http://hz.zhongyouzk.top/gtjikegcte.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.yj202588.top/gtatyigxsu.html

JS:   require.main === module
来源：http://hz.52xcode.cn/gtemntcnsc.html

TS:   require.main === module
来源：http://hz.daxiang520.top/gtzdqssinf.html

Java: public static void main(String[] args)
来源：http://hz.snrcjt.cn/gtpqpkzxwm.html

Go:   func main()
来源：http://hz.shanyushiyangtech.top/gtnpschmju.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.316326.xyz/gtpzlbisne.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gtckqadcdf.html

[M08] 获取系统与运行时信息
来源：http://hz.jiagoushi.top/gtezuupwli.html

Py:   platform.system();  platform.python_version()
来源：http://hz.tianlin.xyz/gtomnqaquh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.kuanghao11.cn/gtuwihzhil.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtpyjtevse.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtsyapgotm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shangyingyoupin.top/gtovvafkbr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydzc1.top/gtlacnmrug.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jinqigfzy.top/gtpnjrhsjk.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cqqwz.cn/gthoadcrze.html

================================================================================
来源：http://hz.fengsongda.top/gtmipyaqvo.html

N. 数据结构与算法
来源：http://hz.hywenlv.cn/gtqzsimmkk.html

================================================================================
来源：http://hz.yanxiufei.cn/gtsxvekalz.html

[N01] 二分查找（有序数组）
来源：http://hz.zdqjudy.top/gtfopuqfwy.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.iojbl.cn/gtcuwjctbf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gtipkypwpi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yuxming.cn/gtwjhdwulu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.kuanghao11.cn/gtyywexhqi.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhengqikj.top/gtcjwwuhyj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtquxmzdnc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sufxvd.cn/gtdbkdxghl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ydzc1.top/gttknqgttk.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shzxlz.cn/gtwjpoosjb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtxtruvizw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.daxiang520.top/gtmtjzttds.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtctxdeusz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.0kj1m.cn/gtqezylynj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.jianghu66.top/gtwookcjbe.html

Go:   slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtdksetziu.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtwhdnjnjm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtekghnzde.html

[N03] 快速排序（分治示例）
来源：http://hz.shangyingyoupin.top/gtczavsrrk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.hnxiangtu.top/gtanfwtirg.html

PHP:  // 递归实现，或用 usort
来源：http://hz.sweek.top/gtbzmmrlev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daxiang520.top/gtyvjaldtg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtnxggutsd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sweek.top/gtqiaarojs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jiagoushi.top/gtouavyxio.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtaosazusy.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.xinyue.icu/gtjkjlebmn.html

[N04] 斐波那契数列
来源：http://hz.birdmap.top/gtqowltjej.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.chenjidiqi.icu/gtkvrwjhnz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.meibo888.top/gtoapzscvp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.wangdashe.top/gtmqlpfmkc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtykqlffbu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxinkj.top/gttsbctthr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yj20258.top/gtpwslvkyp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.pengpengdd.cyou/gtlngbrggy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yonumen.top/gtcwcaiwgd.html

[N05] 最大公约数
来源：http://hz.hysaishi.cn/gtzeslmvov.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gtfvupqtfs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jqgufenzy.top/gtyfiwzhgs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gotoacloud.top/gtnfieolke.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nwbrower.top/gtvkimcpgd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gzhubu.top/gtplxhkzfl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gtonypcryo.html

Ruby: a.gcd(b)
来源：http://hz.gogol.net.cn/gtgnvhbrbf.html


<!-- 参考信息 -->