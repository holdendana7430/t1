代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xziqi.cn/gtivnkcfjt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtuvahploq.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gttmpdychy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xylfe.cn/gtxnhswaih.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhixingplan.top/gtxalrcbof.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtpktjdjsp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtxepbndae.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtjxlgthqe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtbpudhtcw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.0kj1m.cn/gtesslcfto.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hongshengwenyu.top/gtuqpwqmxd.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gtubjgvaya.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtyauyncpb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.smart0.xyz/gtsauxxulf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtalmwrfpy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangkeji.top/gthwtijsjm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtiiflhgju.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtpeknarac.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ywan-chungtsiang.top/gtimqhndas.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gteqbpgtjz.html

================================================================================
来源：http://hz.hfpthk.cn/gtjvqaolxt.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtraycupbu.html

================================================================================
来源：http://hz.andypj.xyz/gtdzhbfmux.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtnitheeiy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtqzzfhqas.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtddugljki.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtridcmfjd.html

TS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtsgzztrsu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtrwkpuosj.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gtdolvuldr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtpevnmlrp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtpzodrmip.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gthxtpcaiu.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtmrvhzzqr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtiydswskc.html

JS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtdzyhyunx.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtnuyjycpn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtfulgcftr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtfmunzrip.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtrzpzxoae.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gaohongyu789.top/gtszgzmpax.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gtyhuromvm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtadcmkfxe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aibaodan.cn/gtckfhizit.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtvmsnepuc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtacwadktk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtwkftciyk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ybcxt.top/gtmnjaycyr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtdxzcdxaa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jqgufenzy.top/gtwbmibfok.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtamihlxqa.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtevwcgqak.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtssrcqurw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtpganfshl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtmafbmtkr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gturoslzsm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shuidangran.top/gtmxmixtwx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgfzy.top/gtgxxkgysi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.daxiang520.top/gtbgmtfjxg.html

[K05] 深拷贝对象
来源：http://hz.fengsongda.top/gtpxcanuxo.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtmdiaqayv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtqgovjdgm.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtfjbvxoex.html

TS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtxibrvbei.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aibaodan.cn/gtiejyswme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gthqtexhfy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtkzlzfivv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hywenlv.cn/gthmizmmth.html

[K06] 解析 URL 查询串
来源：http://hz.jinyuanbaomall.cn/gtgxzpqinu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.iojbl.cn/gtgbjdvfkp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cheryme.top/gtmgiceohd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtueowdxvl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gtihgkdily.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtctpvrjne.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtvfcdupzx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtztimtdtg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.52xcode.cn/gtfqghyqxo.html

[K07] 进制转换
来源：http://hz.yj20258888.top/gtoahejryb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtozdvindj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.haohaochexian.top/gtzgnbiwee.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtpotihuba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtmxsvyzae.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtspdnrrfe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.andypj.xyz/gtccbncorl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtzqckitac.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nanxuanxn.top/gtkrfavgoy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtozgihucc.html

Py:   pickle.dumps(obj)
来源：http://hz.zdqjudy.top/gtsyzlfuqo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sweek.top/gtctkhrsic.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtckpwxmgl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtgnpjsrfy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtzdyubspw.html

Go:   encoding/gob
来源：http://hz.sweek.top/gtmocwtokp.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtgsxcwebf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtqwbxodjd.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtubndnyrg.html

L. 网络请求
来源：http://hz.hnqzz.top/gtvaarjrha.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gthwkaqvjj.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtxvdoxcxi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtzsabutzw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtbehyuapm.html

JS:   await fetch(url)
来源：http://hz.nwbrower.top/gtsacjgeth.html

TS:   await fetch(url)
来源：http://hz.yuxming.cn/gttrrxlner.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.kuanghao11.cn/gtxccjmfaz.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gthvejkjjc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtmdyscjvt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ydjk.org.cn/gtajmqmmfv.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtskgfjaxi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jqgfzy.top/gtplktuclp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.c1oappe.top/gtrepmlzuu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jqgfzy.top/gtsguuqoku.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtwhulwlyy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtjnvrvkgj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenjidiqi.icu/gtdfluuuar.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtlejvdzvk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtblresyln.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gthuyxrizf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aibaodan.cn/gtfnxqlrpy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guowangkeji.top/gtxqgykigy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtqujzvgfo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gthtsqfnxv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yvedp.cn/gtkqavzpls.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtspwwfndw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtlvomuhoi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtjuexuxgy.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtxeedjokc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.wangdashe.top/gtdcvddqxn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtkqlaqrru.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtodmwfpqi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gtyvkiluve.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtqxfhomml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.meibo888.top/gtwxucqgti.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jianghu66.top/gtleziojgj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.svipenyu.cn/gttmytbbxd.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtuezcgnug.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.havefunace.top/gtkgulunpe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yuanzhike.top/gtlzmurgdp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yueranfly.top/gtdoqblbja.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shangyingyoupin.top/gttcrixbrf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtkekhgzuv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zdqjudy.top/gtyvyrwikd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhoulong.xyz/gtjuyzrucq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yonumen.top/gtnghiuxpf.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtnpuxkqns.html

Py:   resp.json()
来源：http://hz.tian-w.cn/gtaljmuehq.html

PHP:  json_decode($body, true);
来源：http://hz.ydzc1.top/gtpozztwwz.html

JS:   await resp.json()
来源：http://hz.nanxinkj.top/gtpdoivgbg.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtvtkavxld.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhoulong.xyz/gtknlifxln.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gttvthkkjp.html

Ruby: JSON.parse(resp.body)
来源：http://hz.9152youxi.cn/gtrncxibgb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jiagoushi.top/gthqziyqlu.html

[L07] 处理 HTTP 状态码
来源：http://hz.dianchejie.cn/gtytrwhpih.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hongshengwenyu.top/gtivozrjcq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gtcqklavpa.html

JS:   resp.ok;  resp.status
来源：http://hz.meibo888.top/gtqpmdkfyw.html

TS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtvrxzgzkk.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gtbvehmphv.html

Go:   resp.StatusCode
来源：http://hz.daxiang520.top/gtklqcdwnp.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtnawvphfw.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtihbsttlk.html

[L08] 并发请求多个地址
来源：http://hz.yanxiufei.cn/gtldesgakq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jqgfzy.top/gtmqawpbsi.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangkeji.top/gtaudmbnzk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtzupfxzja.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yangfankeji.com/gtncjompyr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.316326.xyz/gtmervbckx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtfqlhdmob.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.tianlin.xyz/gtrqfcqfwm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yuxming.cn/gtmfdmksjr.html

================================================================================
来源：http://hz.haohaochexian.top/gtgevgzgaq.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gtbpuotniy.html

================================================================================
来源：http://hz.jinqigufen.top/gtnvidagmj.html

[M01] 读取命令行参数
来源：http://hz.quarkkingdee.top/gtfvxzcmpm.html

Py:   sys.argv[1:]
来源：http://hz.quarkkingdee.top/gtqhhhoykv.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtevvlqriw.html

JS:   process.argv.slice(2)
来源：http://hz.smart0.xyz/gtkjymkpel.html

TS:   process.argv.slice(2)
来源：http://hz.aizwys.cn/gtusgkgtiv.html

Java: args 数组（main 方法参数）
来源：http://hz.meibo888.top/gtzlxvvghz.html

Go:   os.Args[1:]
来源：http://hz.tian-w.cn/gtcicnaqpb.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtxzhmwldt.html

C#:   args 数组（Main 方法参数）
来源：http://hz.dashuyun.cn/gtfnemjwcr.html

[M02] 读取环境变量
来源：http://hz.jinghuilouyu.cn/gtaflpnves.html

Py:   os.environ.get("HOME")
来源：http://hz.havefunace.top/gtaqtrffzv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ydzc1.top/gtbjfazfft.html

JS:   process.env.HOME
来源：http://hz.zycfv.cn/gtedcneqzk.html

TS:   process.env.HOME
来源：http://hz.shuidangran.top/gtnvxfgtjs.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtivikpbfu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.0kj1m.cn/gtkyfmwcnc.html

Ruby: ENV["HOME"]
来源：http://hz.cqqwz.cn/gtketgsxre.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangshuangyany.cn/gtxfxldufw.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gtytxkzhkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jqgufenzy.top/gtnozjkbdh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shanyushiyangkeji.top/gtsaqtbmgq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtxyrfguhv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hysaishi.cn/gtuhurabio.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shanyushiyangkeji.top/gtwyajigrf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhijiandao.cn/gtsakkmwcu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuanzx.com/gtcxcqkfoo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhoulong.xyz/gtyzbcfyez.html

[M04] 获取当前工作目录
来源：http://hz.shanyushiyangtech.top/gtxxqlnfvn.html

Py:   os.getcwd()
来源：http://hz.chenzaomai.com/gtmyhlbzul.html

PHP:  getcwd();
来源：http://hz.zhaomingkeji.xyz/gtconwjaft.html

JS:   process.cwd()
来源：http://hz.gzhubu.top/gtnheymbrp.html

TS:   process.cwd()
来源：http://hz.9152youxi.cn/gtxtwpnfea.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhengqikj.top/gtaznnjesi.html

Go:   os.Getwd()
来源：http://hz.hnxiangtu.top/gtzirepskc.html

Ruby: Dir.pwd
来源：http://hz.c1oappe.top/gtjtmykshh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtanwmhbjv.html

[M05] 设置退出码
来源：http://hz.ydjk.org.cn/gtpxiswjld.html

Py:   sys.exit(1)
来源：http://hz.hysaishi.cn/gtdhohatbo.html

PHP:  exit(1);
来源：http://hz.feifeiyinyue.top/gtxkyhngpp.html

JS:   process.exit(1)
来源：http://hz.yj202588.top/gtheaggtmg.html

TS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtbbyzkxyf.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gthzjefsiw.html

Go:   os.Exit(1)
来源：http://hz.xylfe.cn/gtavbobsrr.html

Ruby: exit 1
来源：http://hz.xziqi.cn/gtdiuumdpo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.bjfxy.top/gtjlxwhfsh.html

[M06] 向标准错误输出
来源：http://hz.dashuyun.cn/gtnfecxdvj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sufxvd.cn/gtliorzspb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yvedp.cn/gtqbovrhtw.html

JS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtsnjzevcw.html

TS:   console.error("err")
来源：http://hz.yueranfly.top/gtxxqadoja.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtzrsdnhyw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtgazggcrv.html

Ruby: warn "err"
来源：http://hz.yj202588.top/gtpyqkpugd.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yvedp.cn/gtdeadrzgl.html

[M07] 判断是否为主入口
来源：http://hz.xuetiantiany.cn/gttrfpzpei.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtbjxavfnu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinqigfzy.top/gtctpauqbe.html

JS:   require.main === module
来源：http://hz.hfpthk.cn/gtvzjishxc.html

TS:   require.main === module
来源：http://hz.zhengqikj.top/gtfwdvvwlz.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtfrfugdiu.html

Go:   func main()
来源：http://hz.quarkkingdee.top/gtexymuzzp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.snrcjt.cn/gtfnvqhsgy.html

C#:   static void Main(string[] args)
来源：http://hz.wangshuangyany.cn/gtgvrbnnsr.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gtsgouumoa.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gtwlejmybx.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtjtnpyroz.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangtech.top/gtylizzcps.html

TS:   process.platform;  process.version
来源：http://hz.xuanzx.com/gtvkramncf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.guowangkeji.top/gtyltayttl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtwvipotcu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yangfankeji.com/gtexvpnbxe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.tian-w.cn/gtlqagqzzc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtdsmtmkoy.html

N. 数据结构与算法
来源：http://hz.0kj1m.cn/gtkycshhfn.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcnmtykde.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtwkgwweif.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtbpmjvtdg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.guannengcc.top/gtpibqoaza.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtzopeewvn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtrwzlewbs.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.andypj.xyz/gtdjwwdtey.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtxzaqionu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtpfhgjwyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.316326.xyz/gtpsjooyoh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.sufxvd.cn/gtjftjyzcf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinghuilouyu.cn/gtycwhccxu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.shanyushiyangkeji.top/gtbioccwez.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.kuanghao11.cn/gtmlxeumvv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtqedxglel.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtogwbpxkr.html

Go:   slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtzshqojir.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gthjscirhp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtwlotrgqe.html

[N03] 快速排序（分治示例）
来源：http://hz.cqqwz.cn/gtqncckakj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.nanxinkj.top/gtmormcmmj.html

PHP:  // 递归实现，或用 usort
来源：http://hz.fengsongda.top/gtmezojwpi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.cheryme.top/gtxleosvrm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.aizwys.cn/gtssjkzvye.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yonumen.top/gtrwbtxwqt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhongyouzk.top/gtfdvgmsqi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sysykeji.top/gtatybhelz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yj202588.top/gtrrvxsggc.html

[N04] 斐波那契数列
来源：http://hz.gzhubu.top/gtlxvhozvk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.fengsongda.top/gttweyqvbu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.gzhubu.top/gttgqqzmod.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ppjwa.cn/gtyxkygybx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtbiggdqub.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.yuxming.cn/gtnovbokom.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.shuidangran.top/gtepxdoefp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gzhubu.top/gtknwkcqnc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtjhixslxv.html

[N05] 最大公约数
来源：http://hz.jiagoushi.top/gtbhtakdpu.html

Py:   math.gcd(a, b)
来源：http://hz.ywan-chungtsiang.top/gtiobamfmd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigufen.top/gtedwuqzfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tianlin.xyz/gtfikcyteg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gttjtsdgmf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.aizwys.cn/gtpjqajhic.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.cashguo.top/gtendhmoec.html

Ruby: a.gcd(b)
来源：http://hz.zhijiandao.cn/gtqbkdfmcf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.ydjk.org.cn/gtrtsaexbs.html

[N06] 判断回文字符串
来源：http://hz.sufxvd.cn/gtoygtlbih.html

Py:   s == s[::-1]
来源：http://hz.ybcxt.top/gtlkajshrk.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtjadggjbl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtaeaxrdai.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtxsqforzc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.shuidangran.top/gtjqarhdjl.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gtqitmrcle.html


<!-- 参考信息 -->