代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xziqi.cn/gtiotzldja.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtxuualgyk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtacnhwhhj.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtdrqyqfxb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtfeoskojs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtyassticq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuetiantiany.cn/gtyfyxielh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtypnxjapx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tanke756.top/gtggnrcolg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtbviouqzu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtzzwzdotg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.feifeiyinyue.top/gttnrrxtwa.html

================================================================================
来源：http://hz.yj20258.top/gtnpodcwia.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gttphrradf.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtzbljjopt.html

[K01] 对象转 JSON 字符串
来源：http://hz.hywenlv.cn/gtyxcijwvr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtgcuvvenw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtfdjcathz.html

JS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtpfnyfcxl.html

TS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gttelvhurt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtmavoqnfr.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtjqzabgof.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yueranfly.top/gtsomkqizo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtiwnnrkst.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gthjyttmij.html

Py:   json.loads(s)
来源：http://hz.gogol.net.cn/gtjhfixcln.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtjnhxgucx.html

JS:   JSON.parse(s)
来源：http://hz.ydzc1.top/gtubakdnkj.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtydsogkxq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtfzbgvpes.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtsadplvtd.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtrbsmxrfx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gttukvodof.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtnspbjqfs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtaoevnaxs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtkcgawpuj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtjvqugvsg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtklqfmzvn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zdqjudy.top/gtatctvnek.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gtdmxgolsa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtettbzxjy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtncvbslnq.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gtmyazancq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gttbiltixq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtldusvyuk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hongshengwenyu.top/gtdtaeiixj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtmuopyowx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.kuanghao11.cn/gtkykfhnyo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtrzbnegnj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtzzrqxlbe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pengpengdd.cyou/gtonvjcmvs.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtaoqvdpdv.html

Py:   copy.deepcopy(obj)
来源：http://hz.xingfuxueyuan.xyz/gtsuenfdou.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtlobkjqxv.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtltffukur.html

TS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtkazcxaer.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yueranfly.top/gtzfowppoq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangtech.top/gtoclsbkms.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtrujufkxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtkooqrptv.html

[K06] 解析 URL 查询串
来源：http://hz.jqgfzy.top/gtmjqhpccz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhiwuduotai.top/gtmsgnfmcs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.haohaochexian.top/gtpfvakitv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtjyjpwooi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.smart0.xyz/gtqcjzoewz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhijiandao.cn/gtbdxjyuiw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fzhhl.top/gtpppfxhcc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtmvjwttbe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sysykeji.top/gtnpduoquv.html

[K07] 进制转换
来源：http://hz.hammf.cn/gtaloobxls.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ybcxt.top/gtsvqtfuzd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hysaishi.cn/gtdkxsycua.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gtdifxmxvl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtnwurcato.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtttmrlxsh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtonczooej.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtoymlxtth.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtxsjilwaa.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tanke756.top/gtsskldstm.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtsaxtfzsc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gtaizwcbwn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtwazyarxn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtgnetynlt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gtpbidsbww.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtzbowhpzu.html

Ruby: Marshal.dump(obj)
来源：http://hz.quarkkingdee.top/gtkullzika.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ppjwa.cn/gtdysvtwlb.html

================================================================================
来源：http://hz.jyoumei.cn/gtescnjydw.html

L. 网络请求
来源：http://hz.hysaishi.cn/gtgesmrfkz.html

================================================================================
来源：http://hz.aizwys.cn/gtycoyuqhd.html

[L01] 发送 GET 请求
来源：http://hz.ywan-chungtsiang.top/gtmcjnilgj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ivvv.top/gtoecdcqws.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cdnleiting.top/gtgdknastf.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtojtxhjin.html

TS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtzwuvnjwv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gzhubu.top/gtumozwhho.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuanzx.com/gthysrwslr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sufxvd.cn/gtuavolkkt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinqigufen.top/gtpmozvayd.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtxigkdphg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtddhyjudm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtpskqaqcr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtbasathfm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtuufyupsu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gttjujwiou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ehwqpu.com/gtdvmoxvce.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtmeccbpdl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.bjfxy.top/gtajipafrm.html

[L03] 设置自定义请求头
来源：http://hz.chenzaomai.com/gtyxpsrtau.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.bjfxy.top/gtxjybpcqt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.xinyue.icu/gtvbaezasa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtzubgwcuk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtuxbctiui.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.pycfn.com/gtgmqsexux.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtgjyjdiks.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.vqdsnc.cn/gtvosjzrxq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hammf.cn/gtpmdghluc.html

[L04] 设置超时
来源：http://hz.kuanghao11.cn/gtfsccbvhw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.pengpengdd.cyou/gtgjwfsohw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gttjtyfpuu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtzndpopdu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtuqtjyyjj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.smart0.xyz/gtdkyerodh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.fzhhl.top/gtgaadaykz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.guannengcc.top/gtseuslxiv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sufxvd.cn/gtjqjxbaij.html

[L05] 上传文件（multipart）
来源：http://hz.zhijiandao.cn/gtlpeesgzg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtajkipqnp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtbwjhsoov.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtvlbtzpgz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hammf.cn/gtxkiupmfy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gtqghcxars.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.haohaochexian.top/gtjluzjtdw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtshuenecb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtqppytfpi.html

[L06] 解析响应为 JSON
来源：http://hz.jianghu66.top/gtxdmhniyo.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtyumrgcke.html

PHP:  json_decode($body, true);
来源：http://hz.jqgfzy.top/gtudcjfloo.html

JS:   await resp.json()
来源：http://hz.0kj1m.cn/gthxjcmill.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtaxkeisox.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.shzxlz.cn/gtvodvzhdq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yj20258.top/gtoiyxynsr.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xuetiantiany.cn/gtblmnpieh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cdnleiting.top/gtduyxyxov.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gthlgbtcsz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhaomingkeji.xyz/gtptabkaea.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cashguo.top/gtytrsxfbv.html

JS:   resp.ok;  resp.status
来源：http://hz.iojbl.cn/gtngamyqdi.html

TS:   resp.ok;  resp.status
来源：http://hz.jqgufenzy.top/gtqeefvfxg.html

Java: resp.statusCode()
来源：http://hz.chenjidiqi.icu/gtjryzkmia.html

Go:   resp.StatusCode
来源：http://hz.0kj1m.cn/gtubmckvtm.html

Ruby: resp.code.to_i
来源：http://hz.sysykeji.top/gthjqcdqml.html

C#:   (int)resp.StatusCode
来源：http://hz.smart0.xyz/gtibvvlufy.html

[L08] 并发请求多个地址
来源：http://hz.yangfankeji.com/gtlhxhboel.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.snrcjt.cn/gtbbxcjjjv.html

PHP:  curl_multi_init() 系列
来源：http://hz.hysaishi.cn/gtwejwrksi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtabzsbzdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daria6918.cn/gterozjwve.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydzc1.top/gtrurepnau.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtxiliyuga.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.nwbrower.top/gtrbwschru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yangfankeji.com/gtwzmanjwk.html

================================================================================
来源：http://hz.c1oappe.top/gtmnhuneje.html

M. 命令行 / 进程 / 环境
来源：http://hz.jinqigufen.top/gtmcpvfrjy.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbpohuaar.html

[M01] 读取命令行参数
来源：http://hz.jinqigfzy.top/gtbbahepda.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtcksmfizi.html

PHP:  $argv;  $argc;
来源：http://hz.c1oappe.top/gtfxiaviin.html

JS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtuyiimkxu.html

TS:   process.argv.slice(2)
来源：http://hz.cdnleiting.top/gtmeecgrix.html

Java: args 数组（main 方法参数）
来源：http://hz.cashguo.top/gtmorpmmpf.html

Go:   os.Args[1:]
来源：http://hz.9152youxi.cn/gtavcxufhw.html

Ruby: ARGV
来源：http://hz.fzhhl.top/gtljfbleau.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sweek.top/gtnktgmmlg.html

[M02] 读取环境变量
来源：http://hz.yvedp.cn/gtondneuti.html

Py:   os.environ.get("HOME")
来源：http://hz.gotoacloud.top/gtagedclzt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.sweek.top/gtfytmufey.html

JS:   process.env.HOME
来源：http://hz.cqqwz.cn/gtritxahvt.html

TS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtimogrqkp.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtcwihzrke.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.cqqwz.cn/gtdxudsdct.html

Ruby: ENV["HOME"]
来源：http://hz.52xcode.cn/gtskncttmz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtgqyqqbol.html

[M03] 执行外部命令
来源：http://hz.mhx1999.top/gtlvuymjko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.meibo888.top/gtmimkgrct.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cqqwz.cn/gtcsltgqyl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtcwiihziu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.havefunace.top/gtwsxcdapx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.ywan-chungtsiang.top/gtfjmkeenw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.0kj1m.cn/gtsrvesbsi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.shanyushiyangtech.top/gtechmqprj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sxryk.cn/gtbobnomrl.html

[M04] 获取当前工作目录
来源：http://hz.jinyuanbaomall.cn/gtmlvsayjl.html

Py:   os.getcwd()
来源：http://hz.yongpay.top/gthnhbwzwr.html

PHP:  getcwd();
来源：http://hz.sxryk.cn/gtjijhljqh.html

JS:   process.cwd()
来源：http://hz.sufxvd.cn/gtvifincxf.html

TS:   process.cwd()
来源：http://hz.aibaodan.cn/gtknkvfsbm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.guowangkeji.top/gtuivctiuj.html

Go:   os.Getwd()
来源：http://hz.daria6918.cn/gthvepnlvv.html

Ruby: Dir.pwd
来源：http://hz.ivvv.top/gtnthijgoo.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.sxryk.cn/gtlgaupqbz.html

[M05] 设置退出码
来源：http://hz.jinyuanbaomall.cn/gthmaibcwz.html

Py:   sys.exit(1)
来源：http://hz.zdqjudy.top/gtlbrtkcwy.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtrooifybf.html

JS:   process.exit(1)
来源：http://hz.jiagoushi.top/gthsepptqz.html

TS:   process.exit(1)
来源：http://hz.xuanzx.com/gtfpqdqebu.html

Java: System.exit(1)
来源：http://hz.hywenlv.cn/gtfwkmyaqu.html

Go:   os.Exit(1)
来源：http://hz.smart0.xyz/gtmjogurrq.html

Ruby: exit 1
来源：http://hz.nanxinkj.top/gtqszdwuzp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtzulamnjw.html

[M06] 向标准错误输出
来源：http://hz.316326.xyz/gtoimcbpfg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.xuetiantiany.cn/gtaruczstg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtgtrddcek.html

JS:   console.error("err")
来源：http://hz.kuanghao11.cn/gtidkvkpnn.html

TS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtssytrhxr.html

Java: System.err.println("err")
来源：http://hz.hnxiangtu.top/gtyiifoenl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.sweek.top/gtoypatxon.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gtcexbpdre.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yj20258888.top/gtyiypwivg.html

[M07] 判断是否为主入口
来源：http://hz.jqgfzy.top/gtchqvbdnx.html

Py:   if __name__ == "__main__":
来源：http://hz.pycfn.com/gtdwgrfeyd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xingfuxueyuan.xyz/gtgmnprlhs.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtheykyhrt.html

TS:   require.main === module
来源：http://hz.xziqi.cn/gtmiceofdq.html

Java: public static void main(String[] args)
来源：http://hz.yj20258888.top/gtpelvrjnw.html

Go:   func main()
来源：http://hz.jianghu66.top/gtbdkhyybc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jlsjyb.cn/gtkggujdyd.html

C#:   static void Main(string[] args)
来源：http://hz.ybcxt.top/gtskfgqfdg.html

[M08] 获取系统与运行时信息
来源：http://hz.cheryme.top/gtebjntovs.html

Py:   platform.system();  platform.python_version()
来源：http://hz.daria6918.cn/gtbmsfczas.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.nanxuanxn.top/gtvoobrrje.html

JS:   process.platform;  process.version
来源：http://hz.316326.xyz/gteudjbodt.html

TS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtgjqkayjq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xuetiantiany.cn/gtiwlexcii.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.quarkkingdee.top/gtukcnfctb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtmjofrtwa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.hnqzz.top/gtsxsokgtk.html

================================================================================
来源：http://hz.fzhhl.top/gtoeafcooe.html

N. 数据结构与算法
来源：http://hz.wangshuangyany.cn/gtqujcyhdo.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpbmrpzkz.html

[N01] 二分查找（有序数组）
来源：http://hz.dashuyun.cn/gtovmwbvyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jlsjyb.cn/gtusdojimo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinghuilouyu.cn/gtthpbwnrk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhengqikj.top/gthmhljpcs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinqigfzy.top/gtaigoowkj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.havefunace.top/gtiidbxpvv.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gtbmcdcqav.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jinqigufen.top/gtrmziobza.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.yj202588.top/gtscrrbgjo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.zhengqikj.top/gtatlwrcnf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zycfv.cn/gttrvcnemt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.chenlongwang.top/gtfoyypdmp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.pengpengdd.cyou/gtuotfkred.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.shanyushiyangtech.top/gtqvszojsb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zdqjudy.top/gtzdqbqjoo.html

Go:   slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtvkqgguye.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtnfasykvs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sysykeji.top/gtjdvtnwgo.html

[N03] 快速排序（分治示例）
来源：http://hz.cheryme.top/gttoiavrgg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.bjfxy.top/gtbzfmgqbu.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhengqikj.top/gtplezmeyn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zhixingplan.top/gtvdbwngzw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtjjyjeyvl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.tianlin.xyz/gtfglndapi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cucudq.cn/gthbcpxlhi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.316326.xyz/gtderugajv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.tian-w.cn/gteutcubbx.html

[N04] 斐波那契数列
来源：http://hz.hnqzz.top/gtvomhbckw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.birdmap.top/gtjzhzprjd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.jinghuilouyu.cn/gtqemdwyyy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gttglkstkp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yanxiufei.cn/gtmhqucrqe.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenzaomai.com/gtymmmarlz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gtwkmejfhx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.quarkkingdee.top/gtmwejulaj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.svipenyu.cn/gtsgrosqyc.html

[N05] 最大公约数
来源：http://hz.jlsjyb.cn/gtbnvknlsc.html

Py:   math.gcd(a, b)
来源：http://hz.sufxvd.cn/gtebpxzibb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtdacikgin.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtwfdeefjc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jinghuilouyu.cn/gtlwqpcgoc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.daxiang520.top/gtrocqljuz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.hongshengwenyu.top/gteqkjeduv.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtrkrflpsp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.hnqzz.top/gtfcgnxdmp.html

[N06] 判断回文字符串
来源：http://hz.yj20258888.top/gtwzefuikd.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtjldtyxjy.html

PHP:  $s === strrev($s);
来源：http://hz.tianlin.xyz/gtzaqafray.html

JS:   s === [...s].reverse().join("")
来源：http://hz.yj202588.top/gtveedsorx.html

TS:   s === [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtzycvsxjb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sweek.top/gtslgeyrih.html

Go:   // 双指针从两端比较
来源：http://hz.yj20258888.top/gtdqxyuyvx.html

Ruby: s == s.reverse
来源：http://hz.birdmap.top/gtpmnmxdai.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtemxzcunc.html

[N07] 两数之和（返回下标）
来源：http://hz.hywenlv.cn/gtjrwjkesx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.nwbrower.top/gtjrcuhfay.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.dashuyun.cn/gtrbdkszyb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ehwqpu.com/gthgsfyotw.html

TS:   // 手写 Map<string, number>
来源：http://hz.snrcjt.cn/gtzctmfcsa.html

Java: // 手写 HashMap
来源：http://hz.quarkkingdee.top/gtdpwetxed.html


<!-- 参考信息 -->