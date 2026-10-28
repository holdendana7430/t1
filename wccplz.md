代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.iojbl.cn/gtdyukjsrs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtcofrrple.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gtbkqpbxwp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhiwuduotai.top/gtqoilqhxz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hammf.cn/gtzdgkqdfn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cqqwz.cn/gtjdltxyst.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtmzmphgpg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtjkwpaiva.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ywan-chungtsiang.top/gtmnsnuggz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtusinducj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtnzlubzgj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnxiangtu.top/gtqsyzqmhk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shzxlz.cn/gtipkqbnya.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtpektnkiu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtpcqiydcr.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gtzdeqgshn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xuanzx.com/gtphuowzow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gtsqwqkvjg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtvmpvlxpj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ehwqpu.com/gtwedbyaxc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtdljffhyc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtvhtotngo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gtftzdfnjj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gtucuzdaih.html

================================================================================
来源：http://hz.yuanzhike.top/gtfaituuka.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtbuauocra.html

================================================================================
来源：http://hz.mhx1999.top/gteuqhnhxe.html

[K01] 对象转 JSON 字符串
来源：http://hz.jiagoushi.top/gtdozzswsa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtvplkhodc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gthqmzlims.html

JS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gttsjmbzed.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtbfczvjkn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gttzqztpdp.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gttfpvnpyz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinyuanbaomall.cn/gthccjfdvy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtsegbgrok.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtnedrdzcf.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gtujdugzfd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtouygrxqd.html

JS:   JSON.parse(s)
来源：http://hz.yj202588.top/gttczyifmq.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gteppgyhpd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtexagftzx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtnoaqznmu.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtavtfdhev.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtnpklyblx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtgndvbhfg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtdvabcefg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtafypdpfe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtevszjuhj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtnzpusfud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pycfn.com/gtqtyhgszh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhaomingkeji.xyz/gtxlmpynkk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtfjjyjlvu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yanxiufei.cn/gtwqciuvwz.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtzusmyzpo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtofdqabmd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.aibaodan.cn/gtebymtxtg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtpprdmybl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtjmxfquvm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtggscphou.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtlnfadtqv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jyoumei.cn/gtkfqsksxo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hammf.cn/gtfwpomame.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtafdssikn.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtznlmshjb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xylfe.cn/gtdsgexwfi.html

JS:   structuredClone(obj)
来源：http://hz.shuidangran.top/gtqdukugzl.html

TS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtuinbcprb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtnyoemtil.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtuasittqm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gaohongyu789.top/gtivshrtsq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtxsmibjum.html

[K06] 解析 URL 查询串
来源：http://hz.0kj1m.cn/gtkgqmbxag.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtldcyxdts.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gthnrnpyuo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtjzpgcikd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtpfeyntbh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aizwys.cn/gtwguwmhjv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtpgopyhtn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtgydilylf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenlongwang.top/gthfdruaic.html

[K07] 进制转换
来源：http://hz.jlsjyb.cn/gtdrzanudy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtlbesemar.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhijiandao.cn/gtzjtmdgzm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtsiaruqkc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtzmelrajl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtvcwcvbre.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhixingplan.top/gtrrwpgpkp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gthspesnpd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtemnxgamz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gteivhkeqe.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtarpgafjt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gtiqmvpiby.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cucudq.cn/gtwpkvdjjf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtnwfbgbmp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinghuilouyu.cn/gtzjuqewpk.html

Go:   encoding/gob
来源：http://hz.ywan-chungtsiang.top/gthlngkvqx.html

Ruby: Marshal.dump(obj)
来源：http://hz.redwolf501.top/gtpejeosrc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtwgbwsqnd.html

================================================================================
来源：http://hz.jyoumei.cn/gtqmyhmede.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtjbfumxmh.html

================================================================================
来源：http://hz.jqgfzy.top/gtkizdpkqf.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gteoofhdcl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtjknpxvvb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj202588.top/gtvwxbdzuc.html

JS:   await fetch(url)
来源：http://hz.yonumen.top/gtvvrarzrp.html

TS:   await fetch(url)
来源：http://hz.316326.xyz/gtuvqalqrt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtewtqjaad.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtjnwayzkc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.aizwys.cn/gtpzcysien.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigfzy.top/gtuukkszkm.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtaxsqjkqf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jyoumei.cn/gtadyciogo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtxpvidgci.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhoulong.xyz/gtzxvligoc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtalgzrwru.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gotoacloud.top/gtoouxxwkp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.vqdsnc.cn/gtkrpgvclb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guowangkeji.top/gtdmvwqyza.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj20258.top/gtvnguwqpv.html

[L03] 设置自定义请求头
来源：http://hz.zhongyouzk.top/gthsogrpqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtpwnntyoc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinyuanbaomall.cn/gtztdbfuyc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.smart0.xyz/gtgbtdxhrp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtckpovqwo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtlnqqwuol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtiaymouva.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gthkosuguz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.cdnleiting.top/gtjnnjwrld.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtrspsmiqt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gotoacloud.top/gtpwlcmfkt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gtqoegrsgo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gtgzqjzlml.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258888.top/gtniawzagd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtyvfnvlol.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yvedp.cn/gtslqvppfj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtxumfnxaq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtmpktfcos.html

[L05] 上传文件（multipart）
来源：http://hz.shzxlz.cn/gtyqdpuwki.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.birdmap.top/gtbkcjjwax.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtzircpxlx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtazlfzovy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jinyuanbaomall.cn/gtgkdhkqqk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtzodpyypx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtpgvzjgrt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cashguo.top/gtnzakivdo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.0kj1m.cn/gttkrzzler.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtquifkkiv.html

Py:   resp.json()
来源：http://hz.snrcjt.cn/gtkjzeiykk.html

PHP:  json_decode($body, true);
来源：http://hz.yangfankeji.com/gthikmvrau.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtotvcvjha.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtydvlthjq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtxofsssqj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtulqfiqbm.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhijiandao.cn/gttrpyvuyj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtvbkgbtmv.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gtvaultdmp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.fengsongda.top/gtwbrzohix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhijiandao.cn/gtqzpmtbzu.html

JS:   resp.ok;  resp.status
来源：http://hz.gaohongyu789.top/gtlcefpopv.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtvremflfu.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gteklodffx.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtttvdalfo.html

Ruby: resp.code.to_i
来源：http://hz.hysaishi.cn/gtvegkjehd.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtzdauopkp.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtddnqeilu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shangyingyoupin.top/gtlpcrcaph.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangshuangyany.cn/gtfweecqwu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cheryme.top/gtcaqwebht.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtjlieqxlp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jianghu66.top/gtlxulitvf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtjunvuvnd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtkdbhhubn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.ywan-chungtsiang.top/gtovrqyrdp.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtjcwdupli.html

M. 命令行 / 进程 / 环境
来源：http://hz.aibaodan.cn/gtpgxwbrny.html

================================================================================
来源：http://hz.ydjk.org.cn/gtynncrjnq.html

[M01] 读取命令行参数
来源：http://hz.hysaishi.cn/gtqdbyeuib.html

Py:   sys.argv[1:]
来源：http://hz.sysykeji.top/gtkkzggzbs.html

PHP:  $argv;  $argc;
来源：http://hz.guannengcc.top/gtscdkzsav.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtaygpubdz.html

TS:   process.argv.slice(2)
来源：http://hz.zhaomingkeji.xyz/gtqmbtihng.html

Java: args 数组（main 方法参数）
来源：http://hz.ehwqpu.com/gtofxwtyvx.html

Go:   os.Args[1:]
来源：http://hz.kuanghao11.cn/gtmqigaiyx.html

Ruby: ARGV
来源：http://hz.xingfuxueyuan.xyz/gtbbrzvzoj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gotoacloud.top/gtvgcvqmit.html

[M02] 读取环境变量
来源：http://hz.zycfv.cn/gtmehdtejv.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtshdoclts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.xinyue.icu/gtubmmebcf.html

JS:   process.env.HOME
来源：http://hz.0kj1m.cn/gtkxoknbiv.html

TS:   process.env.HOME
来源：http://hz.zhijiandao.cn/gtfjiowwpv.html

Java: System.getenv("HOME")
来源：http://hz.zhengqikj.top/gtvahdlttb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhoulong.xyz/gtvyddhpbr.html

Ruby: ENV["HOME"]
来源：http://hz.jinyuanbaomall.cn/gtscgjwujp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ivvv.top/gtxjeflpmn.html

[M03] 执行外部命令
来源：http://hz.feifeiyinyue.top/gtsynycdsv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pengpengdd.cyou/gtvfgljfbp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.aizwys.cn/gtwtmqugxs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtlummsacp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.aibaodan.cn/gtkihmjrer.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.sysykeji.top/gtogydpgva.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.andypj.xyz/gtdqdlolrf.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.tanke756.top/gtecmuylpj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtvbzlgesu.html

[M04] 获取当前工作目录
来源：http://hz.hnqzz.top/gtqktugfho.html

Py:   os.getcwd()
来源：http://hz.snrcjt.cn/gtyrzvuzsx.html

PHP:  getcwd();
来源：http://hz.chenzaomai.com/gtqvgjzjxi.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtrebrutwz.html

TS:   process.cwd()
来源：http://hz.sxryk.cn/gtakvmzlii.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ywan-chungtsiang.top/gtzbvmjnyw.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtqbkcmcdb.html

Ruby: Dir.pwd
来源：http://hz.yangfankeji.com/gtyncefqss.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zycfv.cn/gtnuuxcemn.html

[M05] 设置退出码
来源：http://hz.zhengqikj.top/gtnvkykvfi.html

Py:   sys.exit(1)
来源：http://hz.zhoulong.xyz/gtkqgkbbdi.html

PHP:  exit(1);
来源：http://hz.ydjk.org.cn/gtytnrxxvs.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtczuxvrty.html

TS:   process.exit(1)
来源：http://hz.meibo888.top/gtvizwygfk.html

Java: System.exit(1)
来源：http://hz.xuetiantiany.cn/gtajlrixfa.html

Go:   os.Exit(1)
来源：http://hz.dianchejie.cn/gtylbfknra.html

Ruby: exit 1
来源：http://hz.gzhubu.top/gthqupckqf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xuetiantiany.cn/gtfaxvuydw.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtizvqxmau.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gteqldmovl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.zhiwuduotai.top/gtgtfawpvl.html

JS:   console.error("err")
来源：http://hz.jinghuilouyu.cn/gttqydvwff.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gtjwczsolz.html

Java: System.err.println("err")
来源：http://hz.meibo888.top/gtolykgrdc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ppjwa.cn/gtlnybizfn.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtewticywl.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.svipenyu.cn/gtcswvjxze.html

[M07] 判断是否为主入口
来源：http://hz.hnqzz.top/gtjkybsleb.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gthjirjpvl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtdlwqdmek.html

JS:   require.main === module
来源：http://hz.xziqi.cn/gtlbfztsyv.html

TS:   require.main === module
来源：http://hz.hnqzz.top/gtzagsqaxx.html

Java: public static void main(String[] args)
来源：http://hz.sufxvd.cn/gtbcwhbuqu.html

Go:   func main()
来源：http://hz.jqgfzy.top/gtmmnnflzh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhengqikj.top/gtsziccqut.html

C#:   static void Main(string[] args)
来源：http://hz.ivvv.top/gtibgjwqgq.html

[M08] 获取系统与运行时信息
来源：http://hz.chenlongwang.top/gtpdqvesqs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.meibo888.top/gtfaznmgim.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gttqtkuqfv.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtakokfdwy.html

TS:   process.platform;  process.version
来源：http://hz.nanxuanxn.top/gtayxcmukg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.quarkkingdee.top/gtjztjwyqy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.316326.xyz/gtzxyxtubg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.shuidangran.top/gtgisexsxp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.ehwqpu.com/gtnzlmyfaj.html

================================================================================
来源：http://hz.meibo888.top/gtfxbuwhrv.html

N. 数据结构与算法
来源：http://hz.havefunace.top/gtiumduvxw.html

================================================================================
来源：http://hz.svipenyu.cn/gtuxtvzonx.html

[N01] 二分查找（有序数组）
来源：http://hz.yvedp.cn/gtwfuxrapl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yvedp.cn/gtlhkmjzpw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jqgufenzy.top/gthepgnlgf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtyzajvhjd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yonumen.top/gtpshrobak.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.guowangkeji.top/gteexyuqgv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhoulong.xyz/gtdfwrubzt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigfzy.top/gtlhejsopn.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.chenzaomai.com/gtqyaidbpf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtgxxdwjou.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gthxsueoem.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yonumen.top/gtjoskiubf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.52xcode.cn/gtkggulonp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.vqdsnc.cn/gtjmwnpkqw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.aizwys.cn/gtuklrtobk.html

Go:   slices.Sort(arr)
来源：http://hz.aizwys.cn/gtubfusjlh.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtqughlrci.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.nanxuanxn.top/gtgioytrmt.html

[N03] 快速排序（分治示例）
来源：http://hz.tanke756.top/gtbwybwtfs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.mhx1999.top/gtuoppgxdv.html

PHP:  // 递归实现，或用 usort
来源：http://hz.dianchejie.cn/gtxvohfagd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhoulong.xyz/gtkqmnxrtp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.vqdsnc.cn/gtknqeiqbf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.wangshuangyany.cn/gtwliquers.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.meibo888.top/gtkkyhsyar.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.nanxinkj.top/gtbgtrbyqr.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.daria6918.cn/gtsvqbxvqu.html

[N04] 斐波那契数列
来源：http://hz.ivvv.top/gtriopybvc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.mhx1999.top/gtxqeyayjw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.andypj.xyz/gthjckaogu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.iojbl.cn/gtsdmhlnxn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cdnleiting.top/gtiklkpsxk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtffanshxo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jiagoushi.top/gtwhohanau.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.52xcode.cn/gtewsriiqs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtbyzajixc.html

[N05] 最大公约数
来源：http://hz.daxiang520.top/gtwddkxigq.html

Py:   math.gcd(a, b)
来源：http://hz.yj202588.top/gtecfdqblo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.havefunace.top/gtjvderzbi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yj202588.top/gtqjsdrtsq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtzyouvlzl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ybcxt.top/gtkepttzhh.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.iojbl.cn/gtyehpgtqz.html

Ruby: a.gcd(b)
来源：http://hz.shanyushiyangtech.top/gtrwdxdumd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jiagoushi.top/gtinrqqfqu.html

[N06] 判断回文字符串
来源：http://hz.pycfn.com/gtvtbvnuwl.html

Py:   s == s[::-1]
来源：http://hz.daria6918.cn/gtlquzdzvf.html

PHP:  $s === strrev($s);
来源：http://hz.tanke756.top/gtewkefnrq.html


<!-- 参考信息 -->