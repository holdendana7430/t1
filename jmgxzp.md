代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2aaailpse.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2dpabrnnk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2zwkpxlll.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2rgysfvem.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2fuvmeilh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2gjwaxkpp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2khgtitji.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2pobbfflz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2rktpkydt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2mqqcaoxv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2yrtblkuu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2sitrggww.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2fxzcezts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2fppumbbv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2pcgzcpus.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbcwqaw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sywyvzzk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jhwflaro.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2dxbocrys.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnopuquz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfwjtqix.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2wipqnwbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgsckquv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ytxvokuw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2gjlnbcow.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qurpdhyy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2culdcjeb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2oyvwyeub.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2yfqnlxix.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2intstmvi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2woqzgtun.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szoichjq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2liaumxox.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xepxucuo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2lyzfzkof.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2smzefpul.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lukqzrsw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2npwywadw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sbhmosvv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gnhcfbhd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2haeeusqp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ffwluqwj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2cvzfimnr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qyobizgm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xjsshulk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pekpksck.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2szsmaaaf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lsfpqwpv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oafygttp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qelhphlr.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkohvgrn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sywgaknv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2eiejgaap.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ejusztie.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dxyajncp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bhjquugv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2pycmkspw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vcirvtws.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lljlwyxw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kzjehdma.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crvepstd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2uvamvxzc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ckdizdrz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ukobkqwt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2zkxegrhd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2slgjotpc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lbhmjepa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nbksvooh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2shlkzpqk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cbdgpyoz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2pjytnjxh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwedorg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hxgryxxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sulraejz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dhxvzolm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lisctrmk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xbjmdmpu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pklylrgy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jvnnbpnw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2yvaoouiz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2loxcnoqi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2alxrlhar.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qiaheuer.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cudoywey.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2shtcabsd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsspzjt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2vvbvatgn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jxnjralf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2npcgybfi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2avcamvus.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lcvkxayb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2snhczsyf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vgqclygi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ctagnfiq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fjevjrha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eccippjv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2sprcdfpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzxjpvun.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2phqvqawn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2icnpyfbx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wqvdrgle.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2rszlicnw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kxbbuxax.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qlrkltls.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kryccxmy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2chpcciyt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mpcafjov.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fgmdmwcr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yshdkuxx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qoblcfvn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2drcpauto.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ewcuwyow.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uiillxjy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2buhqcvjy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vyyofodc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfnqutkz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2ggywjthq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xtjdaqtv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vheomjuk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2elhdsmie.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xuhkxbcq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2zwjljhed.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xdctefao.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2txwdnnep.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ycseirsj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ezsiavhn.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2refkxlub.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qqhvdaya.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jvtelpyl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2glfimjxw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ogtxndaf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dktjzxvh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rsgncilr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kbtxozyg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dpzjzypg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ulmhugbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bkolcpdp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tceassfh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2itiadrbj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2sbbzwbbf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vngtubup.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pyyuksmb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vckwbjqk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hitrrptr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sbwdzuoz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tetcjtbe.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ylbswufa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hgayxmbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gmydlgdz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2xttfeauo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yfmbwaeu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2rugandwx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vedmvsgt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2alhxzbte.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rvvtmafe.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jcrsvxxn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uttuchpt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pbojxucc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2izlhozfq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2sunfqicx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mydlmtyy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jmazrdyp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xxhoubuz.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ffcqmrun.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2irwwbdrv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qtuzyauo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cvsqqjfw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ayofaqaz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qpjplapp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2chwkinju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akvbpnax.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2dkznicun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjukxmsc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xnmtyrlg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qjezzalr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ukjpuvmf.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rdhzmyuk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tqytrtpc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2rxtkabid.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2evlwxboi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2nfbvhoea.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jetnoonf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kyusncit.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vrhgumwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vgibbszd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2famsonhx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ojpwuwms.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tzadnxyf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bildnrba.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hioygmwr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iuvaajad.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2czhjgjyf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mijixheg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2irroilea.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xwtzmvtv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ufmydrll.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2nzsuuypf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2azagwrms.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2exdrmbiq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lprzgfld.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uowtbopz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zssqeosi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2gbqppquo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yxevcyby.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jagdilgy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ipgztfgf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2yfvneapm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2tbsplxtu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ngvcdjqy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2hwfzqkli.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xiyjrxxj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2luhqiqgf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yegqkbto.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eipmorxq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fwetkrsi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvwkbaok.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ycxgukkv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vrqxbzbd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tzbukhbl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2hklripls.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2tpscwtci.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zjzpkqgf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tamuobih.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rjjrnjfg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfvaqtde.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2licdjqrp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wwjablzl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2adsgngvt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wgwvflru.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vehijmez.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ffavhlgq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2duadrncz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2vvdhysax.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lupcewmw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hgbecerj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ckffnief.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rnkqrvck.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ffrwtzho.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2mitrccyg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2gxekgjmn.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uoordyhh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2krypuecx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2alwmjfcy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kqlaamxe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jhkikrec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2juvlutxw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pwmxzhdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pssikkut.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2epbatlih.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xuyflgql.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yorsgiih.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fiqloynj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mbodetqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjpftzhp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iyhtorjf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zzpwmraf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xximyzbo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dmxcdrji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2yyjawjxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2welyltlg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2imuvheik.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2akuhjdrc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2varzfxrr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yoboywez.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fffxkbtn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lgjvfgdw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qunamfpe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qhpxvdjr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2saygzicn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iipohftq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ankqooht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tsjyudpg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2gyuttdjo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2twavcueb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2cjwjsgvy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2byosgpqu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sklerpoa.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2lzwxmhcq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2imiwbujq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ffxrcbqd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkcfkfnt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ylnfagru.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dsoxjuok.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zttmmljy.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2fidalein.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eybmcohj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lecxefwu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhagdunz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jxpmarau.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2biqbyetk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lpincypi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xxtdpllm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xujppsok.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hrtwgnfd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ecnpbyyd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yzhtgrew.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfiqjhg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eojpfdqv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tfrwopqu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2wvqplmjj.html


<!-- 参考信息 -->