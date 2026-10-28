代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtogoomize.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtanlgejrn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtjyqiykug.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tanke756.top/gtmdhyeigs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtfrwrqbhf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtflbbqxvt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jlsjyb.cn/gtluxeisnm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj202588.top/gtrmowatnl.html

================================================================================
来源：http://hz.yonumen.top/gtjkiavebl.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtidsfsmlx.html

================================================================================
来源：http://hz.hnqzz.top/gtaeycwecy.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuetiantiany.cn/gtzztdwpfc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yvedp.cn/gttnffrszp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtpffaciwt.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtcmjaasza.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gtidzssgay.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenjidiqi.icu/gtahcteadv.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtexbvkhrv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.meibo888.top/gtcrwbmlvx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shzxlz.cn/gtmgopksyc.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtxezghaxt.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangtech.top/gtucbudkjl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtwjjybals.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtywohbbtq.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtxggysdws.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtclgtmnmx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtjitroivr.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtqdaotxrv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhaomingkeji.xyz/gtigsqqwqt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtggqruoaa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtoedsidaf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtfpmzgsma.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtwwbxranh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtjzfnreok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtbbbnuznd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtihfbmvya.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guowangkeji.top/gtaeizxbuf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtgnryrpkx.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gttybzejha.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hfpthk.cn/gtaihuuqmb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtbhwyexxh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtzusyrydu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtjrovdnwg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hongshengwenyu.top/gtqmaeftsv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gthrdocgsf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydjk.org.cn/gtbeojonhi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgufenzy.top/gtutfjzkpj.html

[K05] 深拷贝对象
来源：http://hz.cucudq.cn/gtxuqfrkse.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtnmiisrnq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtvfegmdno.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtluoyjwiv.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtboyzlqvn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtcghwmase.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtttoxrvch.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gtzofezrct.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtgknxvyal.html

[K06] 解析 URL 查询串
来源：http://hz.yangfankeji.com/gtjnihhwcq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.52xcode.cn/gtzouvtlce.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.quarkkingdee.top/gtclqmdrqd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ybcxt.top/gtucbpdvhz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtpptklcal.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gthydqialz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtlmbqyovy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtjkmloonu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtmthnsreq.html

[K07] 进制转换
来源：http://hz.yanxiufei.cn/gtqccrtdio.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ivvv.top/gtbwxnvmoe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtugkemuiv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtgqaxvzgp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtclfximbu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258888.top/gtnspnvmxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pengpengdd.cyou/gttrpwovpb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtiuydsmeb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.quarkkingdee.top/gtkduxyvly.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.bjfxy.top/gtsbcanart.html

Py:   pickle.dumps(obj)
来源：http://hz.cqqwz.cn/gtcxyfpnie.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtnhpkrgfg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtmycsuogo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtkvlypqyv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.smart0.xyz/gtrycthrly.html

Go:   encoding/gob
来源：http://hz.wangshuangyany.cn/gtlcmctwif.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gtriuobpcs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aibaodan.cn/gtobrobgic.html

================================================================================
来源：http://hz.dashuyun.cn/gtbxrxknjy.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtsqmjcxnd.html

================================================================================
来源：http://hz.daria6918.cn/gtqlcwqnss.html

[L01] 发送 GET 请求
来源：http://hz.daxiang520.top/gtcepaquxv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.vqdsnc.cn/gtvpqxiwst.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.vqdsnc.cn/gthqjllopa.html

JS:   await fetch(url)
来源：http://hz.gzhubu.top/gtgsieawro.html

TS:   await fetch(url)
来源：http://hz.redwolf501.top/gtlskyljeb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.tanke756.top/gtusiqhifv.html

Go:   resp, err := http.Get(url)
来源：http://hz.gotoacloud.top/gtzesblnxn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xylfe.cn/gthjiodojb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtpxmuawan.html

[L02] 发送 POST JSON
来源：http://hz.hysaishi.cn/gtlxrvexpw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cqqwz.cn/gtbvtjgnon.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuxming.cn/gtkhbpmvqd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gtqbgqqsxo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cheryme.top/gtbvzodexw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.meibo888.top/gtsgggxcmg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cashguo.top/gtgvdfoarc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gttowwigic.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xinyue.icu/gteduiaqxe.html

[L03] 设置自定义请求头
来源：http://hz.meibo888.top/gtfhtmjwsc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.redwolf501.top/gtzxemxgzk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtrmcehcim.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtzpzvfwad.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ehwqpu.com/gtpedgpdxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.haohaochexian.top/gtzkpwaahe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtnehivpgs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gtwjzqrbdn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.smart0.xyz/gttgyfbasp.html

[L04] 设置超时
来源：http://hz.wangshuangyany.cn/gtkrzparhr.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shanyushiyangkeji.top/gtsvwytphv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aibaodan.cn/gtiytyrgfy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtbhtkfqxx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtxrtlkhxs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ehwqpu.com/gtmegomenf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.wangshuangyany.cn/gtprpkkxvr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tianlin.xyz/gtqiraibgz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zdqjudy.top/gtgewfvkmo.html

[L05] 上传文件（multipart）
来源：http://hz.shanyushiyangtech.top/gtuunjbbtz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhixingplan.top/gtlymklevr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pycfn.com/gtvraqktfo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtqbdjtsbd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yvedp.cn/gtwbecvkuj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yanxiufei.cn/gtcbqcpirj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.redwolf501.top/gtqkcdptsn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ydjk.org.cn/gtqgpnaete.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.aibaodan.cn/gtddlaoevr.html

[L06] 解析响应为 JSON
来源：http://hz.guowangkeji.top/gtnpgqcvvc.html

Py:   resp.json()
来源：http://hz.svipenyu.cn/gtipzwkvni.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtmxpdlrfq.html

JS:   await resp.json()
来源：http://hz.zdqjudy.top/gtfrysstzz.html

TS:   await resp.json()
来源：http://hz.sweek.top/gtxxuftzzf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtomnfhyqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtcdtjgcgi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.chenlongwang.top/gtaktcintb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.vqdsnc.cn/gtnfuupgxs.html

[L07] 处理 HTTP 状态码
来源：http://hz.svipenyu.cn/gtivjsylzk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.tian-w.cn/gtwpymiond.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtpztbzqzg.html

JS:   resp.ok;  resp.status
来源：http://hz.aibaodan.cn/gtsxnyybfo.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtgbqlplyc.html

Java: resp.statusCode()
来源：http://hz.yuanzhike.top/gtsyirkiyr.html

Go:   resp.StatusCode
来源：http://hz.jqgufenzy.top/gtsyijqbps.html

Ruby: resp.code.to_i
来源：http://hz.ppjwa.cn/gtpodkkjex.html

C#:   (int)resp.StatusCode
来源：http://hz.hywenlv.cn/gtdfsoypqe.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtmevjvpvb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.haohaochexian.top/gtolzjtyko.html

PHP:  curl_multi_init() 系列
来源：http://hz.cdnleiting.top/gtokhzesoc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.guannengcc.top/gtsibvspza.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtmeoemlat.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zycfv.cn/gtyjpukgpe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtjuuxqhjw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yongpay.top/gtdsjdhybl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinyuanbaomall.cn/gtzvbsspbw.html

================================================================================
来源：http://hz.redwolf501.top/gteielmmxv.html

M. 命令行 / 进程 / 环境
来源：http://hz.jqgufenzy.top/gtrnibrils.html

================================================================================
来源：http://hz.yj20258.top/gtjqyldjfx.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtrcfajvmr.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtmpllkepf.html

PHP:  $argv;  $argc;
来源：http://hz.kuanghao11.cn/gtwtonanwe.html

JS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtwbfqgfqa.html

TS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtvywvakjf.html

Java: args 数组（main 方法参数）
来源：http://hz.ybcxt.top/gtcnxnfnpq.html

Go:   os.Args[1:]
来源：http://hz.cucudq.cn/gthngdxuxy.html

Ruby: ARGV
来源：http://hz.ydzc1.top/gtajyesxqm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.snrcjt.cn/gtckupmotl.html

[M02] 读取环境变量
来源：http://hz.jqgufenzy.top/gtikcwbopm.html

Py:   os.environ.get("HOME")
来源：http://hz.zhixingplan.top/gtyaesklpp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.snrcjt.cn/gtonlzvqdx.html

JS:   process.env.HOME
来源：http://hz.yanxiufei.cn/gtknboygot.html

TS:   process.env.HOME
来源：http://hz.cashguo.top/gtskjbyxwe.html

Java: System.getenv("HOME")
来源：http://hz.guannengcc.top/gtglkbvlko.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtiwfvsydb.html

Ruby: ENV["HOME"]
来源：http://hz.feifeiyinyue.top/gtqcqzwnop.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtxlczlzru.html

[M03] 执行外部命令
来源：http://hz.andypj.xyz/gtbvjcogvp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtxbgczwad.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yongpay.top/gtifcirqwl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.meibo888.top/gthsxiserc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtthumesaz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.xinyue.icu/gtkatweguw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yj20258.top/gtwkeiztog.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.9152youxi.cn/gtvnlklnyp.html

C#:   Process.Start("ls", "-l");
来源：http://hz.sysykeji.top/gtrvuqxomt.html

[M04] 获取当前工作目录
来源：http://hz.52xcode.cn/gtsebkcanb.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gttnudmhec.html

PHP:  getcwd();
来源：http://hz.316326.xyz/gtuzgnlrsj.html

JS:   process.cwd()
来源：http://hz.hysaishi.cn/gtblxodhqa.html

TS:   process.cwd()
来源：http://hz.cucudq.cn/gtbojodlos.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinyuanbaomall.cn/gtrwmixesf.html

Go:   os.Getwd()
来源：http://hz.ywan-chungtsiang.top/gtmsbgefmw.html

Ruby: Dir.pwd
来源：http://hz.smart0.xyz/gtmmxrrntw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.pengpengdd.cyou/gtikutuyjp.html

[M05] 设置退出码
来源：http://hz.chenjidiqi.icu/gtvnnjmzhw.html

Py:   sys.exit(1)
来源：http://hz.yangfankeji.com/gtjqaoctiu.html

PHP:  exit(1);
来源：http://hz.tanke756.top/gtpjqrtxce.html

JS:   process.exit(1)
来源：http://hz.bjfxy.top/gtvqfaxphs.html

TS:   process.exit(1)
来源：http://hz.wangshuangyany.cn/gthwtpiehx.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gtgavxwctf.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtcsltdynp.html

Ruby: exit 1
来源：http://hz.jqgfzy.top/gtckjjjfxu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guowangkeji.top/gtnouarspe.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gttbhtuojm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cucudq.cn/gtehyaqmjn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj20258.top/gtnyzlzsgr.html

JS:   console.error("err")
来源：http://hz.316326.xyz/gtdswxtixw.html

TS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtqrzjdshw.html

Java: System.err.println("err")
来源：http://hz.yangfankeji.com/gtrubxnixn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.wangshuangyany.cn/gtymycjctu.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtczydhbpo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.cqqwz.cn/gtvxiwdlsp.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtzhvitgwn.html

Py:   if __name__ == "__main__":
来源：http://hz.hnqzz.top/gtwogqrxce.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gttphclrpz.html

JS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtfanqyvvp.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtfvshbtcn.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtzcqxntvv.html

Go:   func main()
来源：http://hz.52xcode.cn/gtpiuqptyh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xuanzx.com/gtuiiiqfwo.html

C#:   static void Main(string[] args)
来源：http://hz.yanxiufei.cn/gtmmodxucu.html

[M08] 获取系统与运行时信息
来源：http://hz.nwbrower.top/gtlynucjcz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.chenjidiqi.icu/gtvzkqtifl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ybcxt.top/gttugkozbp.html

JS:   process.platform;  process.version
来源：http://hz.yuanzhike.top/gtszveimiz.html

TS:   process.platform;  process.version
来源：http://hz.sweek.top/gtuwnwjqvs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhiwuduotai.top/gthdthsung.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gtpgqpryas.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.zhixingplan.top/gtvhihjssn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shanyushiyangkeji.top/gtmpnpzfqu.html

================================================================================
来源：http://hz.smart0.xyz/gtlzufxkha.html

N. 数据结构与算法
来源：http://hz.dianchejie.cn/gtqjppnmjb.html

================================================================================
来源：http://hz.gzhubu.top/gtvoedfpyx.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtxycwkrtg.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.andypj.xyz/gtlxuznwjo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.shzxlz.cn/gtwkepgtiq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.wangdashe.top/gtbnhnlmyr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.snrcjt.cn/gtljnsrovu.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinyuanbaomall.cn/gteunhcgcm.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hongshengwenyu.top/gtdgoepkxo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.smart0.xyz/gtsudccati.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.pengpengdd.cyou/gtypwvenva.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.svipenyu.cn/gtomxnpbiv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sysykeji.top/gtlotmhoch.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.jinqigufen.top/gtvzelagyz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yueranfly.top/gtavvriyht.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinqigfzy.top/gtkczgitlt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gttslapyfo.html

Go:   slices.Sort(arr)
来源：http://hz.daxiang520.top/gttardwksf.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtsbtledwq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.aizwys.cn/gtykhivmym.html

[N03] 快速排序（分治示例）
来源：http://hz.cucudq.cn/gtjnyludmq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jqgfzy.top/gtlenqupmn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gthditishq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.redwolf501.top/gtohtiuvgf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.havefunace.top/gtcfuykzgd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.ybcxt.top/gtnpxygkzh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhiwuduotai.top/gtxknngfqe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.shzxlz.cn/gtzvarlqcv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.zhengqikj.top/gthjfqrokd.html

[N04] 斐波那契数列
来源：http://hz.hysaishi.cn/gtnupjxqvv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.andypj.xyz/gtlrexlscp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.chenlongwang.top/gtbpzgnoeq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.hysaishi.cn/gthimoxsya.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.feifeiyinyue.top/gtpowcgdfj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jinyuanbaomall.cn/gtcpcbyktz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.havefunace.top/gthvqfbnya.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.hammf.cn/gtveofleqb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.zycfv.cn/gtcdssyqqr.html

[N05] 最大公约数
来源：http://hz.bjfxy.top/gthtigmkpl.html

Py:   math.gcd(a, b)
来源：http://hz.gotoacloud.top/gtteeceiow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinghuilouyu.cn/gtpogiafhq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.vqdsnc.cn/gtaxxbvvpi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.pycfn.com/gtknzbwgag.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.gogol.net.cn/gteggnpbsx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.ppjwa.cn/gtairazskv.html

Ruby: a.gcd(b)
来源：http://hz.tanke756.top/gtcqozxjig.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.gogol.net.cn/gtwgboikbd.html

[N06] 判断回文字符串
来源：http://hz.0kj1m.cn/gtqphvbwpy.html

Py:   s == s[::-1]
来源：http://hz.sysykeji.top/gtxlyrzjrc.html

PHP:  $s === strrev($s);
来源：http://hz.yonumen.top/gtbjgcqreh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gthxbwvnwz.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sweek.top/gtardjglpy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.ppjwa.cn/gtubyzjyoc.html

Go:   // 双指针从两端比较
来源：http://hz.daxiang520.top/gthuwhranu.html

Ruby: s == s.reverse
来源：http://hz.hnxiangtu.top/gtrvpweted.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtgfefcums.html

[N07] 两数之和（返回下标）
来源：http://hz.zhoulong.xyz/gtepscsgbh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.svipenyu.cn/gtntweqzff.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.hnqzz.top/gtkoducgyp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.havefunace.top/gtyyguhhsx.html

TS:   // 手写 Map<string, number>
来源：http://hz.yanxiufei.cn/gtqbznivwm.html

Java: // 手写 HashMap
来源：http://hz.ydjk.org.cn/gtevgspefh.html

Go:   // 手写 map[int]int
来源：http://hz.cashguo.top/gtnqengfra.html

Ruby: // 手写 Hash
来源：http://hz.wangdashe.top/gtinlwmrom.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yj20258888.top/gtuynvkbrd.html

[N08] 生成全排列
来源：http://hz.fzhhl.top/gtiecdwqqo.html


<!-- 参考信息 -->