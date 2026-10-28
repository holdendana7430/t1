代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aizwys.cn/gtwgjnvfdu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydjk.org.cn/gtpdqeoeny.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cqqwz.cn/gtuotjeyyj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gtkeahbick.html

================================================================================
来源：http://hz.zhijiandao.cn/gttsqplgmq.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtgpkhphuv.html

================================================================================
来源：http://hz.gaohongyu789.top/gtfpbmnbon.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtvdyqabyt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtmerrkdwm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtghxrjvux.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtqyikwimy.html

TS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtrhayrayd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gteqrdfevb.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gtpzsyhufu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtohxwnbdq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtrixcdfhc.html

[K02] JSON 字符串转对象
来源：http://hz.gzhubu.top/gtobtjvybp.html

Py:   json.loads(s)
来源：http://hz.jinqigfzy.top/gtnwvfuxgb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtijyotptl.html

JS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtsvvvdpbz.html

TS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtjqrluves.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtpqoagipv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtkbqvxkes.html

Ruby: JSON.parse(s)
来源：http://hz.meibo888.top/gtumaforcx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtmdhvanck.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gttnrmtdbd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtmbiqbfsi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtwbqqaork.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtlbhdymbg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtjshmipow.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtfnycnfgt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gtnfmaotkq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtlbbwkyck.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gttrbklzdv.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtcbejtaks.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtdfhbvodj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtmdnjrpgv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtmrhpukrd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtkfgdoxmm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenjidiqi.icu/gtfoytjten.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtszqsqmur.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yongpay.top/gtpodsaski.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj202588.top/gtvjkhetrg.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtzmrjkfgm.html

Py:   copy.deepcopy(obj)
来源：http://hz.jqgufenzy.top/gtozqdhszv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtklvjaakq.html

JS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtbvofqevu.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtdoyhohvs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtnaeshfxu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhiwuduotai.top/gtryjtfjys.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gtlmdyglku.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gttyizpgud.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gthfraptdk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtyxwgfqca.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yanxiufei.cn/gttrglibzo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtmmoswdud.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtejyrpske.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtfqjcixid.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gzhubu.top/gtukhfpiax.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtrfndxbtn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ivvv.top/gtvbptkxjg.html

[K07] 进制转换
来源：http://hz.tanke756.top/gtcjtvvior.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtpycilitd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtfjhiytow.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtatzapqgk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtbhurgbdz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gteduswcgt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinyuanbaomall.cn/gtpwibmqkp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtriquprux.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtdvmthgev.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtsiurjdzo.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtgeojoosj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtnqajzboz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtwegyungk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.316326.xyz/gtnhgntfqr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtwwogwyxz.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtlcxlguhe.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gtittvmuap.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.feifeiyinyue.top/gtuczgbmfx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtiygvfibk.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtjgpsigzt.html

================================================================================
来源：http://hz.yj20258.top/gtwqwbmgho.html

[L01] 发送 GET 请求
来源：http://hz.dianchejie.cn/gtbgtknlyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yj20258888.top/gtlfgnevbk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhoulong.xyz/gtelrataft.html

JS:   await fetch(url)
来源：http://hz.yj20258.top/gtidjspqse.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtwljqaeby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hongshengwenyu.top/gtqhtqntgj.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxinkj.top/gtiexldoiy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnxiangtu.top/gtalxbtsci.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gtutdtepzu.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtqkodxhxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhengqikj.top/gtstlqiqyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtfwpbynws.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gttvsravzw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gzhubu.top/gthiprcphs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtjjqydppe.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtvglozpkp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtinusvmpc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenjidiqi.icu/gtwoldannn.html

[L03] 设置自定义请求头
来源：http://hz.xinyue.icu/gtwwvpuqfg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnxiangtu.top/gtxzlsrsyc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tian-w.cn/gtrcjgjlzr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nwbrower.top/gtlqaghmns.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtzfedokei.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xinyue.icu/gtnjdksgoq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtcjjxjpps.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fzhhl.top/gtxiuygmxp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtmlvsfqwn.html

[L04] 设置超时
来源：http://hz.xuetiantiany.cn/gtlyytuqqk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cashguo.top/gtnjyqxmnn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jiagoushi.top/gtsolvggws.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtkcznnwrl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnxiangtu.top/gtcpjgbzdc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cashguo.top/gtzgraewzb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cucudq.cn/gtjrilqajc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtyskextao.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtjmcvilze.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtdncrunan.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtpdswtjnw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gaohongyu789.top/gtxenbakdj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtljvcepzv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtgabayzjw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtobrdrogi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtdnpyfrju.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hfpthk.cn/gtiscibhap.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenlongwang.top/gtkdblqqzr.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtjoofedxq.html

Py:   resp.json()
来源：http://hz.tanke756.top/gtvaflpofg.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtmpvsumwi.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtkbxeyoal.html

TS:   await resp.json()
来源：http://hz.zdqjudy.top/gtijefthqy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yvedp.cn/gtdvmcjaev.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gtxvefldkf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gtdmdpuqyk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yongpay.top/gtmxvpduxm.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigfzy.top/gtvauoxfaf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ydzc1.top/gtodtipead.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.andypj.xyz/gtarkblttw.html

JS:   resp.ok;  resp.status
来源：http://hz.tian-w.cn/gtboztbffg.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtehheagew.html

Java: resp.statusCode()
来源：http://hz.wangdashe.top/gturwsntvc.html

Go:   resp.StatusCode
来源：http://hz.gotoacloud.top/gtmbcrtocj.html

Ruby: resp.code.to_i
来源：http://hz.ydjk.org.cn/gtolbccixs.html

C#:   (int)resp.StatusCode
来源：http://hz.cucudq.cn/gtovzmbnqz.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gttnxnhvnt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangtech.top/gtjxrooekt.html

PHP:  curl_multi_init() 系列
来源：http://hz.dashuyun.cn/gtzqlvxayv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hongshengwenyu.top/gtbilcwuxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.snrcjt.cn/gtuhspjuuz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.iojbl.cn/gtxgpbdtqi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.mhx1999.top/gthkxxglkd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtqheqbcin.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shzxlz.cn/gtjdgzwovr.html

================================================================================
来源：http://hz.zhijiandao.cn/gtdwmpjpsv.html

M. 命令行 / 进程 / 环境
来源：http://hz.yueranfly.top/gtebqewczi.html

================================================================================
来源：http://hz.smart0.xyz/gteswejxsk.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtghgqubxu.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtlfmwrazq.html

PHP:  $argv;  $argc;
来源：http://hz.yuanzhike.top/gteskhdpzt.html

JS:   process.argv.slice(2)
来源：http://hz.jqgufenzy.top/gtfoujzssz.html

TS:   process.argv.slice(2)
来源：http://hz.chenjidiqi.icu/gtpioijhgv.html

Java: args 数组（main 方法参数）
来源：http://hz.ppjwa.cn/gtckooflgv.html

Go:   os.Args[1:]
来源：http://hz.zdqjudy.top/gtvwqfnxlw.html

Ruby: ARGV
来源：http://hz.haohaochexian.top/gtwjumzjqm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtrzwlbrvz.html

[M02] 读取环境变量
来源：http://hz.yj202588.top/gtlhvnhwyb.html

Py:   os.environ.get("HOME")
来源：http://hz.dashuyun.cn/gtipqeagkr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cdnleiting.top/gtwlzyenjr.html

JS:   process.env.HOME
来源：http://hz.redwolf501.top/gtenhmojpc.html

TS:   process.env.HOME
来源：http://hz.ehwqpu.com/gtdhbavfpq.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtjuuzxqli.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gteigwffst.html

Ruby: ENV["HOME"]
来源：http://hz.cucudq.cn/gtddraazzb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinyuanbaomall.cn/gtiyeazelb.html

[M03] 执行外部命令
来源：http://hz.yj20258.top/gtghbxhbfi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.c1oappe.top/gtturyrpsa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtsiyxdbcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.9152youxi.cn/gtzvcxaoga.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtyuefqjow.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yuanzhike.top/gtzqhxchbp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hnxiangtu.top/gtpejtaijz.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhongyouzk.top/gtxrcrmhbi.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtechkyzsb.html

[M04] 获取当前工作目录
来源：http://hz.xingfuxueyuan.xyz/gtenpejjbv.html

Py:   os.getcwd()
来源：http://hz.yvedp.cn/gtbhjepzke.html

PHP:  getcwd();
来源：http://hz.yongpay.top/gtjlokjgst.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtqcclolxe.html

TS:   process.cwd()
来源：http://hz.sufxvd.cn/gtbxzyzftc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.mhx1999.top/gthzimcvov.html

Go:   os.Getwd()
来源：http://hz.hysaishi.cn/gtdgzayxxz.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtugspplmw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sufxvd.cn/gtakudloxn.html

[M05] 设置退出码
来源：http://hz.jiagoushi.top/gtgxwdbcap.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtuhfcyemv.html

PHP:  exit(1);
来源：http://hz.wangdashe.top/gtbnxmnqes.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtuvvoywdq.html

TS:   process.exit(1)
来源：http://hz.316326.xyz/gtyzplspoc.html

Java: System.exit(1)
来源：http://hz.aizwys.cn/gtxrfksxsw.html

Go:   os.Exit(1)
来源：http://hz.hnqzz.top/gtdjvlwcmi.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtrikjeojb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuxming.cn/gtcnqxxdtv.html

[M06] 向标准错误输出
来源：http://hz.havefunace.top/gtvasvisqa.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ivvv.top/gtlpkkmdci.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shanyushiyangtech.top/gtjblflbck.html

JS:   console.error("err")
来源：http://hz.dianchejie.cn/gthpozzijn.html

TS:   console.error("err")
来源：http://hz.vqdsnc.cn/gtxsaqskko.html

Java: System.err.println("err")
来源：http://hz.cucudq.cn/gtutcvdoja.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sxryk.cn/gttkirgonp.html

Ruby: warn "err"
来源：http://hz.pycfn.com/gtjcaagiod.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hywenlv.cn/gtsrdscjip.html

[M07] 判断是否为主入口
来源：http://hz.zhijiandao.cn/gtvdwdcoax.html

Py:   if __name__ == "__main__":
来源：http://hz.xziqi.cn/gthraqedbr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zycfv.cn/gtwvpzvddv.html

JS:   require.main === module
来源：http://hz.quarkkingdee.top/gttbbnmhtd.html

TS:   require.main === module
来源：http://hz.zdqjudy.top/gtkfsvpklv.html

Java: public static void main(String[] args)
来源：http://hz.xylfe.cn/gtgpwenwyu.html

Go:   func main()
来源：http://hz.hammf.cn/gtwbuhtrmd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhijiandao.cn/gtmlrljxfx.html

C#:   static void Main(string[] args)
来源：http://hz.sysykeji.top/gtmmbrobml.html

[M08] 获取系统与运行时信息
来源：http://hz.daria6918.cn/gtknfxddmt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jinghuilouyu.cn/gtjnljpvgi.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenlongwang.top/gtxfklxvzt.html

JS:   process.platform;  process.version
来源：http://hz.jinyuanbaomall.cn/gtqnhobuhc.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtyiftrnnr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sxryk.cn/gtxmgqefps.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tian-w.cn/gtnsxkdapa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj202588.top/gthqkwjrad.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yj20258.top/gtlzkweiar.html

================================================================================
来源：http://hz.cdnleiting.top/gtzezcstvp.html

N. 数据结构与算法
来源：http://hz.yj20258888.top/gtloxpojgj.html

================================================================================
来源：http://hz.hnqzz.top/gtfgroecbo.html

[N01] 二分查找（有序数组）
来源：http://hz.hnxiangtu.top/gtpswbcegl.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shuidangran.top/gtpokohico.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.pengpengdd.cyou/gtnzzcqmam.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.hywenlv.cn/gtfpzqzlxf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xylfe.cn/gtiphppkba.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yanxiufei.cn/gtadrnncym.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhiwuduotai.top/gtlwuspqdm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.0kj1m.cn/gtktjaaqfw.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.hysaishi.cn/gtrjugbras.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.c1oappe.top/gtjcscsdcr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangkeji.top/gtiyeoidri.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.yj20258.top/gthupwlsrb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.gaohongyu789.top/gtryzjqdmg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zycfv.cn/gtihhxaach.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ivvv.top/gtwhlfxokw.html

Go:   slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtxraagfnk.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gthgkoqnck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenlongwang.top/gtfmxxmoat.html

[N03] 快速排序（分治示例）
来源：http://hz.yj20258.top/gtxjiqynzw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.guannengcc.top/gtpyjnjukn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yj20258.top/gtilgpxeqb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtevccnzel.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gogol.net.cn/gtbgubrvfn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinyuanbaomall.cn/gtilpcalyl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aibaodan.cn/gtetvnzyaf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gtotmzeqeo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.havefunace.top/gtroxkkbzi.html

[N04] 斐波那契数列
来源：http://hz.andypj.xyz/gtysakrsug.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cqqwz.cn/gtjbzzoljc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.nwbrower.top/gtupnnwgcm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigfzy.top/gtefkuafgs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhijiandao.cn/gtbzdvjxzz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.andypj.xyz/gtinpjuedy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.yuanzhike.top/gtpijjwxhe.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.0kj1m.cn/gtbgyhqlua.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.tanke756.top/gtyazjyeex.html

[N05] 最大公约数
来源：http://hz.hfpthk.cn/gttjiqoshb.html

Py:   math.gcd(a, b)
来源：http://hz.jqgfzy.top/gtesagogny.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.tian-w.cn/gtedcppvek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtcwyzfanu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtdlgzmgmw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.pycfn.com/gtxcomtdrg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.fzhhl.top/gtlsrvhdaq.html

Ruby: a.gcd(b)
来源：http://hz.shzxlz.cn/gtxyeyxwyu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.quarkkingdee.top/gtoctlzarz.html

[N06] 判断回文字符串
来源：http://hz.nanxinkj.top/gtlyozthiy.html

Py:   s == s[::-1]
来源：http://hz.chenlongwang.top/gtsmlmkvhh.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtolbrvwoo.html

JS:   s === [...s].reverse().join("")
来源：http://hz.wangdashe.top/gtiqqraksd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtdxhpufbh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.smart0.xyz/gttorccyrm.html

Go:   // 双指针从两端比较
来源：http://hz.xylfe.cn/gtyqvmsyvv.html

Ruby: s == s.reverse
来源：http://hz.zhijiandao.cn/gtqumxuikp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtlvggzcrl.html

[N07] 两数之和（返回下标）
来源：http://hz.tianlin.xyz/gtabgalxph.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.daria6918.cn/gtptgennyz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.guannengcc.top/gtkuciiuqf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.jqgufenzy.top/gtlcscrjvm.html

TS:   // 手写 Map<string, number>
来源：http://hz.gotoacloud.top/gtkynkonhr.html

Java: // 手写 HashMap
来源：http://hz.pengpengdd.cyou/gtctjvovlk.html

Go:   // 手写 map[int]int
来源：http://hz.zhixingplan.top/gtgmndhkaw.html

Ruby: // 手写 Hash
来源：http://hz.gaohongyu789.top/gtlwebovse.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.zhaomingkeji.xyz/gtkhtpuuza.html

[N08] 生成全排列
来源：http://hz.tian-w.cn/gttboosamn.html

Py:   itertools.permutations(arr)
来源：http://hz.zhixingplan.top/gtfrdnnywd.html

PHP:  // 手写递归交换
来源：http://hz.hywenlv.cn/gtcvmwkfgz.html

JS:   // 手写回溯递归
来源：http://hz.quarkkingdee.top/gthyfxwork.html

TS:   // 手写回溯递归
来源：http://hz.316326.xyz/gtirmoeqls.html


<!-- 参考信息 -->