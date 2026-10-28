代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtkqlxuvhk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tianlin.xyz/gtydbaxorz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtwnpelzyh.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtbgkllwzf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtrhmplrpd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtjhcoxove.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtdssrbsct.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtzsxcsmsi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtlezzecpu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtkzcruxdb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtgqwrrnkp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtcymwkwjl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtnphcrkix.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtbsvwaqdd.html

================================================================================
来源：http://hz.yuxming.cn/gtntvknedt.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gtumuyczox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gtfavcspjj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtlqvtposa.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtizohfkhk.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtqkreedol.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.meibo888.top/gtbauleuxs.html

Go:   json.Marshal(obj)
来源：http://hz.redwolf501.top/gtfokfsakw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtkuvmworv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtsaijwusu.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtuafyazgn.html

Py:   json.loads(s)
来源：http://hz.havefunace.top/gthyceakae.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jyoumei.cn/gtbxoexezm.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtdzndghra.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtfvrgruqe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtpuhjllyf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtnvroifak.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gtxuwfwaop.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.svipenyu.cn/gtopiywbus.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtyfpfwaww.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gthlpyqove.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sweek.top/gtlykifxjc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtfvgqdgcs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtkfqfgtrd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtojvvbyga.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtlsibiakb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtgtknfwgc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gtpmkcgsbt.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtnjhommyn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtwhaqfrku.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gthwgcetvb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gogol.net.cn/gtrouwpetz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtmjrkzvhq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtllizqmyq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtbvjdfnfm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtwpivejcp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aibaodan.cn/gtpcskfcno.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtjjkqshaz.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhoulong.xyz/gtcnsfnexw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtzjzdjftc.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtdxcviymp.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtcatbbula.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cashguo.top/gtfoomqitx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtphvxnblu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtdoebmisd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhoulong.xyz/gtwkxriyag.html

[K06] 解析 URL 查询串
来源：http://hz.bjfxy.top/gteyamlybm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtavojrlfz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gthupytmka.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtpmwhwqie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gtlzeshewx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gtbmkfskxy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtsdwyejec.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtclnudtwr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtnplvzjeq.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtcsodxlhb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gaohongyu789.top/gtfnbsuhgf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtzczjqbtr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtpkyzqcdj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtwqgbmszp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtygxirtva.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtrgpdwwvj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtunfmapem.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtpixixovr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtsjegsvjx.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtvqfsscey.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtyuzuxxja.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtvmubjqwv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtqtwpujwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cheryme.top/gtlzphytdp.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtirpauapa.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhixingplan.top/gtuzgrsvhv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtsxdubbhr.html

================================================================================
来源：http://hz.fzhhl.top/gtrzrmnpjj.html

L. 网络请求
来源：http://hz.mhx1999.top/gtnbhspnuh.html

================================================================================
来源：http://hz.ydzc1.top/gtxyfqdvlb.html

[L01] 发送 GET 请求
来源：http://hz.nanxuanxn.top/gtmeoamqdr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtnphvgcee.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtfhwibsnu.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtvbondrrr.html

TS:   await fetch(url)
来源：http://hz.yj20258.top/gtwbhgtahu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj202588.top/gtycaxatbt.html

Go:   resp, err := http.Get(url)
来源：http://hz.xylfe.cn/gtismdoxdt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj20258.top/gtonbdfqaw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgufenzy.top/gtkmnrkjrl.html

[L02] 发送 POST JSON
来源：http://hz.yuxming.cn/gtpbsfyccn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtirmieagq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtzdfoxfbu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtzimnssal.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cdnleiting.top/gtnpatervr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gtwztbbxeh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.birdmap.top/gttnugurcw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xylfe.cn/gtvpnewaff.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtjkogjszg.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtgxixcoqb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.birdmap.top/gtyxdnvirx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gttxzalvxs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtnyndjspz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gtxcuegmsg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ehwqpu.com/gtiismrevh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhengqikj.top/gtjdckvooh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtjdnmnvah.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtlnfcgrqd.html

[L04] 设置超时
来源：http://hz.zhengqikj.top/gtprzmoihl.html

Py:   requests.get(url, timeout=5)
来源：http://hz.dashuyun.cn/gtqbjbafou.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtcaunahac.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtgbdgpjmo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtxamjarqo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ivvv.top/gtczggnbmy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtxwpuxmkc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhongyouzk.top/gtwkzqgfuo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ybcxt.top/gtybkyqviu.html

[L05] 上传文件（multipart）
来源：http://hz.jinghuilouyu.cn/gtbsdqhsgi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtuihatfyu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtkozzpmak.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gttvxabspm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtjglzeany.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.chenjidiqi.icu/gtzukdzgcx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtfjzoewnd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtaqsaibin.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hfpthk.cn/gtkcsxwqol.html

[L06] 解析响应为 JSON
来源：http://hz.zhiwuduotai.top/gthxmkmogk.html

Py:   resp.json()
来源：http://hz.xziqi.cn/gtapsdwhet.html

PHP:  json_decode($body, true);
来源：http://hz.nwbrower.top/gtriylqchd.html

JS:   await resp.json()
来源：http://hz.yuanzhike.top/gtdbqqnrkh.html

TS:   await resp.json()
来源：http://hz.zhijiandao.cn/gteyjwdyhq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xylfe.cn/gtntjeckqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hnxiangtu.top/gtmwecmkjw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jinghuilouyu.cn/gtbfnpfcmp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.nwbrower.top/gtbvjpuzfv.html

[L07] 处理 HTTP 状态码
来源：http://hz.hfpthk.cn/gttbddzdjq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gttwsnygft.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.birdmap.top/gtfixdmsyd.html

JS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtutbmklts.html

TS:   resp.ok;  resp.status
来源：http://hz.tianlin.xyz/gtcvrreaof.html

Java: resp.statusCode()
来源：http://hz.mhx1999.top/gtkdvslfip.html

Go:   resp.StatusCode
来源：http://hz.gogol.net.cn/gtoimrrbwo.html

Ruby: resp.code.to_i
来源：http://hz.ehwqpu.com/gtmalanfui.html

C#:   (int)resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtpdhfahym.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtoycahkkb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zdqjudy.top/gtgurcckly.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtoupjpmxg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhaomingkeji.xyz/gtipmefgpz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yuxming.cn/gtzvydhhab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cucudq.cn/gtnhlfkblr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yueranfly.top/gtvpdmagng.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtwcdcsyau.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yanxiufei.cn/gtstjgkctj.html

================================================================================
来源：http://hz.iojbl.cn/gtqstasvyy.html

M. 命令行 / 进程 / 环境
来源：http://hz.jyoumei.cn/gtfzxyqzig.html

================================================================================
来源：http://hz.9152youxi.cn/gtorqmitma.html

[M01] 读取命令行参数
来源：http://hz.hnqzz.top/gtscgpmgru.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtywuxhljn.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtkiclvbmp.html

JS:   process.argv.slice(2)
来源：http://hz.zhengqikj.top/gtgebwnimf.html

TS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtajapgxkq.html

Java: args 数组（main 方法参数）
来源：http://hz.c1oappe.top/gtejfvyism.html

Go:   os.Args[1:]
来源：http://hz.jinqigfzy.top/gtygwmuryp.html

Ruby: ARGV
来源：http://hz.chenjidiqi.icu/gtmfjxfxft.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuetiantiany.cn/gtnbxeyqrl.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtihbiqghg.html

Py:   os.environ.get("HOME")
来源：http://hz.zhoulong.xyz/gtyffixzkj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtimultqcg.html

JS:   process.env.HOME
来源：http://hz.fengsongda.top/gtoykvtawt.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtohdyxrfw.html

Java: System.getenv("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtbopdhqwv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.xziqi.cn/gtghfjjsyb.html

Ruby: ENV["HOME"]
来源：http://hz.bjfxy.top/gtwejxowla.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shangyingyoupin.top/gtkdxwtilv.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtnfccmfmc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zdqjudy.top/gtyddnzocj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhongyouzk.top/gtwarprnkg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jianghu66.top/gtpzybpjxk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ehwqpu.com/gtqcqzmevn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtubgotwyc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.guowangkeji.top/gtbeznvqdg.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.mhx1999.top/gtghrluvfx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gtuqpfzdah.html

[M04] 获取当前工作目录
来源：http://hz.jinghuilouyu.cn/gtmhnjlzhs.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtgqspxuns.html

PHP:  getcwd();
来源：http://hz.ydjk.org.cn/gtpynywpmt.html

JS:   process.cwd()
来源：http://hz.hywenlv.cn/gtcvkscltn.html

TS:   process.cwd()
来源：http://hz.jqgfzy.top/gtxybfluhg.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.yanxiufei.cn/gtkanhzkiy.html

Go:   os.Getwd()
来源：http://hz.zhaomingkeji.xyz/gtjpzcmopg.html

Ruby: Dir.pwd
来源：http://hz.yvedp.cn/gtcrmopvhn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.dianchejie.cn/gtakpbnfij.html

[M05] 设置退出码
来源：http://hz.sxryk.cn/gttmrteueu.html

Py:   sys.exit(1)
来源：http://hz.jyoumei.cn/gtrmmgwzja.html

PHP:  exit(1);
来源：http://hz.chenzaomai.com/gtjzvciokk.html

JS:   process.exit(1)
来源：http://hz.yj20258888.top/gtpvjjwlvh.html

TS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtkwrsvnmh.html

Java: System.exit(1)
来源：http://hz.pycfn.com/gtjikebpgv.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtmqytcbcq.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtvccqxfhg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtsdvawhjl.html

[M06] 向标准错误输出
来源：http://hz.aizwys.cn/gtxcxxdzey.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yuanzhike.top/gtpsepalmv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.fengsongda.top/gtvbdtojic.html

JS:   console.error("err")
来源：http://hz.nwbrower.top/gtubaazwcm.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtrioxdvog.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtnahwqsfw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhongyouzk.top/gtzvffbhlm.html

Ruby: warn "err"
来源：http://hz.ivvv.top/gtlpqlaukz.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.daxiang520.top/gtujayboss.html

[M07] 判断是否为主入口
来源：http://hz.wangdashe.top/gtxcfsebdj.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtoasnrbpf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.zhoulong.xyz/gtbxaajygu.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gtmdropnxu.html

TS:   require.main === module
来源：http://hz.tianlin.xyz/gtnfhsdngu.html

Java: public static void main(String[] args)
来源：http://hz.haohaochexian.top/gtlxhxdxth.html

Go:   func main()
来源：http://hz.zhiwuduotai.top/gtvdunjjaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cdnleiting.top/gtssvtaztq.html

C#:   static void Main(string[] args)
来源：http://hz.zycfv.cn/gtkokezuck.html

[M08] 获取系统与运行时信息
来源：http://hz.meibo888.top/gthxdmzsqz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.havefunace.top/gtrroysvxg.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yangfankeji.com/gtkpdjhwli.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtdmwrhjcd.html

TS:   process.platform;  process.version
来源：http://hz.nwbrower.top/gtnevaiiba.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.52xcode.cn/gttmyaircv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cqqwz.cn/gtbmzcfedv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.gotoacloud.top/gthjatfdhw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.kuanghao11.cn/gtwzujxlnb.html

================================================================================
来源：http://hz.hnxiangtu.top/gtaptbanip.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtlwkfnmck.html

================================================================================
来源：http://hz.andypj.xyz/gtozkysnls.html

[N01] 二分查找（有序数组）
来源：http://hz.aibaodan.cn/gtnolzabxu.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtnrgolsbq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.meibo888.top/gtyaihnfuw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ybcxt.top/gtjajwjaab.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yvedp.cn/gtjvpdrevr.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.redwolf501.top/gtndhfxpny.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.gaohongyu789.top/gtqzdbojde.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.ivvv.top/gtvxlzlemd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.ivvv.top/gtwcxusfuc.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xuetiantiany.cn/gtswpydnzr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtulqdrsuo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtvxbkaflp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.svipenyu.cn/gtxguaonbj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtodszcztw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.dashuyun.cn/gtjcansair.html

Go:   slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtcrykyffw.html

Ruby: arr.sort
来源：http://hz.zhoulong.xyz/gthfxpzgis.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.ywan-chungtsiang.top/gtsgndrwei.html

[N03] 快速排序（分治示例）
来源：http://hz.ywan-chungtsiang.top/gtuqlnudaz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.xziqi.cn/gtfhmujcwy.html

PHP:  // 递归实现，或用 usort
来源：http://hz.hysaishi.cn/gtlcugowoz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shuidangran.top/gtonxyqyra.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shanyushiyangkeji.top/gtzogccrfh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yj20258.top/gtrzzubhgm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.hongshengwenyu.top/gtibajphim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cdnleiting.top/gtuttkuwho.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.ppjwa.cn/gtqabgtlus.html

[N04] 斐波那契数列
来源：http://hz.jinqigfzy.top/gtgqksoyuu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtbqpmfjnm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.havefunace.top/gtsjwgykkj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gotoacloud.top/gtjarqyejs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gzhubu.top/gtfzxscwcf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.hnxiangtu.top/gtnifbjlyu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.gotoacloud.top/gtxjogkbwt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.tanke756.top/gtcnkzzwja.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jinghuilouyu.cn/gtzlilfvyx.html

[N05] 最大公约数
来源：http://hz.zhiwuduotai.top/gtcaitxdew.html

Py:   math.gcd(a, b)
来源：http://hz.hongshengwenyu.top/gtacvevxkb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.svipenyu.cn/gtihrkmlbm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.shanyushiyangtech.top/gtbqyyortu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.hywenlv.cn/gtqncfwflj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.tianlin.xyz/gtbuppubue.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.pengpengdd.cyou/gtkyymgado.html

Ruby: a.gcd(b)
来源：http://hz.hnqzz.top/gtgjpicrfx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.aibaodan.cn/gtnbhvoxhq.html

[N06] 判断回文字符串
来源：http://hz.tian-w.cn/gtjeinslsr.html

Py:   s == s[::-1]
来源：http://hz.aibaodan.cn/gtizuvvxdz.html

PHP:  $s === strrev($s);
来源：http://hz.jyoumei.cn/gtinqxqcuk.html

JS:   s === [...s].reverse().join("")
来源：http://hz.52xcode.cn/gtbwnsicqq.html

TS:   s === [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtiqswqvoz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.kuanghao11.cn/gtbolgglpe.html

Go:   // 双指针从两端比较
来源：http://hz.dianchejie.cn/gtotcqdcyx.html

Ruby: s == s.reverse
来源：http://hz.mhx1999.top/gtslthhnkq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtowfryzgi.html

[N07] 两数之和（返回下标）
来源：http://hz.hammf.cn/gtfdosrebn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.xuetiantiany.cn/gteezcgutv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.aizwys.cn/gtforqeydm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.haohaochexian.top/gtkcgpozwt.html

TS:   // 手写 Map<string, number>
来源：http://hz.gaohongyu789.top/gtafizsvsn.html

Java: // 手写 HashMap
来源：http://hz.yj202588.top/gtamslkzeu.html


<!-- 参考信息 -->