代发 wailian999

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtifbepyzy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtvpvoeqci.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuanzhike.top/gtwxahnsxv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gttycpjtad.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxinkj.top/gtabpsiqvu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtdnmckugg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtsaxbvywv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtvkjayala.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtwgyyjtmv.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtsurayocl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gaohongyu789.top/gtrokrtmfx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtbnjvrvql.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yangfankeji.com/gtgdytdgef.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtgneximbe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shzxlz.cn/gtvyxhrpjf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtjipmaoog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtrlvtnqjz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtzstvrdal.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtplbuyjcp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtdrswzpgr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtztolngri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gtyyokrzgp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gthctjqdkk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cucudq.cn/gtlwwjndlx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtvdjgyqqd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gthoxxpgjp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtmrwbjtad.html

[J10] 取今天 / 本月第一天
来源：http://hz.ehwqpu.com/gtktyofmmm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gtajlwfhlo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigfzy.top/gtpuohyins.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtczknsydr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtzwmlhnfk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtaylakbvz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gttdfebkvi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtjigfizxu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtnlqtqvsj.html

================================================================================
来源：http://hz.chenlongwang.top/gtmzmqookt.html

K. JSON 与序列化
来源：http://hz.meibo888.top/gtdzwhcbmj.html

================================================================================
来源：http://hz.yongpay.top/gtccfsdrhd.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gtrcdbnzuk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtdlfjahtm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtqtxtglku.html

JS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtpbajkwho.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtibuaawns.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gtvxzqkeim.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtseheyiap.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtsquubtqo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtgeoyzhps.html

[K02] JSON 字符串转对象
来源：http://hz.wangshuangyany.cn/gtfooxrbuv.html

Py:   json.loads(s)
来源：http://hz.jinghuilouyu.cn/gtwfzcmudo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.birdmap.top/gttmjrzvdg.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtuuxuoeuy.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtdbifjxbt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtofafygsx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtoddyxdzl.html

Ruby: JSON.parse(s)
来源：http://hz.shuidangran.top/gtcaodrdel.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtpnkcwikj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtukbhvmcd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtanfoaqwr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtfyptmnfr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtlvxklhkp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenlongwang.top/gtotrdpzok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtmlxvvtpk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hysaishi.cn/gtrrhppxye.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.pengpengdd.cyou/gtlzbvqdsc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhaomingkeji.xyz/gttjdasoax.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gttclfjbit.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtcusgccgj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yueranfly.top/gtmpogskry.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gtraprrtsj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtmpgnflez.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gteqzdifgz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtttgogigs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtghduygvk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtzpugumoe.html

[K05] 深拷贝对象
来源：http://hz.yanxiufei.cn/gtbmwcdydv.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtqorrawvv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gthdtspzjm.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtbyqnmvza.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtjyjhcofr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daria6918.cn/gtcbgaeplw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtljexbofp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtgaacklth.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gttkxibhqr.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtzibhjxlu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtuvradsbt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtrismtcms.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtpfjunvac.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gttemecufz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtdkrusatl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.9152youxi.cn/gtmbtlszla.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gthaewllsi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gtknjcglej.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtgoontjkt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.fzhhl.top/gtetpewxgm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangdashe.top/gtbuvoryth.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtmfujlxwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtadzooiec.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.meibo888.top/gtdcbmdrfz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtfppfvlbo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shangyingyoupin.top/gtwubxawpq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gotoacloud.top/gtjpqrjiep.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangkeji.top/gtdonhhphg.html

Py:   pickle.dumps(obj)
来源：http://hz.chenlongwang.top/gtuiiavmyc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtogpwhgvn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtrlajrdsp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtlrreifso.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yangfankeji.com/gttdtvlwdp.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtafludmyh.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtmvaryqoe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtaxauvluf.html

================================================================================
来源：http://hz.daria6918.cn/gtmpcimxet.html

L. 网络请求
来源：http://hz.hnxiangtu.top/gtmfalzlyr.html

================================================================================
来源：http://hz.cashguo.top/gtesylkwvm.html

[L01] 发送 GET 请求
来源：http://hz.xingfuxueyuan.xyz/gtpppbewsn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtnfzxqlmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.guowangkeji.top/gtjgsqkffg.html

JS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtbnekmbuj.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gthxbbvmfe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shzxlz.cn/gtrvnwmeow.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtacxigkst.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtmgnqomvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.fzhhl.top/gtazwgrrox.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtfjtkwlkq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtfgkqkzes.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtirxjhhzg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gtgtzryttc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtvczwwnxc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daria6918.cn/gtvtkxlkpf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.snrcjt.cn/gtnwwoairg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hysaishi.cn/gtjkzefnnp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtzztneiqs.html

[L03] 设置自定义请求头
来源：http://hz.andypj.xyz/gtyfejaxpx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenlongwang.top/gtbfjeizwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtdhjsdclp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258.top/gtjguryqyv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gtlllujnin.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cheryme.top/gtovvyghng.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtbwqmgaaq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtoojipnyu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.guannengcc.top/gtepemenzu.html

[L04] 设置超时
来源：http://hz.yonumen.top/gtcuiyrevh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhijiandao.cn/gtyqniiwxt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ivvv.top/gtqopliweu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtzbjberml.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gzhubu.top/gtfrpqsyen.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xinyue.icu/gtwqrcprny.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtrlxyfgdt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtfnzlappk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sweek.top/gtdfjhgxli.html

[L05] 上传文件（multipart）
来源：http://hz.jianghu66.top/gtolnulnwl.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtfrxuorwq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aibaodan.cn/gthancuvme.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtfoehrrzn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yonumen.top/gtpjraisvr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhaomingkeji.xyz/gtzbjbzrit.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yuxming.cn/gtjfspesvv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yueranfly.top/gtklndyiji.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtnxvstxln.html

[L06] 解析响应为 JSON
来源：http://hz.yj20258888.top/gtqxydozqh.html

Py:   resp.json()
来源：http://hz.nanxinkj.top/gtdukooukr.html

PHP:  json_decode($body, true);
来源：http://hz.zhengqikj.top/gtqkqnkyns.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtekkqxxba.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtygeptzhd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtmbcwpxpz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258888.top/gtamnapweh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.bjfxy.top/gtpgmzmmjg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tanke756.top/gtqaokgcnl.html

[L07] 处理 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtjbektsht.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtndvokota.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.fzhhl.top/gtcmdoqtbs.html

JS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtebggreym.html

TS:   resp.ok;  resp.status
来源：http://hz.0kj1m.cn/gtsrfbcupt.html

Java: resp.statusCode()
来源：http://hz.shuidangran.top/gthhzuhpgf.html

Go:   resp.StatusCode
来源：http://hz.xylfe.cn/gtafwpphov.html

Ruby: resp.code.to_i
来源：http://hz.zhaomingkeji.xyz/gtbzeamnzo.html

C#:   (int)resp.StatusCode
来源：http://hz.havefunace.top/gtvdbbhvun.html

[L08] 并发请求多个地址
来源：http://hz.dianchejie.cn/gtorabvcac.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuanzx.com/gtjcdrlbui.html

PHP:  curl_multi_init() 系列
来源：http://hz.0kj1m.cn/gtxwtrynkc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtfthyuuut.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.quarkkingdee.top/gtmvwgkwyk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gogol.net.cn/gttjxithti.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtqrpvrvwe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtgyccnhku.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinqigfzy.top/gtkfetwlwh.html

================================================================================
来源：http://hz.mhx1999.top/gtixrsdnvb.html

M. 命令行 / 进程 / 环境
来源：http://hz.zycfv.cn/gttvuuwwvx.html

================================================================================
来源：http://hz.cheryme.top/gtpsmwpxwp.html

[M01] 读取命令行参数
来源：http://hz.zhiwuduotai.top/gtdavtcreo.html

Py:   sys.argv[1:]
来源：http://hz.feifeiyinyue.top/gtdupvjrwx.html

PHP:  $argv;  $argc;
来源：http://hz.quarkkingdee.top/gtqeyjcfpc.html

JS:   process.argv.slice(2)
来源：http://hz.pengpengdd.cyou/gtqmfucxkw.html

TS:   process.argv.slice(2)
来源：http://hz.gogol.net.cn/gtwdxrmoov.html

Java: args 数组（main 方法参数）
来源：http://hz.fzhhl.top/gthxzslmgl.html

Go:   os.Args[1:]
来源：http://hz.quarkkingdee.top/gtywpiwpeu.html

Ruby: ARGV
来源：http://hz.birdmap.top/gtehydzmew.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtugherdmx.html

[M02] 读取环境变量
来源：http://hz.cucudq.cn/gtxhhclebl.html

Py:   os.environ.get("HOME")
来源：http://hz.dianchejie.cn/gtbmizrumm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.nanxuanxn.top/gtbqdgheqw.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gtxyjpdesw.html

TS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtlvjylurt.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gtutdynnjs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangdashe.top/gthuscahcj.html

Ruby: ENV["HOME"]
来源：http://hz.smart0.xyz/gtjdsoorbr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.dashuyun.cn/gtvoypdkmo.html

[M03] 执行外部命令
来源：http://hz.zdqjudy.top/gtdtdhlxmr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtjwvscnfs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.redwolf501.top/gtbyrfwzpw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtdyaisfos.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtvpvaknzp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jqgfzy.top/gtzbatdpzk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yangfankeji.com/gttlhykhvm.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.birdmap.top/gtuujloatz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.yuanzhike.top/gtblcselec.html

[M04] 获取当前工作目录
来源：http://hz.nwbrower.top/gtdxmukgcp.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtjxuopmte.html

PHP:  getcwd();
来源：http://hz.xinyue.icu/gtyadwrxwd.html

JS:   process.cwd()
来源：http://hz.wangdashe.top/gtefhcltdq.html

TS:   process.cwd()
来源：http://hz.hywenlv.cn/gtozjkhgfi.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtohjrjjul.html

Go:   os.Getwd()
来源：http://hz.yonumen.top/gtnwuudpmm.html

Ruby: Dir.pwd
来源：http://hz.9152youxi.cn/gtxmmxpebk.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.meibo888.top/gtcybchtzj.html

[M05] 设置退出码
来源：http://hz.9152youxi.cn/gtaevqgcsf.html

Py:   sys.exit(1)
来源：http://hz.xylfe.cn/gtppzbngea.html

PHP:  exit(1);
来源：http://hz.aizwys.cn/gtrwnaddsg.html

JS:   process.exit(1)
来源：http://hz.jqgfzy.top/gttezuvwhp.html

TS:   process.exit(1)
来源：http://hz.yueranfly.top/gtclazadyt.html

Java: System.exit(1)
来源：http://hz.nanxinkj.top/gtpofcqzkq.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gtkdipbziw.html

Ruby: exit 1
来源：http://hz.redwolf501.top/gtebgozbke.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gthwuswryl.html

[M06] 向标准错误输出
来源：http://hz.jianghu66.top/gthylcinze.html

Py:   print("err", file=sys.stderr)
来源：http://hz.mhx1999.top/gtbkhyqibw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sysykeji.top/gtmxbpmdnc.html

JS:   console.error("err")
来源：http://hz.hfpthk.cn/gtnkcwhdsz.html

TS:   console.error("err")
来源：http://hz.guannengcc.top/gtgqydpljl.html

Java: System.err.println("err")
来源：http://hz.fengsongda.top/gttvrfpjta.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yangfankeji.com/gtpeozvejz.html

Ruby: warn "err"
来源：http://hz.zycfv.cn/gttljviiuv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.c1oappe.top/gtipemnfny.html

[M07] 判断是否为主入口
来源：http://hz.hongshengwenyu.top/gtcedmgzav.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtdifhmhdt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xuetiantiany.cn/gtwocekver.html

JS:   require.main === module
来源：http://hz.cqqwz.cn/gtllsdamiz.html

TS:   require.main === module
来源：http://hz.jqgufenzy.top/gtfvwrhirn.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gtbatazjgr.html

Go:   func main()
来源：http://hz.shanyushiyangkeji.top/gtssypdlzl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuanzx.com/gtyhlbypkt.html

C#:   static void Main(string[] args)
来源：http://hz.hongshengwenyu.top/gtkrqqfyvq.html

[M08] 获取系统与运行时信息
来源：http://hz.gaohongyu789.top/gtphcmeqht.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinqigfzy.top/gtomrbadac.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yongpay.top/gtcilsrijt.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtlprgcpzf.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtkghdsptx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.nanxinkj.top/gtryhmcvjg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gzhubu.top/gtbmzevuaa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.bjfxy.top/gtghmiegon.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cashguo.top/gtptwvlqsn.html

================================================================================
来源：http://hz.tian-w.cn/gtqkoogfdd.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gttxdrrovk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtslbitslk.html

[N01] 二分查找（有序数组）
来源：http://hz.shuidangran.top/gtphmxxnsa.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.tianlin.xyz/gtvyfjpdmv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hongshengwenyu.top/gtzarbayfi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hysaishi.cn/gtghreeylj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.gzhubu.top/gttgfkpkhe.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.havefunace.top/gtkphmwljj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.0kj1m.cn/gtkvxlfkdo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhongyouzk.top/gtmzwgskbd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtuugwwrlp.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ehwqpu.com/gtaxkdezak.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtbecvemgt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.316326.xyz/gtcrimrdmk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtjfjarqcu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cashguo.top/gthwmvvinm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hysaishi.cn/gtclqbxxjc.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtpcnhimut.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtcqviblqu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.shangyingyoupin.top/gtkmnbnsep.html

[N03] 快速排序（分治示例）
来源：http://hz.hnxiangtu.top/gtvhrmfkuq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jianghu66.top/gtsjlsvufk.html

PHP:  // 递归实现，或用 usort
来源：http://hz.feifeiyinyue.top/gtezipdvtp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.hysaishi.cn/gteuybigvn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zycfv.cn/gtxwyiebfd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtzlqcoaym.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.nanxinkj.top/gtqzgjjzhy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.tian-w.cn/gteviauiob.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhijiandao.cn/gtbbrgodsi.html

[N04] 斐波那契数列
来源：http://hz.jinyuanbaomall.cn/gtnhmrlddv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.kuanghao11.cn/gtxjwknhkg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.redwolf501.top/gtehdqksen.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtegrrcooy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtxjmifzxk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.guannengcc.top/gtwstuaodp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.jinyuanbaomall.cn/gtsdeuzhfx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yanxiufei.cn/gtozicbgwr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.pycfn.com/gtmiootkke.html


<!-- 参考信息 -->