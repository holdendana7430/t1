代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtkcgsdsbs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.snrcjt.cn/gtvzcvzpiy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtdegxvvhy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtmzhqvcaw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtclqmlwpu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtnczamdlv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gttgrcedyp.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtraqtoyle.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xinyue.icu/gtrwuelnwy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtlopmkhrq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gtefkamaua.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.feifeiyinyue.top/gtnycslomu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gotoacloud.top/gttreqonkr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtvvfvhijt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtctcaotkf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtewjgipig.html

================================================================================
来源：http://hz.havefunace.top/gtsmrfmxky.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtqnsevonr.html

================================================================================
来源：http://hz.redwolf501.top/gtabrdjtsb.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtbacvwwbd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtpbxfbddt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gthowkattg.html

JS:   JSON.stringify(obj)
来源：http://hz.zhaomingkeji.xyz/gtjdhsajzs.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gththarxvf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xingfuxueyuan.xyz/gtpjxkvihs.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtdvkgttxp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuanzx.com/gtpquvyjqo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtoncqarfg.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtmryomdgk.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtqmpmvzza.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtxbyhapeq.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtnbrfjlrk.html

TS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtqqcodtbl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ehwqpu.com/gtmjcutcuf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtlmxgncqk.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtqboxtldl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gttqybhtlg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xziqi.cn/gtggnrqnzv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xylfe.cn/gtjwtcuyvu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtbzpqjivp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gthgvlrsyi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtcihdrhqn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtukrcvnoz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtradqvocm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenzaomai.com/gtipjfqozi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtexhnonpt.html

[K04] 读取 JSON 文件
来源：http://hz.yangfankeji.com/gtxqkxjpom.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhijiandao.cn/gtezwbvvom.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shuidangran.top/gtfmmezuei.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aizwys.cn/gtcoadfbfs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtpmayfzdg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nwbrower.top/gtnyxdpbkg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtagcyefow.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtigcfwbph.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtounptulv.html

[K05] 深拷贝对象
来源：http://hz.haohaochexian.top/gtoqindlts.html

Py:   copy.deepcopy(obj)
来源：http://hz.xziqi.cn/gtnsslnxfh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shzxlz.cn/gtfyldgrbi.html

JS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtpsigrtfc.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtlwgngdth.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtkgsnmije.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtvfjnczbg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tianlin.xyz/gteetwcgny.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gthtebupte.html

[K06] 解析 URL 查询串
来源：http://hz.cheryme.top/gtcflwyddk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtjlphjmxd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtmvvqcufw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtrovunsun.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fzhhl.top/gtlhjeutze.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinqigufen.top/gtzkwempyj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.smart0.xyz/gtcwtkzjcf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtoemxfjzw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtgkcdwaim.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtgsupkjat.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtktkivocw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtpfzedpan.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtpiaomwbq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtdyirfznp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtskqhvmjr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtiwnltqus.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.c1oappe.top/gtwoupuagz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ppjwa.cn/gtbeabjixg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gtrrgczjbr.html

Py:   pickle.dumps(obj)
来源：http://hz.cqqwz.cn/gtmuuqpvhr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuanzx.com/gtookoflec.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gtbcchzcqk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gtlwxhyiek.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhijiandao.cn/gtqxkkrdvt.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtfixfizvr.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtiqdoqymy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtneneicoo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttzwabuby.html

L. 网络请求
来源：http://hz.yj202588.top/gttawtvnau.html

================================================================================
来源：http://hz.yonumen.top/gtlcuaxbtr.html

[L01] 发送 GET 请求
来源：http://hz.jyoumei.cn/gtelfzzzzu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnxiangtu.top/gtxczukhaa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.meibo888.top/gtvotkranv.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtedqjknif.html

TS:   await fetch(url)
来源：http://hz.smart0.xyz/gtvnfbxxfr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtlusyancs.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtonmablmp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hnqzz.top/gtbhxhgnrg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.316326.xyz/gtcxiusile.html

[L02] 发送 POST JSON
来源：http://hz.daria6918.cn/gtxhkjfrot.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtlotcjydr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.quarkkingdee.top/gtucjuvupj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydzc1.top/gtfeqxjvxt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtgrnuzvzw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtvjrdhfjk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yj202588.top/gtulbfqpzh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jinyuanbaomall.cn/gtlgzrzrtw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gtciqgezde.html

[L03] 设置自定义请求头
来源：http://hz.chenjidiqi.icu/gtqyeucnsp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhijiandao.cn/gtexltpzfh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gttuajqong.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.bjfxy.top/gtlbzzlibp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.aizwys.cn/gtfvbhiirg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cdnleiting.top/gteanzassl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenzaomai.com/gtigeehmch.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.feifeiyinyue.top/gtdtooxkej.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtpyvqnwxm.html

[L04] 设置超时
来源：http://hz.havefunace.top/gtnbnuyqjn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shangyingyoupin.top/gtgetqlssj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.redwolf501.top/gtroqncqfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gtosoarcvt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtzixolgto.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.dashuyun.cn/gtyjemngsi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtnffkxbli.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtcyugedxi.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtlpclqsmq.html

[L05] 上传文件（multipart）
来源：http://hz.hongshengwenyu.top/gtyurzmsoy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guannengcc.top/gtopsahbiy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.svipenyu.cn/gtgwdubegw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gthupmyias.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgfzy.top/gtxljcuzuz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtggtpylaz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.quarkkingdee.top/gtzimslxjx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.guowangkeji.top/gtjlqobnbc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtfrimqxbd.html

[L06] 解析响应为 JSON
来源：http://hz.zhijiandao.cn/gtjymefidk.html

Py:   resp.json()
来源：http://hz.gotoacloud.top/gtpcjzbvlc.html

PHP:  json_decode($body, true);
来源：http://hz.jiagoushi.top/gtcimwhjxq.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtdevinoqp.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtaveudfvi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pycfn.com/gtzvxssbty.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangshuangyany.cn/gtbmmctsqs.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xingfuxueyuan.xyz/gttbkxuxre.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.meibo888.top/gtxkvkjyjp.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinqigufen.top/gtuawfdcrv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.redwolf501.top/gtvuoxjyqq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.svipenyu.cn/gtuwsmgaze.html

JS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtvhzeakdl.html

TS:   resp.ok;  resp.status
来源：http://hz.cucudq.cn/gteioatbjx.html

Java: resp.statusCode()
来源：http://hz.shangyingyoupin.top/gtjmykrvps.html

Go:   resp.StatusCode
来源：http://hz.yanxiufei.cn/gtbykkhymn.html

Ruby: resp.code.to_i
来源：http://hz.tianlin.xyz/gtzudydvkb.html

C#:   (int)resp.StatusCode
来源：http://hz.gaohongyu789.top/gthdjkoiqi.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtdeftaovr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.yonumen.top/gtxlfzngqr.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtornbertp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtsabnkate.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258888.top/gtavjuwepp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhixingplan.top/gtjcmpflua.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yangfankeji.com/gtabcvltqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.mhx1999.top/gtmnldnibp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtjqtzgius.html

================================================================================
来源：http://hz.0kj1m.cn/gthacgtyui.html

M. 命令行 / 进程 / 环境
来源：http://hz.chenjidiqi.icu/gtvdkgbvqs.html

================================================================================
来源：http://hz.yj20258888.top/gtsnsqztbg.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gturmrkhyh.html

Py:   sys.argv[1:]
来源：http://hz.hysaishi.cn/gtdedwjzee.html

PHP:  $argv;  $argc;
来源：http://hz.yj20258.top/gtjqxpckfp.html

JS:   process.argv.slice(2)
来源：http://hz.vqdsnc.cn/gthumowyhn.html

TS:   process.argv.slice(2)
来源：http://hz.chenzaomai.com/gtnppkbxos.html

Java: args 数组（main 方法参数）
来源：http://hz.ywan-chungtsiang.top/gtwvbwydmy.html

Go:   os.Args[1:]
来源：http://hz.hammf.cn/gtibeqvlqf.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtteyukpwu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhaomingkeji.xyz/gtmxxiyjyh.html

[M02] 读取环境变量
来源：http://hz.zhoulong.xyz/gtfimonvwd.html

Py:   os.environ.get("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtukhhnmll.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.quarkkingdee.top/gtxjjwdchw.html

JS:   process.env.HOME
来源：http://hz.gaohongyu789.top/gtxvyyjrfl.html

TS:   process.env.HOME
来源：http://hz.birdmap.top/gtzmzbbyvg.html

Java: System.getenv("HOME")
来源：http://hz.zhixingplan.top/gtvsmkavxj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.vqdsnc.cn/gtvcssgtdu.html

Ruby: ENV["HOME"]
来源：http://hz.ywan-chungtsiang.top/gtqlvjjuhn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xziqi.cn/gtrdzabjdh.html

[M03] 执行外部命令
来源：http://hz.shzxlz.cn/gthvgmiell.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuxming.cn/gtlsadkwlm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtdysrnrxv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtsyxtzbar.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gtazvruyxp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jyoumei.cn/gtwckqmmmf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.chenjidiqi.icu/gtgubtyldu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xylfe.cn/gtwxghugus.html

C#:   Process.Start("ls", "-l");
来源：http://hz.bjfxy.top/gtdzlykrpp.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gttaotawtp.html

Py:   os.getcwd()
来源：http://hz.daria6918.cn/gtgitjzwgv.html

PHP:  getcwd();
来源：http://hz.shzxlz.cn/gtbewmajnt.html

JS:   process.cwd()
来源：http://hz.ppjwa.cn/gtyljrnlro.html

TS:   process.cwd()
来源：http://hz.cqqwz.cn/gtahjamvpv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xziqi.cn/gtubomlaii.html

Go:   os.Getwd()
来源：http://hz.gotoacloud.top/gticdrtlrn.html

Ruby: Dir.pwd
来源：http://hz.hnqzz.top/gthfrriutb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yonumen.top/gtarjyuvue.html

[M05] 设置退出码
来源：http://hz.yj20258888.top/gtrvrrcjdo.html

Py:   sys.exit(1)
来源：http://hz.shuidangran.top/gtgiskiqwr.html

PHP:  exit(1);
来源：http://hz.zhaomingkeji.xyz/gtjibcdoce.html

JS:   process.exit(1)
来源：http://hz.yongpay.top/gtmfsaworq.html

TS:   process.exit(1)
来源：http://hz.xziqi.cn/gtfvoiihpm.html

Java: System.exit(1)
来源：http://hz.quarkkingdee.top/gtbighxprs.html

Go:   os.Exit(1)
来源：http://hz.nanxuanxn.top/gtrchqehce.html

Ruby: exit 1
来源：http://hz.meibo888.top/gtekqruolx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yj20258888.top/gtulhrlidt.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gttyvzmrfb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hysaishi.cn/gtrhiglkvm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.nwbrower.top/gtuilupdqc.html

JS:   console.error("err")
来源：http://hz.tanke756.top/gtkjdavgfm.html

TS:   console.error("err")
来源：http://hz.yj20258.top/gtbvfqenrp.html

Java: System.err.println("err")
来源：http://hz.tanke756.top/gtfflwzasq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guannengcc.top/gtcvilbxpx.html

Ruby: warn "err"
来源：http://hz.meibo888.top/gtoazxdfgv.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hnxiangtu.top/gtxqtbshwr.html

[M07] 判断是否为主入口
来源：http://hz.shzxlz.cn/gtvtotapul.html

Py:   if __name__ == "__main__":
来源：http://hz.andypj.xyz/gtdqgplwmq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shanyushiyangtech.top/gtigrtorep.html

JS:   require.main === module
来源：http://hz.gogol.net.cn/gtxmfcgjyz.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtvlxnqkcr.html

Java: public static void main(String[] args)
来源：http://hz.yj202588.top/gtxqoccpgf.html

Go:   func main()
来源：http://hz.shangyingyoupin.top/gtdranjsdf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ehwqpu.com/gtmfwqgark.html

C#:   static void Main(string[] args)
来源：http://hz.svipenyu.cn/gtgrunrcbc.html

[M08] 获取系统与运行时信息
来源：http://hz.hnxiangtu.top/gtlayccxhw.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtkptvlwdl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hongshengwenyu.top/gtzkbqrmbu.html

JS:   process.platform;  process.version
来源：http://hz.chenzaomai.com/gtyproegjx.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtmligovyh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.shanyushiyangkeji.top/gtxoswvrnu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.snrcjt.cn/gtkviblkqv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtaabpwkhr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.vqdsnc.cn/gtclqjybxk.html

================================================================================
来源：http://hz.shuidangran.top/gtppyoqvue.html

N. 数据结构与算法
来源：http://hz.guowangkeji.top/gtemrdbigu.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtrbhkoypl.html

[N01] 二分查找（有序数组）
来源：http://hz.ivvv.top/gtnxazmidd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtiyxwjjin.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.daxiang520.top/gtxcipemwx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jianghu66.top/gtjqasouky.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cucudq.cn/gtuemvrgtp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtklksqwxc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhaomingkeji.xyz/gttkavnjkr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.nwbrower.top/gtogycbnah.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.haohaochexian.top/gtcsilupui.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.9152youxi.cn/gtprbdmggd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtquzxbepd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.cheryme.top/gtvpceyvxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhixingplan.top/gtwdqqymjf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jyoumei.cn/gtbileokgs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.zhengqikj.top/gtgcqfljct.html

Go:   slices.Sort(arr)
来源：http://hz.c1oappe.top/gtryhvnbot.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtfejpyjiq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.xuetiantiany.cn/gtzejfxldb.html

[N03] 快速排序（分治示例）
来源：http://hz.xingfuxueyuan.xyz/gtchxfayre.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sxryk.cn/gtnkjcsozb.html

PHP:  // 递归实现，或用 usort
来源：http://hz.xylfe.cn/gtpoagcgbi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.svipenyu.cn/gtvmwstifk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.9152youxi.cn/gtelugqzhw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.aizwys.cn/gtzhdnrrkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhijiandao.cn/gtfsgtebet.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhengqikj.top/gtpmhdjjyv.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.nanxinkj.top/gtuzcoalxx.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gtemzysluw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sufxvd.cn/gtcenjnpbc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.tian-w.cn/gtniwgvfee.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.yj202588.top/gtogaedryz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gogol.net.cn/gtrqlmwhgu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.316326.xyz/gtmvlhtrtg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.xinyue.icu/gtxhkclzbz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zycfv.cn/gtnyrdcayh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.jiagoushi.top/gtjatebqrt.html

[N05] 最大公约数
来源：http://hz.fzhhl.top/gthljryxix.html

Py:   math.gcd(a, b)
来源：http://hz.fzhhl.top/gtnqrvrqok.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.shanyushiyangtech.top/gtsuikurrt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.sufxvd.cn/gtjxqoutfh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhixingplan.top/gtxhvajtuf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cqqwz.cn/gtkemtbkgi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.52xcode.cn/gthaionydn.html

Ruby: a.gcd(b)
来源：http://hz.zhongyouzk.top/gtptwjykow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jqgfzy.top/gteqgqpfhh.html

[N06] 判断回文字符串
来源：http://hz.wangshuangyany.cn/gtwmbhrqog.html

Py:   s == s[::-1]
来源：http://hz.guannengcc.top/gtzzpllsft.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtqclwgerh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtzxpoegxp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtjzsmugyu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.daxiang520.top/gtveuughcw.html

Go:   // 双指针从两端比较
来源：http://hz.fengsongda.top/gtwflietvr.html

Ruby: s == s.reverse
来源：http://hz.zhiwuduotai.top/gtjbrkadke.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtusdhqspy.html

[N07] 两数之和（返回下标）
来源：http://hz.ehwqpu.com/gtlhfomnzo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.jqgfzy.top/gtqwzpwnmi.html


<!-- 参考信息 -->