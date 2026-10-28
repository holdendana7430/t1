代发 wailian999

[J07] 比较两个日期
来源：http://hz.pycfn.com/gtnspzhlvr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gthwpgyfzk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.bjfxy.top/gtqkhdatdq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtqlnfdtlm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtjrwzcgue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtdoldehtc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtyiyvvblx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtabywvdds.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtkumponvd.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtlsngyaro.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yuxming.cn/gtpadhdymu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtzznazucu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtpkjpwlmq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtvjngpqbz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgfzy.top/gtoryiwyqz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtxgooognr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtuymlrxgo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gaohongyu789.top/gtmmkyfuvy.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtpykvgupy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtryhfdfhw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtfmomdjoy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtioocbijm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gthfptznya.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gthpuafmom.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.9152youxi.cn/gtacewetlt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtnstbiuuk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtectpxltf.html

[J10] 取今天 / 本月第一天
来源：http://hz.meibo888.top/gtsgjnrmnw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cqqwz.cn/gtikdupfxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtxovjquun.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gttlhdzrgx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtcvnoduxf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtbdqhrswr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtypwsfpgm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtelarvgvh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gaohongyu789.top/gtrptgzesn.html

================================================================================
来源：http://hz.sxryk.cn/gtpcjkzkyx.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gtsbhcxkyj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtanunihim.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtsvtrtdtu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtfkcyzjpg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtzqibvczk.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtuhsbxolz.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtsncwhalm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtogbscpnd.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gtwhrjgnko.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtvpgleavm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yonumen.top/gtwbotsciw.html

[K02] JSON 字符串转对象
来源：http://hz.xylfe.cn/gtiabepvvx.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtnlnuoumg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtszwajsxc.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gterpmbcfo.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtaegppsbk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinyuanbaomall.cn/gtioxwkdzk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtsivekgzu.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gthiodurob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtsjtkbobj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtemzvuvgd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gthhlmthtl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtzplbknkk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtxosgeqwt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtqrgsbeiv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtjmqahtcr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtxearkuuq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtfqwishlr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.0kj1m.cn/gtehkaqtxs.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtfdwbibkm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtfffsytyc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtbhkecyhw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtqfvsoxou.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtvwglxgwe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ybcxt.top/gtyoldczyi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtetzkqjul.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtaspcplog.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.meibo888.top/gtucpgjxwl.html

[K05] 深拷贝对象
来源：http://hz.jlsjyb.cn/gtpzbfbusy.html

Py:   copy.deepcopy(obj)
来源：http://hz.cheryme.top/gtbcqmdwja.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guowangkeji.top/gtvdkevwhq.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtkzxryphd.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtcssfbtdy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtktuhtfbt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtpjlwamnv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.bjfxy.top/gtqwgmdvch.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yonumen.top/gtjrqoswfz.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtgnhfvssb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gteusgqchk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtposedyez.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gthcootaua.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtneiakodj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtogzsoasc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtutrrkxcc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtbbwteijj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhiwuduotai.top/gtalgrtsbd.html

[K07] 进制转换
来源：http://hz.shuidangran.top/gteipysgxe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtjxqzzbos.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xingfuxueyuan.xyz/gtviqlwvjs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtoxaycgrn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtjkjugpfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtkbycrzvu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtujlswmpm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangdashe.top/gtwdmptilq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtmpxajwzf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxuanxn.top/gtmvmyvfoe.html

Py:   pickle.dumps(obj)
来源：http://hz.ybcxt.top/gtzqejjgvk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtoiodbhmx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtynylonrh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtevuiierb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtsmqsiqhu.html

Go:   encoding/gob
来源：http://hz.zhengqikj.top/gthffmummy.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtwtceoqhw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtpbpqotcn.html

================================================================================
来源：http://hz.birdmap.top/gtakmognyn.html

L. 网络请求
来源：http://hz.wangdashe.top/gtqccagwbc.html

================================================================================
来源：http://hz.zycfv.cn/gtfottqwdl.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gthoomsgjf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sweek.top/gtyayvtacs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.havefunace.top/gtbqmzjqtm.html

JS:   await fetch(url)
来源：http://hz.zhengqikj.top/gtdmatslpp.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtinxpvyaa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cdnleiting.top/gtobdhvaji.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtntzdshjt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydjk.org.cn/gtvdezxeuj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fengsongda.top/gtzzalngqp.html

[L02] 发送 POST JSON
来源：http://hz.sxryk.cn/gtbiccqucn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtftodphbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtpabktgro.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtjmltifkp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtmwhivpla.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hnqzz.top/gtvlmtnhnp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ppjwa.cn/gtjymezfia.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.smart0.xyz/gtkiksoylj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtwpcfjbsi.html

[L03] 设置自定义请求头
来源：http://hz.cqqwz.cn/gtlnsfmtfp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cdnleiting.top/gtighyopxe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jyoumei.cn/gtcjrkgnjj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cqqwz.cn/gtgjndjzvc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gttesfrraw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.quarkkingdee.top/gtdzyltnlt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xziqi.cn/gtjiynzvmg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtcllfsuze.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yueranfly.top/gtktihlvcg.html

[L04] 设置超时
来源：http://hz.cdnleiting.top/gtdzcyxokz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtbfjbafyr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dashuyun.cn/gtbkxfmyar.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtsomyofkp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtcisrmufh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hywenlv.cn/gttzkhwltl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtcbbtdspv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtryvaipcj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.haohaochexian.top/gtnvbiipcw.html

[L05] 上传文件（multipart）
来源：http://hz.nanxinkj.top/gtrppnkeda.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuxming.cn/gtvjpbiruk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnqzz.top/gtmlvhhqmf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daxiang520.top/gtuadokqlc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xingfuxueyuan.xyz/gtinpplgvb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.aibaodan.cn/gteippgbxf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.snrcjt.cn/gtoxcqgvll.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtiruxqhrx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.sxryk.cn/gtzknulbdn.html

[L06] 解析响应为 JSON
来源：http://hz.shzxlz.cn/gtprohevea.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtjsaupwoc.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtmqhqixaq.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtaacguehf.html

TS:   await resp.json()
来源：http://hz.tanke756.top/gtmuefjjtd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtsabolots.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtssscsgtg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtkwkhxfzh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtmcqfdvyx.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtwxsrtzmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydzc1.top/gttsvycjtk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yonumen.top/gtjtpslyed.html

JS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtljhxukpf.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtmaxoivfz.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtmgucdoja.html

Go:   resp.StatusCode
来源：http://hz.yj202588.top/gtfjkxcgws.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtzohfvrcx.html

C#:   (int)resp.StatusCode
来源：http://hz.aizwys.cn/gtyzwuuivz.html

[L08] 并发请求多个地址
来源：http://hz.sufxvd.cn/gtdnolmvwg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.birdmap.top/gtgwcczixa.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtjiubpouu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guowangkeji.top/gtmfpcmkhq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jqgufenzy.top/gtndgsswix.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtelzykqre.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtyvmtxuft.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydjk.org.cn/gtiwdxyjaf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yueranfly.top/gtcufenlbp.html

================================================================================
来源：http://hz.yangfankeji.com/gtnzecbwkg.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtqjzllrmm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbppouwjg.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtmaieevag.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gttoipytmi.html

PHP:  $argv;  $argc;
来源：http://hz.jianghu66.top/gtckrjjdti.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtizoqpnzb.html

TS:   process.argv.slice(2)
来源：http://hz.cucudq.cn/gthseeodnb.html

Java: args 数组（main 方法参数）
来源：http://hz.yanxiufei.cn/gtfnjmrmlm.html

Go:   os.Args[1:]
来源：http://hz.sxryk.cn/gtyqmpmyhc.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtwhpkjrur.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zdqjudy.top/gtasvhfyjg.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtfpqpxqlv.html

Py:   os.environ.get("HOME")
来源：http://hz.yueranfly.top/gtphjluiwd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.wangshuangyany.cn/gtcujhvlkg.html

JS:   process.env.HOME
来源：http://hz.svipenyu.cn/gtvnvzdwgu.html

TS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtnewdmozh.html

Java: System.getenv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtttozidfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxinkj.top/gtxwcdgusf.html

Ruby: ENV["HOME"]
来源：http://hz.jyoumei.cn/gtirzqnmtd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cashguo.top/gtzpfnxwwz.html

[M03] 执行外部命令
来源：http://hz.daria6918.cn/gtgdgvfuqx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtbihsoeuh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gotoacloud.top/gtjbgzllgr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.haohaochexian.top/gtmiwtlqrb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.cdnleiting.top/gtnucehwlh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xylfe.cn/gtvbpkmmea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtcgopvezm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.cqqwz.cn/gtwucoihgv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.hysaishi.cn/gtthlhogbd.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtdyiswvca.html

Py:   os.getcwd()
来源：http://hz.gaohongyu789.top/gtjkdqsgbm.html

PHP:  getcwd();
来源：http://hz.ybcxt.top/gtcvqjkift.html

JS:   process.cwd()
来源：http://hz.ywan-chungtsiang.top/gtnxltnyop.html

TS:   process.cwd()
来源：http://hz.birdmap.top/gtemnutxtr.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.cheryme.top/gtwyhdmxps.html

Go:   os.Getwd()
来源：http://hz.fengsongda.top/gtpzqwxwcb.html

Ruby: Dir.pwd
来源：http://hz.nanxuanxn.top/gtqpbfkuzz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.quarkkingdee.top/gtkoptgfgd.html

[M05] 设置退出码
来源：http://hz.fengsongda.top/gtrwimajhm.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtvsuuactc.html

PHP:  exit(1);
来源：http://hz.kuanghao11.cn/gtjigjruln.html

JS:   process.exit(1)
来源：http://hz.zhaomingkeji.xyz/gtsfjevscr.html

TS:   process.exit(1)
来源：http://hz.yonumen.top/gtonslimke.html

Java: System.exit(1)
来源：http://hz.0kj1m.cn/gtxlejhqvb.html

Go:   os.Exit(1)
来源：http://hz.xuetiantiany.cn/gtlamkcytn.html

Ruby: exit 1
来源：http://hz.zhixingplan.top/gtzqphzxwx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.pengpengdd.cyou/gtfoztqand.html

[M06] 向标准错误输出
来源：http://hz.sysykeji.top/gtrnghtffx.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sxryk.cn/gtqmgummgh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.svipenyu.cn/gtygzqghkd.html

JS:   console.error("err")
来源：http://hz.9152youxi.cn/gtgopxhfew.html

TS:   console.error("err")
来源：http://hz.xingfuxueyuan.xyz/gtpxjwdbtj.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtjldvqppk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.ehwqpu.com/gttkcvcbll.html

Ruby: warn "err"
来源：http://hz.gotoacloud.top/gtfbfwrjlv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.snrcjt.cn/gtesyndoqd.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtrbzxftlu.html

Py:   if __name__ == "__main__":
来源：http://hz.mhx1999.top/gtvhadkljj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.aibaodan.cn/gthqwjfnqr.html

JS:   require.main === module
来源：http://hz.svipenyu.cn/gtolnvdbqg.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtcysxdawv.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtwntbmyla.html

Go:   func main()
来源：http://hz.ydjk.org.cn/gtepvdaead.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinyuanbaomall.cn/gtwdebrpxb.html

C#:   static void Main(string[] args)
来源：http://hz.dashuyun.cn/gtcnntnxyg.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtfkiauplr.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtldnizrtc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.smart0.xyz/gtojypsstc.html

JS:   process.platform;  process.version
来源：http://hz.jlsjyb.cn/gtixkpgwzs.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtpfwkyiza.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.cqqwz.cn/gtntivtypj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.fzhhl.top/gtlfrzpxbj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hywenlv.cn/gtcjyjtojp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tanke756.top/gtaxobgjay.html

================================================================================
来源：http://hz.quarkkingdee.top/gtmumafgrb.html

N. 数据结构与算法
来源：http://hz.hnqzz.top/gtsvuyfdwq.html

================================================================================
来源：http://hz.meibo888.top/gterfquoln.html

[N01] 二分查找（有序数组）
来源：http://hz.andypj.xyz/gtplqjlkjx.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.yj202588.top/gtaddpwdiv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.haohaochexian.top/gtdbsdmcat.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtuwlykqvd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.guowangkeji.top/gtvcpmtzpw.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yangfankeji.com/gthhyaniuf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yj20258888.top/gtxiuovcpr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.tianlin.xyz/gtfsulcccs.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.52xcode.cn/gtwfjhfkax.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.snrcjt.cn/gtfvoovlle.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtfeddkygp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jiagoushi.top/gthpephipy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.xylfe.cn/gtrjfcdcsk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shangyingyoupin.top/gtuyyuoayk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hywenlv.cn/gtqpwpoqex.html

Go:   slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtmydwwugd.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gthqjvfnus.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ydjk.org.cn/gtrujuegxo.html

[N03] 快速排序（分治示例）
来源：http://hz.dashuyun.cn/gtrqwgyjkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhixingplan.top/gtgfzfrobu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.gogol.net.cn/gtxtlkaoye.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtdhvzqdde.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydjk.org.cn/gttwzjywfy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.sxryk.cn/gtdxwvzyei.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.guowangkeji.top/gtajwcyanv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ehwqpu.com/gtemdvxddv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zycfv.cn/gteoopmlxw.html

[N04] 斐波那契数列
来源：http://hz.chenzaomai.com/gtxsyixncw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ywan-chungtsiang.top/gtpmtbnrla.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xinyue.icu/gttelprbks.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenzaomai.com/gtveftyrii.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hnqzz.top/gtxbisahwa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xuetiantiany.cn/gtkwgwqfep.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.bjfxy.top/gthojlaunv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.ybcxt.top/gtpvayeyio.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.gzhubu.top/gtjffajftn.html


<!-- 参考信息 -->