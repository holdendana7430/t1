代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtnijvqrxv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnxiangtu.top/gtqytiiqnm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtwzwygyid.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtueckltgh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtjtwedagx.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtgbksyqaj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtcjxmjrld.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigufen.top/gtnbonnhka.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtgsdjaaik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gtgrcmyebu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtxllfkrcv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dashuyun.cn/gtqnqppptd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtmpemsesy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuetiantiany.cn/gtxesanttm.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gteanpvxbm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtukqbzqyf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtljsnykwk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yongpay.top/gtwxnwudrj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gtglmpbgto.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtslzrdiqa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangshuangyany.cn/gtsbqyynnf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtzsjtrwdh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtrynrueeh.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangdashe.top/gtywmjrqwy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtmaxjbtyh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gtovymutwo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtiozxhwoo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gttebbkrty.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtbxnknfzx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtbanyczop.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhaomingkeji.xyz/gtwvnydifh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtvmcsnutt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtgcwdbdfd.html

K. JSON 与序列化
来源：http://hz.cqqwz.cn/gtfkmnyncj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtubebvelo.html

[K01] 对象转 JSON 字符串
来源：http://hz.pycfn.com/gteqfzgjua.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gtttcqbytp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtuinuthbn.html

JS:   JSON.stringify(obj)
来源：http://hz.9152youxi.cn/gttoruqbzs.html

TS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtldlytgst.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtzhwyupos.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtpkrlhekl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtqbubisha.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cdnleiting.top/gtbfiqczfv.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtyevcuccv.html

Py:   json.loads(s)
来源：http://hz.pycfn.com/gtxibqxqsh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtrwvnitoc.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtvokrtzqo.html

TS:   JSON.parse(s)
来源：http://hz.sufxvd.cn/gtwzpcvzws.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jiagoushi.top/gtsecpcicw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtmmykdjmu.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gttsdiwwvw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nanxuanxn.top/gtdhdxpats.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtnffwqmis.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtjugdjwdl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtevhtopvr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtejzxfzno.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtaijtbhud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xinyue.icu/gtmlbjuiyg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtvvevadtv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.redwolf501.top/gtqcufpdfu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xinyue.icu/gtigbgavao.html

[K04] 读取 JSON 文件
来源：http://hz.redwolf501.top/gtykkljujg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gteqbehvqm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtowfyjhoa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtyzyaeexf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtzsnetlhb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.mhx1999.top/gtvmminugx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtqhyybhdh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtfqpbedvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtwqddppqu.html

[K05] 深拷贝对象
来源：http://hz.0kj1m.cn/gtkjmrjdbf.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtsinswlaf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gthkdxtddr.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtlpklkevv.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtcvnbwefa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.0kj1m.cn/gtylnclwyi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtdeioottc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtbnovwhtm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtnvmcxmnz.html

[K06] 解析 URL 查询串
来源：http://hz.sweek.top/gtzgsaijmi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gaohongyu789.top/gtvrdddbzf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtpjwwnffr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtbsudpkof.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtjzvvmnzc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.aibaodan.cn/gtnnhiewsl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yongpay.top/gtacbagwog.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhengqikj.top/gtdmalpfai.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtyyuhmlpi.html

[K07] 进制转换
来源：http://hz.jinqigfzy.top/gtrybswvbs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtckpmxqej.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtbvedygul.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtmumfadex.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.birdmap.top/gtqowpatvm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtwbstottk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtyjgxcscs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.9152youxi.cn/gtjzdcmwlh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yvedp.cn/gtjjdjbssr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhengqikj.top/gtdtumoshb.html

Py:   pickle.dumps(obj)
来源：http://hz.quarkkingdee.top/gtnzqjrkko.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gteseycxux.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtbndiyhwt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gtpchoslaa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shanyushiyangtech.top/gtfzwgsvxs.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtfjkqmjoc.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj20258.top/gtylitibhd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtjrghknal.html

================================================================================
来源：http://hz.ehwqpu.com/gtkcgbqcto.html

L. 网络请求
来源：http://hz.jinyuanbaomall.cn/gtrtdonpol.html

================================================================================
来源：http://hz.guannengcc.top/gtghgrzxdl.html

[L01] 发送 GET 请求
来源：http://hz.zycfv.cn/gtcslwihkj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtesxqilgv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.aizwys.cn/gtftaszmxw.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gttonpmgdr.html

TS:   await fetch(url)
来源：http://hz.pycfn.com/gtcptumemj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtbxvrkoob.html

Go:   resp, err := http.Get(url)
来源：http://hz.pengpengdd.cyou/gtcaurkzuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtwhvwzvio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinghuilouyu.cn/gthconpjty.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtrakppcsw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cashguo.top/gtbxtubfaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gthegsjdhl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtmhwnkdba.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtwcyjwock.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.fengsongda.top/gtmkvalkxb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtglfbfisn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtkuhzeclu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.haohaochexian.top/gtqlsikgtj.html

[L03] 设置自定义请求头
来源：http://hz.zycfv.cn/gtjwonlbqw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jqgufenzy.top/gtwkgoapbi.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hfpthk.cn/gtjfmjghck.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtdlydlmgv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gthtalnwld.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtbsivunzw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtknesmufh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.iojbl.cn/gtxmmgbprv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnqzz.top/gtgnrvvbgg.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gtrxqgcgou.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gtgxdiovis.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtcgqwxwkr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gthyvoqfix.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtqbblbheu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.52xcode.cn/gtkcxttcyw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtltkjydjf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hnxiangtu.top/gtjyoudanu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.birdmap.top/gtbzpvzxcy.html

[L05] 上传文件（multipart）
来源：http://hz.xuanzx.com/gthldlyuel.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.bjfxy.top/gtjqcuxgmh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.haohaochexian.top/gtutmrtjwn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtaapvlarr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gthskllelz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shangyingyoupin.top/gtdxzbfnxs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nwbrower.top/gtvsdpyuwo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtykfpztac.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daria6918.cn/gtwinlgdfe.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtupkgerxc.html

Py:   resp.json()
来源：http://hz.cashguo.top/gticwvyvhc.html

PHP:  json_decode($body, true);
来源：http://hz.snrcjt.cn/gtbhlpjdib.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtwqqqfdcz.html

TS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtzjuoxfvi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.daria6918.cn/gtsfwhhrfx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yonumen.top/gtztrrevbj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zdqjudy.top/gtwsvnchoj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xuanzx.com/gtcyjqduun.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhixingplan.top/gtvmjyskcq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yj20258888.top/gtcfvixkui.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yvedp.cn/gtuyobatlq.html

JS:   resp.ok;  resp.status
来源：http://hz.pycfn.com/gtplkemnls.html

TS:   resp.ok;  resp.status
来源：http://hz.xinyue.icu/gteaelibor.html

Java: resp.statusCode()
来源：http://hz.svipenyu.cn/gthpeatauq.html

Go:   resp.StatusCode
来源：http://hz.sweek.top/gtlwdzgjsz.html

Ruby: resp.code.to_i
来源：http://hz.xuanzx.com/gtvoxgmwak.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtkereborq.html

[L08] 并发请求多个地址
来源：http://hz.sufxvd.cn/gtdlxdwwtq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.guannengcc.top/gtycpuamof.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtalbjpckd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtybtwetfo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydjk.org.cn/gtxrxtghrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.sweek.top/gtrdihqlzp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yanxiufei.cn/gtxecogkyc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuetiantiany.cn/gtcehleymu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigufen.top/gtwrffjlop.html

================================================================================
来源：http://hz.mhx1999.top/gtlptlfpej.html

M. 命令行 / 进程 / 环境
来源：http://hz.nanxinkj.top/gtrmhrlrle.html

================================================================================
来源：http://hz.aibaodan.cn/gtxqmjxwsw.html

[M01] 读取命令行参数
来源：http://hz.sxryk.cn/gtlmhemqsx.html

Py:   sys.argv[1:]
来源：http://hz.havefunace.top/gtjipmrekz.html

PHP:  $argv;  $argc;
来源：http://hz.cqqwz.cn/gthztigolo.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtyotxnwto.html

TS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtjzladngu.html

Java: args 数组（main 方法参数）
来源：http://hz.chenjidiqi.icu/gtqkgsiydu.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gttrrisvul.html

Ruby: ARGV
来源：http://hz.hongshengwenyu.top/gtjuzgiilc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.yj20258888.top/gtnofynwpf.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtfhclgdaq.html

Py:   os.environ.get("HOME")
来源：http://hz.zhijiandao.cn/gtxhzdibmx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtblukskom.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtsjujclxa.html

TS:   process.env.HOME
来源：http://hz.zhixingplan.top/gtfxozeccl.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtaqajksvy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtesvoysan.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtnnzmlcwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtbwqmaeuu.html

[M03] 执行外部命令
来源：http://hz.wangshuangyany.cn/gtybwydmko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtnbwrjkdq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.daxiang520.top/gtiaoibqtj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xingfuxueyuan.xyz/gtbkednfjk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtryzjicgp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuxming.cn/gtuyfrbeud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtgjsyjyll.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.svipenyu.cn/gtmxegvjoj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yueranfly.top/gtjobpdyae.html

[M04] 获取当前工作目录
来源：http://hz.zhengqikj.top/gtjwbfcqsh.html

Py:   os.getcwd()
来源：http://hz.jqgufenzy.top/gthuczztuf.html

PHP:  getcwd();
来源：http://hz.chenlongwang.top/gtftymjfgz.html

JS:   process.cwd()
来源：http://hz.ybcxt.top/gtgqjubpkd.html

TS:   process.cwd()
来源：http://hz.chenzaomai.com/gttvzcoecl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhongyouzk.top/gtrcyfmhln.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtlpkycdve.html

Ruby: Dir.pwd
来源：http://hz.yj20258888.top/gtqujcvjdv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gtdzblitzk.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gthiyeixwq.html

Py:   sys.exit(1)
来源：http://hz.xingfuxueyuan.xyz/gtyfnozuop.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gtdaxhglia.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gtmbpwntbc.html

TS:   process.exit(1)
来源：http://hz.vqdsnc.cn/gtgrkjhhui.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtfjqdfdvu.html

Go:   os.Exit(1)
来源：http://hz.jinyuanbaomall.cn/gtlnqpgwka.html

Ruby: exit 1
来源：http://hz.yonumen.top/gtwcmvtsan.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zhoulong.xyz/gtgtxasfuc.html

[M06] 向标准错误输出
来源：http://hz.sxryk.cn/gtscoexwck.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cqqwz.cn/gtkbltbude.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.bjfxy.top/gtmpqijdgc.html

JS:   console.error("err")
来源：http://hz.jqgufenzy.top/gtefqsvqoi.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtkzdqjvps.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtcevklvtl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj202588.top/gtajkfvcyo.html

Ruby: warn "err"
来源：http://hz.hfpthk.cn/gtnzpzwoud.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yangfankeji.com/gtlprbcdmi.html

[M07] 判断是否为主入口
来源：http://hz.jinqigfzy.top/gtsffzyoad.html

Py:   if __name__ == "__main__":
来源：http://hz.cashguo.top/gtxvojrqcw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.andypj.xyz/gtgzweyjbu.html

JS:   require.main === module
来源：http://hz.mhx1999.top/gtacmklxjo.html

TS:   require.main === module
来源：http://hz.chenzaomai.com/gtomyukcur.html

Java: public static void main(String[] args)
来源：http://hz.52xcode.cn/gtnxagxhzd.html

Go:   func main()
来源：http://hz.jqgufenzy.top/gtpotdgnfp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuetiantiany.cn/gtfqilsmwj.html

C#:   static void Main(string[] args)
来源：http://hz.shanyushiyangkeji.top/gtrrixazko.html

[M08] 获取系统与运行时信息
来源：http://hz.xuanzx.com/gthsnxdafj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtgfppxrso.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yuxming.cn/gtpsgqfqva.html

JS:   process.platform;  process.version
来源：http://hz.cdnleiting.top/gtdepsxkzu.html

TS:   process.platform;  process.version
来源：http://hz.cucudq.cn/gtmokupyze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtemqjdjqd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.sxryk.cn/gtpgxhuvjq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnqzz.top/gttpfilixa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.nwbrower.top/gtuiwqcbrg.html

================================================================================
来源：http://hz.xinyue.icu/gtoluhefto.html

N. 数据结构与算法
来源：http://hz.nanxinkj.top/gtwhnjcoib.html

================================================================================
来源：http://hz.yj202588.top/gtuzhzndoc.html

[N01] 二分查找（有序数组）
来源：http://hz.gzhubu.top/gtdldymeje.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zdqjudy.top/gtiisonhxr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jyoumei.cn/gtyvhaqwuf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yangfankeji.com/gtluyoofpw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhijiandao.cn/gtjvljuyaj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jlsjyb.cn/gtrxuxteid.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cdnleiting.top/gtsqazavwy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhongyouzk.top/gtscqzijrx.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jinqigfzy.top/gthacikhqf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jlsjyb.cn/gtkxeebjml.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtyxhgjsnk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuetiantiany.cn/gtnpioqbbq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sufxvd.cn/gtmmjzgmvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yj20258.top/gtkaidjuzi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtsaxdgnbm.html

Go:   slices.Sort(arr)
来源：http://hz.wangshuangyany.cn/gtybthtcby.html

Ruby: arr.sort
来源：http://hz.vqdsnc.cn/gtyxtrwiux.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuanzx.com/gtwphvghbu.html

[N03] 快速排序（分治示例）
来源：http://hz.guowangkeji.top/gtbstxwdla.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.havefunace.top/gtkwopmbai.html

PHP:  // 递归实现，或用 usort
来源：http://hz.bjfxy.top/gtkgmcymqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtmywxcxjq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.xuetiantiany.cn/gtdvktgujc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.zhixingplan.top/gtyrnbjgkx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jlsjyb.cn/gtlgcuutmc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sweek.top/gtirgxkofw.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shanyushiyangkeji.top/gtxmfzaarp.html

[N04] 斐波那契数列
来源：http://hz.shzxlz.cn/gtyokvgayf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.zhiwuduotai.top/gtznlgtaph.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tanke756.top/gtoxfuduaz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.chenjidiqi.icu/gtuwwedwyn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ehwqpu.com/gtudmsmwjj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zdqjudy.top/gturlrpxfb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.pengpengdd.cyou/gtdngdfrjr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangdashe.top/gtaqnmbzub.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zhoulong.xyz/gtqcfoafdk.html

[N05] 最大公约数
来源：http://hz.wangshuangyany.cn/gtohozezpv.html

Py:   math.gcd(a, b)
来源：http://hz.tanke756.top/gtmmclgfss.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.xuetiantiany.cn/gtzlvaveag.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenlongwang.top/gtyxrdknes.html


<!-- 参考信息 -->