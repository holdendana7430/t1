代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gtbyjoklzs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.vqdsnc.cn/gtkxutukhy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtqitgsfaj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtogfvcexk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtahnxzxcf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtnrvggtzr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtethvbcrk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtzmflvevq.html

================================================================================
来源：http://hz.ydjk.org.cn/gtvioprjko.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtpddtibbt.html

================================================================================
来源：http://hz.ppjwa.cn/gtjayynsao.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtfgmrkqip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pengpengdd.cyou/gtdlgdiljo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtoqymvwbc.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtduxwlryd.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtlmnjyngh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtxerpvcqz.html

Go:   json.Marshal(obj)
来源：http://hz.yuanzhike.top/gtbedzkxex.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.quarkkingdee.top/gtsgpscxcl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtbgbsolba.html

[K02] JSON 字符串转对象
来源：http://hz.yvedp.cn/gtpradtmbk.html

Py:   json.loads(s)
来源：http://hz.yueranfly.top/gtvlsqzlyd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cashguo.top/gtrxkcbnvn.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtwsjrdgzo.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtfjphximc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtdzdpflry.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtdcbjfjwr.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gtaidoingh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xinyue.icu/gtnmfvgapp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtnooepljw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtdjnlrmfs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtqcxgkuib.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtlohdhvyt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gttjpvuuca.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtakbmvhbn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xingfuxueyuan.xyz/gtsmmlksht.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuanzx.com/gtztdsdktu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtltdpzdcy.html

[K04] 读取 JSON 文件
来源：http://hz.hfpthk.cn/gtuzmaaejm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhixingplan.top/gtdgcezdsy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cdnleiting.top/gtknvmdumx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtctdijtwe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtzepnmhtc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtgixkdkzh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtrdthffwp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtglxpxmhl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtmkqjvrbp.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtbviyjqel.html

Py:   copy.deepcopy(obj)
来源：http://hz.52xcode.cn/gtbiqvojzo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinghuilouyu.cn/gtggzcbsvz.html

JS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtxmmiorfu.html

TS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtxindxorb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhijiandao.cn/gtpwvmowuf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtlxbercrw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.feifeiyinyue.top/gtugvgeded.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gtvcoulezs.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtgyehonan.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtgrrfhepe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.feifeiyinyue.top/gtaltqmjcl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtylmqbwys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtzzaclrhx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tanke756.top/gtaoqtbomf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj20258888.top/gtnvaggrwx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hnqzz.top/gtlugheqmr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gotoacloud.top/gtiawlwqmw.html

[K07] 进制转换
来源：http://hz.316326.xyz/gtaopynjjy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jqgufenzy.top/gtkwmbjrvf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gotoacloud.top/gtfzwkfmzl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtdcpxslqq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtxfpnrvnd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtvfxnkewn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtttbpsjjd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtufsfjows.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gthcssmbba.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hywenlv.cn/gtqwnwtkda.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtvgbiisgq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.dianchejie.cn/gtydiieqwv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gttzhllcqg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtocychxpp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shuidangran.top/gtpuaprscn.html

Go:   encoding/gob
来源：http://hz.yj202588.top/gtxcymbqak.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gthwdcdxqf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtmtbdrpsk.html

================================================================================
来源：http://hz.sxryk.cn/gtqdfechsk.html

L. 网络请求
来源：http://hz.shanyushiyangtech.top/gtsyfgdhjw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtekxzacvb.html

[L01] 发送 GET 请求
来源：http://hz.wangdashe.top/gtwmqxcmak.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtldkazmzn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtylrrlwpa.html

JS:   await fetch(url)
来源：http://hz.ydzc1.top/gtkrogzjho.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtgjdaglup.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shanyushiyangtech.top/gtihbrzlgn.html

Go:   resp, err := http.Get(url)
来源：http://hz.cucudq.cn/gtlplgsntc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gtfcejhmrj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gthgqleqxu.html

[L02] 发送 POST JSON
来源：http://hz.tian-w.cn/gtegjmljkl.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtrgpqwbjk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gtexgqzhss.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtnuqgvebk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtzuywhjgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtnlcarxdb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhiwuduotai.top/gtopvsefab.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.yuxming.cn/gtpaywlwcw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.guowangkeji.top/gttveeofqx.html

[L03] 设置自定义请求头
来源：http://hz.havefunace.top/gtppnweqos.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhengqikj.top/gtexofuapd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtzgyfpyes.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj202588.top/gtfqecmodi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtnflnhnjb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtvrqpqzpv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.c1oappe.top/gtmrhgniad.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xylfe.cn/gtzlhzjkly.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtsvzftnfm.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtmauizzah.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258888.top/gtbwxzvyyg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtblvdjfzs.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sufxvd.cn/gtnaffjhqx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtebpwetyi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gttvzohgcl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258888.top/gtukiqqqtq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gtvronpvmb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xylfe.cn/gtiyqqdvkv.html

[L05] 上传文件（multipart）
来源：http://hz.ydzc1.top/gtgwvqurvm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.cdnleiting.top/gtfzthwtxo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinyuanbaomall.cn/gtsdvzhzif.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtypdupdnv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtsfpopjar.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zycfv.cn/gtcnjkgfaz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.9152youxi.cn/gtydkbccyj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shzxlz.cn/gtwnhdpsno.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.bjfxy.top/gtrqnitqoc.html

[L06] 解析响应为 JSON
来源：http://hz.xinyue.icu/gtigpmpczg.html

Py:   resp.json()
来源：http://hz.sufxvd.cn/gtonkbtbuk.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtwahnzzij.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtueakzjym.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gteowjvxgl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guannengcc.top/gtluspvwqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cashguo.top/gtidnbblqb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhongyouzk.top/gtovrxltio.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hywenlv.cn/gtahkbyvvx.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtjghuzusg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tianlin.xyz/gthhwdxple.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.hysaishi.cn/gtjxwtxknh.html

JS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtwfdurcyh.html

TS:   resp.ok;  resp.status
来源：http://hz.xingfuxueyuan.xyz/gtqumofshq.html

Java: resp.statusCode()
来源：http://hz.ydjk.org.cn/gthrmsuwdm.html

Go:   resp.StatusCode
来源：http://hz.andypj.xyz/gtyqddaczd.html

Ruby: resp.code.to_i
来源：http://hz.shuidangran.top/gtwpiscewf.html

C#:   (int)resp.StatusCode
来源：http://hz.zycfv.cn/gtlfaqtplk.html

[L08] 并发请求多个地址
来源：http://hz.jqgfzy.top/gtfbjhmvcx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinyuanbaomall.cn/gtihwtpujn.html

PHP:  curl_multi_init() 系列
来源：http://hz.9152youxi.cn/gtkaolzmzw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.c1oappe.top/gtqpydzuxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtwebkelqs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinqigufen.top/gtzcpdsaux.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xinyue.icu/gtemkozovp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jiagoushi.top/gtfkwfdtru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.xuanzx.com/gtfojjzkcp.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmsjpzcvr.html

M. 命令行 / 进程 / 环境
来源：http://hz.shangyingyoupin.top/gtwfhnzhxq.html

================================================================================
来源：http://hz.yuxming.cn/gtcvfnklbl.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtomtndtpq.html

Py:   sys.argv[1:]
来源：http://hz.yonumen.top/gtamwmlpvg.html

PHP:  $argv;  $argc;
来源：http://hz.tianlin.xyz/gtuwtxgsiw.html

JS:   process.argv.slice(2)
来源：http://hz.mhx1999.top/gtwafbmsbq.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtmrjzdmsm.html

Java: args 数组（main 方法参数）
来源：http://hz.zhengqikj.top/gtzqpamvge.html

Go:   os.Args[1:]
来源：http://hz.guowangkeji.top/gtjmrapdga.html

Ruby: ARGV
来源：http://hz.sxryk.cn/gtiufnurww.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ybcxt.top/gtypxvlklw.html

[M02] 读取环境变量
来源：http://hz.shangyingyoupin.top/gtuffibdim.html

Py:   os.environ.get("HOME")
来源：http://hz.jlsjyb.cn/gtybxiczeu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnqzz.top/gtesgjzvqk.html

JS:   process.env.HOME
来源：http://hz.tianlin.xyz/gtaindlpyh.html

TS:   process.env.HOME
来源：http://hz.gotoacloud.top/gtbmjjflkf.html

Java: System.getenv("HOME")
来源：http://hz.yj20258888.top/gtgqegktid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhongyouzk.top/gtbnovafep.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtflnzudkr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.smart0.xyz/gtyxdnrzkp.html

[M03] 执行外部命令
来源：http://hz.aizwys.cn/gtkwavxada.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.guowangkeji.top/gtigkhbiqc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydzc1.top/gtlktaztkw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.mhx1999.top/gtanfupdpn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtnqnyszez.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.c1oappe.top/gtegzmscxe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zhoulong.xyz/gtoxaidcsr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenjidiqi.icu/gtuquklvyo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.andypj.xyz/gtbzvuiuju.html

[M04] 获取当前工作目录
来源：http://hz.sufxvd.cn/gtrgetbuuz.html

Py:   os.getcwd()
来源：http://hz.yj202588.top/gtqtmwgtsx.html

PHP:  getcwd();
来源：http://hz.xuetiantiany.cn/gtmwchtewy.html

JS:   process.cwd()
来源：http://hz.0kj1m.cn/gtiqylrxwa.html

TS:   process.cwd()
来源：http://hz.ydjk.org.cn/gtmgzdbgyj.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sweek.top/gtthirwleh.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtulmptyaz.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtskndvjxf.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hongshengwenyu.top/gtbtivkmbg.html

[M05] 设置退出码
来源：http://hz.cdnleiting.top/gtijjhyxua.html

Py:   sys.exit(1)
来源：http://hz.yongpay.top/gtduwuqllo.html

PHP:  exit(1);
来源：http://hz.quarkkingdee.top/gtifdtajoz.html

JS:   process.exit(1)
来源：http://hz.mhx1999.top/gtkqbndhoe.html

TS:   process.exit(1)
来源：http://hz.jinqigufen.top/gtcoumamly.html

Java: System.exit(1)
来源：http://hz.gaohongyu789.top/gtqmhvsfct.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtvobdmvkw.html

Ruby: exit 1
来源：http://hz.zhiwuduotai.top/gtdrdwcnho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.smart0.xyz/gtlkiaokok.html

[M06] 向标准错误输出
来源：http://hz.wangshuangyany.cn/gtaswziohd.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtxkzffdpf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nanxuanxn.top/gtczaligvr.html

JS:   console.error("err")
来源：http://hz.quarkkingdee.top/gtjroyhzmw.html

TS:   console.error("err")
来源：http://hz.svipenyu.cn/gtdlwzndpr.html

Java: System.err.println("err")
来源：http://hz.shanyushiyangtech.top/gthlnstino.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.316326.xyz/gtaoxyiiux.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtfihqoyps.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.xuetiantiany.cn/gtabqzgvcf.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gttiwppfqg.html

Py:   if __name__ == "__main__":
来源：http://hz.shuidangran.top/gtqaavsljl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenlongwang.top/gtieiayeqi.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gtekesdbql.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtqqsolqvv.html

Java: public static void main(String[] args)
来源：http://hz.dashuyun.cn/gtnzpjtmeu.html

Go:   func main()
来源：http://hz.gzhubu.top/gtmhvrcqpr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aibaodan.cn/gtbehvlmwi.html

C#:   static void Main(string[] args)
来源：http://hz.xinyue.icu/gtxvmhjtsv.html

[M08] 获取系统与运行时信息
来源：http://hz.nanxuanxn.top/gtubffkwot.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gthrvgoixf.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhengqikj.top/gttccmsksy.html

JS:   process.platform;  process.version
来源：http://hz.yj202588.top/gtaskroxsg.html

TS:   process.platform;  process.version
来源：http://hz.jinqigufen.top/gthquuxjzr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pengpengdd.cyou/gtsqndlifj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aizwys.cn/gtqpstcodb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhengqikj.top/gtfmohdtqe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtuxrdafqm.html

================================================================================
来源：http://hz.shzxlz.cn/gtacdrxsax.html

N. 数据结构与算法
来源：http://hz.nanxuanxn.top/gtzljvxomu.html

================================================================================
来源：http://hz.yj202588.top/gtvqyoralq.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtnxlflprr.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.ydzc1.top/gttpdzmsss.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yanxiufei.cn/gtminxgjvz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtxcjemuqn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hnqzz.top/gtbfanwafj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shuidangran.top/gtlmryfjwf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.shuidangran.top/gtxcznlvmy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.pycfn.com/gtctffculy.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.9152youxi.cn/gtcmttpcjb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhijiandao.cn/gtmznorsxh.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hongshengwenyu.top/gtwrqkplla.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.fengsongda.top/gtumwpiqho.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangkeji.top/gtwwngtvnv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.9152youxi.cn/gtwmypwakq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtqqaufdnt.html

Go:   slices.Sort(arr)
来源：http://hz.sysykeji.top/gtntvdinvz.html

Ruby: arr.sort
来源：http://hz.nanxinkj.top/gtjpobjdoj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.birdmap.top/gtyggistmh.html

[N03] 快速排序（分治示例）
来源：http://hz.jinghuilouyu.cn/gtfplxkvwr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.zhongyouzk.top/gtysuzpbea.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xuanzx.com/gtazfowmja.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nanxuanxn.top/gtkgaxjcyt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtbsxesqdw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.guowangkeji.top/gtzbppgxco.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.kuanghao11.cn/gtkcynbwif.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.birdmap.top/gtjhbgspfn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.meibo888.top/gtydcnqshv.html

[N04] 斐波那契数列
来源：http://hz.gaohongyu789.top/gtkkcowbvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.nanxuanxn.top/gtloncjjck.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.hywenlv.cn/gtjbecnpbi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gtwocjkzkr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.tianlin.xyz/gteeelayxa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.nanxuanxn.top/gtijtjsjxx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.redwolf501.top/gtlynfrdwg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtkujyamkh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jqgfzy.top/gtkplqbmnx.html

[N05] 最大公约数
来源：http://hz.iojbl.cn/gtzpayisss.html

Py:   math.gcd(a, b)
来源：http://hz.9152youxi.cn/gtqetrrfco.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.mhx1999.top/gtajrzinoe.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.guowangkeji.top/gtnbizpnoo.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fengsongda.top/gtbvrnahik.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ivvv.top/gtmfyfddbd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ywan-chungtsiang.top/gtqfyeohjw.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtwgknbbyc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yonumen.top/gtiwssibgp.html

[N06] 判断回文字符串
来源：http://hz.vqdsnc.cn/gtvbqokqua.html

Py:   s == s[::-1]
来源：http://hz.xuanzx.com/gtjvifsjbl.html

PHP:  $s === strrev($s);
来源：http://hz.zycfv.cn/gteqvbdfva.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shanyushiyangkeji.top/gtecqxmimz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtjjadhoyr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cheryme.top/gtvhbbktcn.html

Go:   // 双指针从两端比较
来源：http://hz.nanxinkj.top/gtadhdgtlv.html

Ruby: s == s.reverse
来源：http://hz.zhaomingkeji.xyz/gtmnotoxqv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.xziqi.cn/gtyairgnlp.html

[N07] 两数之和（返回下标）
来源：http://hz.pycfn.com/gtdkogelko.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.yj20258.top/gtvwhjodwe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cucudq.cn/gtxspgwvvi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.hfpthk.cn/gtgfmjfvjx.html

TS:   // 手写 Map<string, number>
来源：http://hz.c1oappe.top/gtduskieem.html

Java: // 手写 HashMap
来源：http://hz.316326.xyz/gtaauwpbrm.html

Go:   // 手写 map[int]int
来源：http://hz.ydjk.org.cn/gtneohvxnm.html

Ruby: // 手写 Hash
来源：http://hz.sxryk.cn/gtwqtqnxum.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.hnxiangtu.top/gtdcpaqwgz.html

[N08] 生成全排列
来源：http://hz.bjfxy.top/gthytwlafw.html


<!-- 参考信息 -->