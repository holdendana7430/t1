代发 wailian999

================================================================================
来源：http://hz.jinqigfzy.top/gtivqshtbc.html

K. JSON 与序列化
来源：http://hz.snrcjt.cn/gtzddckhym.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvkpfcjlx.html

[K01] 对象转 JSON 字符串
来源：http://hz.gaohongyu789.top/gtwliyhcpn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtpmhzsorf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtsnhqjhsc.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtebapkoyq.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtmsfbuggm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zycfv.cn/gthabrldgv.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtjgdadsvb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ywan-chungtsiang.top/gticetjnrg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtriccegmw.html

[K02] JSON 字符串转对象
来源：http://hz.hfpthk.cn/gtlswfqoib.html

Py:   json.loads(s)
来源：http://hz.yj20258.top/gttulcjewp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gtpqivtrfe.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtglimhkik.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtzodvnmxw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gttkwdebbi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtjctgjwth.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtvpauzfjg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tianlin.xyz/gturolldux.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gtcfjcpiub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gttyuonmre.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtigbzewjd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtdglpzdpi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtwqyvuayq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pengpengdd.cyou/gthpumhzeh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhijiandao.cn/gthjlyuqwa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtunpkrswb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtyfjwyfxi.html

[K04] 读取 JSON 文件
来源：http://hz.316326.xyz/gtblejegok.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gteorxwrow.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pengpengdd.cyou/gtyxbqpaij.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtneckegns.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtbrpplcdo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sxryk.cn/gtnqqpjnrp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtblbjibdo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtynyoxpkq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtbxstsbhx.html

[K05] 深拷贝对象
来源：http://hz.tianlin.xyz/gtuwhasyyb.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtwhtgookq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtikyajhlm.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtzbppacwa.html

TS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtuyrnwajo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gtfxzcrxaj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.pycfn.com/gtcogxjbud.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtzswssywn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tianlin.xyz/gtipuxhozk.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtmjbprctc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtchliwyzs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtmtdoaujy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtvdxxxasc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gttezmsvzl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtekjfjjeo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aibaodan.cn/gtjwemydvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hfpthk.cn/gtsjbahpdo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtfizvdpdv.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gthyprudaj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gteerizcwv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtlrqvuock.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtivfhnawo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtodsvqbpt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtwczvgcnh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guowangkeji.top/gtuxtpclss.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtnilucddw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hfpthk.cn/gtdohhtzxm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daxiang520.top/gtjxfqaiaz.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtljssrohv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.birdmap.top/gtugywmfnl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtyxbpnuyr.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtnuraiyaa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtsbcowukm.html

Go:   encoding/gob
来源：http://hz.zhijiandao.cn/gtxethqnmu.html

Ruby: Marshal.dump(obj)
来源：http://hz.gaohongyu789.top/gttmvyzyuz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.iojbl.cn/gthjqzxepu.html

================================================================================
来源：http://hz.hywenlv.cn/gthelqrpnp.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtgbhsegmf.html

================================================================================
来源：http://hz.yj202588.top/gtmuiqqmzr.html

[L01] 发送 GET 请求
来源：http://hz.zycfv.cn/gtnvigcpfb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aizwys.cn/gtgmmlwrxm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ivvv.top/gtpcfcxmhz.html

JS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtbqpbdhax.html

TS:   await fetch(url)
来源：http://hz.daria6918.cn/gtaxhrhsqy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gtkudnipsk.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gthqkyliyo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gtipnkxczy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.havefunace.top/gtvxcucefr.html

[L02] 发送 POST JSON
来源：http://hz.chenlongwang.top/gtcdywbrrx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yangfankeji.com/gtucqbshla.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hnxiangtu.top/gtddekkwlf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtobkowpoh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtekopgnre.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtyoicywcv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhaomingkeji.xyz/gtgswwaluv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtrghvmbbx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtxyjmelio.html

[L03] 设置自定义请求头
来源：http://hz.yonumen.top/gtwdvruvmx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xylfe.cn/gtawtjxfak.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigufen.top/gttruduwlc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cucudq.cn/gtpbkyrqpf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.quarkkingdee.top/gttkdijbrm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shzxlz.cn/gtzfxbgmyh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hnqzz.top/gtalzzwavd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.dianchejie.cn/gtlkhuvgvr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ybcxt.top/gtawcdwbqe.html

[L04] 设置超时
来源：http://hz.daxiang520.top/gtmkpzrfvd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xziqi.cn/gthstrdshd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yonumen.top/gtrzmkzcsl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtmcahzaqc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gtfugerjfb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xziqi.cn/gtvuirjjlf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtsaqqraec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtilcdpzcq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.0kj1m.cn/gtfbpmlhva.html

[L05] 上传文件（multipart）
来源：http://hz.hnqzz.top/gtaramdgek.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangdashe.top/gtozxuhhob.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.wangdashe.top/gtbedewzrw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtkjyrnzlx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtouickxfl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.smart0.xyz/gtwkgrkujf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtdfacrvtm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xingfuxueyuan.xyz/gtbxhhjzkj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jlsjyb.cn/gtgqevmgya.html

[L06] 解析响应为 JSON
来源：http://hz.smart0.xyz/gtrsutvyes.html

Py:   resp.json()
来源：http://hz.haohaochexian.top/gtydsijbqo.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtjxxwsvqv.html

JS:   await resp.json()
来源：http://hz.pycfn.com/gtkvmhwjpu.html

TS:   await resp.json()
来源：http://hz.ydzc1.top/gtpeqsubqb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtiluzhetx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ehwqpu.com/gtrdukhizg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hfpthk.cn/gtkonnmwvn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.gaohongyu789.top/gtzjtnvvfm.html

[L07] 处理 HTTP 状态码
来源：http://hz.nwbrower.top/gtdvlngwhu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.dashuyun.cn/gtyzcefiix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtxydfdhzt.html

JS:   resp.ok;  resp.status
来源：http://hz.jlsjyb.cn/gtdfweqifz.html

TS:   resp.ok;  resp.status
来源：http://hz.ybcxt.top/gtngwyzwfm.html

Java: resp.statusCode()
来源：http://hz.yvedp.cn/gtbfwgcydz.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtzzgpfttk.html

Ruby: resp.code.to_i
来源：http://hz.gotoacloud.top/gthydexzya.html

C#:   (int)resp.StatusCode
来源：http://hz.jyoumei.cn/gtljfsxlur.html

[L08] 并发请求多个地址
来源：http://hz.ywan-chungtsiang.top/gtinphbcrn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenjidiqi.icu/gtewnqtqfv.html

PHP:  curl_multi_init() 系列
来源：http://hz.gaohongyu789.top/gtpeaujpvz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.shanyushiyangtech.top/gtivwyynyp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gotoacloud.top/gtvniwqnkn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jinyuanbaomall.cn/gtylbepity.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtasdqjzhr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yonumen.top/gtmbcixhpd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tian-w.cn/gtycuzouiv.html

================================================================================
来源：http://hz.ppjwa.cn/gtpowjpqvm.html

M. 命令行 / 进程 / 环境
来源：http://hz.52xcode.cn/gtwqrdnmro.html

================================================================================
来源：http://hz.xinyue.icu/gtytjlnoss.html

[M01] 读取命令行参数
来源：http://hz.cqqwz.cn/gtgtxdmfbc.html

Py:   sys.argv[1:]
来源：http://hz.nanxinkj.top/gtsayxeryl.html

PHP:  $argv;  $argc;
来源：http://hz.wangshuangyany.cn/gtevfplvwa.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtvsxjgtcz.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtzpnwcqbh.html

Java: args 数组（main 方法参数）
来源：http://hz.52xcode.cn/gtobnnvqty.html

Go:   os.Args[1:]
来源：http://hz.gotoacloud.top/gtsmdxfxjw.html

Ruby: ARGV
来源：http://hz.jinqigufen.top/gtgypsgfxk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.bjfxy.top/gtapcujdaw.html

[M02] 读取环境变量
来源：http://hz.svipenyu.cn/gtmvtdzgrs.html

Py:   os.environ.get("HOME")
来源：http://hz.fzhhl.top/gtfrdekdwe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.smart0.xyz/gtlswrioqa.html

JS:   process.env.HOME
来源：http://hz.ivvv.top/gtfglxxsct.html

TS:   process.env.HOME
来源：http://hz.kuanghao11.cn/gtowjassfx.html

Java: System.getenv("HOME")
来源：http://hz.ywan-chungtsiang.top/gteidfwagm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hammf.cn/gtqndnzhmr.html

Ruby: ENV["HOME"]
来源：http://hz.aibaodan.cn/gtbqgqnpgi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xingfuxueyuan.xyz/gtxefqazqr.html

[M03] 执行外部命令
来源：http://hz.nanxuanxn.top/gtswrzqens.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xuetiantiany.cn/gtiwzywfbz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtkwxqbrle.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhoulong.xyz/gtnkezlrkv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgufenzy.top/gthtadjlas.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gogol.net.cn/gtuqqdwxzb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.haohaochexian.top/gtimrowuae.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258.top/gtqiqnsves.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tian-w.cn/gtvlruurqr.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtbfsvyidv.html

Py:   os.getcwd()
来源：http://hz.shanyushiyangtech.top/gtobjwcccq.html

PHP:  getcwd();
来源：http://hz.yj202588.top/gtdxrsprnl.html

JS:   process.cwd()
来源：http://hz.cqqwz.cn/gtavztefiy.html

TS:   process.cwd()
来源：http://hz.fengsongda.top/gtwvkbofqs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.sxryk.cn/gtfjfsfemb.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtfylluojs.html

Ruby: Dir.pwd
来源：http://hz.cheryme.top/gthzlcqhcn.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ivvv.top/gtketeixjb.html

[M05] 设置退出码
来源：http://hz.redwolf501.top/gtmicnpyef.html

Py:   sys.exit(1)
来源：http://hz.iojbl.cn/gtjcjpqgyt.html

PHP:  exit(1);
来源：http://hz.hysaishi.cn/gtlcrrrswy.html

JS:   process.exit(1)
来源：http://hz.cqqwz.cn/gtqpjfraak.html

TS:   process.exit(1)
来源：http://hz.zhoulong.xyz/gtgdsnmusl.html

Java: System.exit(1)
来源：http://hz.cdnleiting.top/gtyzezvqlv.html

Go:   os.Exit(1)
来源：http://hz.aizwys.cn/gthlfebink.html

Ruby: exit 1
来源：http://hz.jlsjyb.cn/gtgmjlndtc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.andypj.xyz/gtkpnwfwjv.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtylcoditb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinyuanbaomall.cn/gtaduftezu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jlsjyb.cn/gtcyrnusqz.html

JS:   console.error("err")
来源：http://hz.bjfxy.top/gtmzwzrzho.html

TS:   console.error("err")
来源：http://hz.smart0.xyz/gtwtcsfqbh.html

Java: System.err.println("err")
来源：http://hz.zhengqikj.top/gtgeedsffr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gotoacloud.top/gtththfkxz.html

Ruby: warn "err"
来源：http://hz.yuanzhike.top/gtvsaogfvk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.birdmap.top/gtjdczmzgf.html

[M07] 判断是否为主入口
来源：http://hz.nanxuanxn.top/gtsrzdmyzl.html

Py:   if __name__ == "__main__":
来源：http://hz.gzhubu.top/gtpwuyoiam.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.vqdsnc.cn/gtwbjjqdnr.html

JS:   require.main === module
来源：http://hz.feifeiyinyue.top/gtkaymrplc.html

TS:   require.main === module
来源：http://hz.yuanzhike.top/gtowbsfbzi.html

Java: public static void main(String[] args)
来源：http://hz.hywenlv.cn/gtvxcvsdvv.html

Go:   func main()
来源：http://hz.aizwys.cn/gtiacsyhpq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zhoulong.xyz/gtwizmzhdq.html

C#:   static void Main(string[] args)
来源：http://hz.andypj.xyz/gtytymhsnu.html

[M08] 获取系统与运行时信息
来源：http://hz.yueranfly.top/gtjrrlpjst.html

Py:   platform.system();  platform.python_version()
来源：http://hz.haohaochexian.top/gtsmvlzvwk.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.daxiang520.top/gtxpavqldj.html

JS:   process.platform;  process.version
来源：http://hz.ppjwa.cn/gthwvhsqjl.html

TS:   process.platform;  process.version
来源：http://hz.jyoumei.cn/gtayianlnr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.kuanghao11.cn/gtewtbhyxe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.tanke756.top/gtvbykmbwy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.cucudq.cn/gtfgajvprp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.c1oappe.top/gtuqijozzl.html

================================================================================
来源：http://hz.dianchejie.cn/gtbwmnuvcw.html

N. 数据结构与算法
来源：http://hz.52xcode.cn/gtwbbtowgx.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkkexjbtc.html

[N01] 二分查找（有序数组）
来源：http://hz.yangfankeji.com/gtilwhzayn.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xuetiantiany.cn/gtrgafdmoi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.redwolf501.top/gtypkkrcwj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.ydzc1.top/gtflzniupy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sweek.top/gtyujallkq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.xziqi.cn/gtvpndtkcc.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.ivvv.top/gtwlhflccd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.meibo888.top/gtqdbgaotd.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jiagoushi.top/gtdkuvhonh.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.shuidangran.top/gtvxfcnmyc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tianlin.xyz/gthcvidkbb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.feifeiyinyue.top/gtchsgdqbh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jinghuilouyu.cn/gtbutyrlrj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hywenlv.cn/gtheualvxh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.quarkkingdee.top/gtksjsgqut.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtzxlpuirz.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtyhgwaoaj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.yangfankeji.com/gtfqtwtsij.html

[N03] 快速排序（分治示例）
来源：http://hz.dianchejie.cn/gthwbmfxdk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.jyoumei.cn/gttauoiahm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.jianghu66.top/gtnoezcjjg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtlmhoauug.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.nwbrower.top/gtgmvdvqzd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jyoumei.cn/gtpuylvpvw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.zhoulong.xyz/gteevvwinn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.guannengcc.top/gttppaemgn.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.chenjidiqi.icu/gtnknmkaau.html

[N04] 斐波那契数列
来源：http://hz.havefunace.top/gtbftiyjfi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtepdisidm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.ivvv.top/gtqxeglddz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.cashguo.top/gtphwxioly.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.dianchejie.cn/gtpxgioxeb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.chenlongwang.top/gtyoryaynl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhaomingkeji.xyz/gtkhozgflv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yj20258888.top/gtnhnnbbmn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.nanxinkj.top/gtioamhjqf.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtrpwlbdth.html

Py:   math.gcd(a, b)
来源：http://hz.meibo888.top/gtjuzpdaib.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jianghu66.top/gtzgfaudah.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.tian-w.cn/gtrrysijhs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtrdehyyie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtznfvcpgj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zycfv.cn/gtnsgqskns.html

Ruby: a.gcd(b)
来源：http://hz.52xcode.cn/gtpmzxtmwf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.feifeiyinyue.top/gtmukfzlzt.html

[N06] 判断回文字符串
来源：http://hz.quarkkingdee.top/gtleajszwp.html

Py:   s == s[::-1]
来源：http://hz.jqgfzy.top/gtglpmdikh.html

PHP:  $s === strrev($s);
来源：http://hz.yuxming.cn/gtucoczoem.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtrengqhcv.html

TS:   s === [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtgcebjqrh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.jqgufenzy.top/gthsycuglj.html

Go:   // 双指针从两端比较
来源：http://hz.yongpay.top/gtimxmfslf.html

Ruby: s == s.reverse
来源：http://hz.cqqwz.cn/gtouiihsnv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.pengpengdd.cyou/gtgtaljdyi.html

[N07] 两数之和（返回下标）
来源：http://hz.aibaodan.cn/gtrpqbiojj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.pycfn.com/gtmxjhjigw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenjidiqi.icu/gtgkehexrv.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.pengpengdd.cyou/gtjmqtfqpc.html

TS:   // 手写 Map<string, number>
来源：http://hz.cashguo.top/gttsevyjry.html

Java: // 手写 HashMap
来源：http://hz.ehwqpu.com/gtcejuqqbf.html

Go:   // 手写 map[int]int
来源：http://hz.shanyushiyangtech.top/gtoeqvskud.html

Ruby: // 手写 Hash
来源：http://hz.tianlin.xyz/gtfalztnph.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.fengsongda.top/gtthvnrhmo.html

[N08] 生成全排列
来源：http://hz.quarkkingdee.top/gtwlqtdkxn.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtwsupuiej.html

PHP:  // 手写递归交换
来源：http://hz.fzhhl.top/gtdttcxwcm.html

JS:   // 手写回溯递归
来源：http://hz.xuanzx.com/gtoknywynl.html

TS:   // 手写回溯递归
来源：http://hz.aizwys.cn/gtqwilgelk.html

Java: // 手写回溯递归
来源：http://hz.iojbl.cn/gtucpkqtvq.html

Go:   // 手写回溯递归
来源：http://hz.zhongyouzk.top/gtriyqdehk.html

Ruby: arr.permutation.to_a
来源：http://hz.pengpengdd.cyou/gtthxodarp.html

C#:   // 手写回溯递归
来源：http://hz.xuetiantiany.cn/gtwkwgmxxr.html


<!-- 参考信息 -->