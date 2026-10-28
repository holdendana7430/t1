代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtsoehtfft.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ybcxt.top/gtsccmmmrx.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtswpexsjq.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtvdeztrdj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhijiandao.cn/gtpaahergo.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtamcxqhvy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gtcscsmevo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtbevpvxup.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigfzy.top/gtnxycqnyv.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtcmnhqjdv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtqhimunpk.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtncbyugoo.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtdympkrjy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtwhgkstze.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtidmfkwew.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtzzstqyxs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtbuhsomat.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtrcrgffbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtlxrqhgzf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtwmpngzjb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtibelrvsm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtrczieelp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.pycfn.com/gtjijqutsb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtiqqtrfjj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cucudq.cn/gtcigdwxdy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtisbqaarr.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtvxtycpml.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.52xcode.cn/gtzwynxdad.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xingfuxueyuan.xyz/gtuddsbkjt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtqofwazdq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtaipvemki.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ivvv.top/gtlgxpppif.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtcakhaxvl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtzeeombaf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.havefunace.top/gtlbwefxhp.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtzgvhupou.html

Py:   copy.deepcopy(obj)
来源：http://hz.kuanghao11.cn/gtuxincctq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yonumen.top/gtoktphlmp.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtipfqntgj.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtzbmfgoyr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.dianchejie.cn/gtpzwkzhxn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hnqzz.top/gtefwvxkyi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cashguo.top/gtearybvzk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtmbozcxyf.html

[K06] 解析 URL 查询串
来源：http://hz.sweek.top/gtpskjgoox.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sysykeji.top/gtpyqurzba.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.havefunace.top/gtphywafyi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtsbmtpwvh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gthtakhxvv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtqhtyobrl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtodiuvswy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.c1oappe.top/gthxhehrmt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shangyingyoupin.top/gtcmdznkmy.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtrhmpjyoi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hnqzz.top/gtdloamjov.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtbajpndtl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtbexothwn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtunihzrmg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtbbroppuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtkfggodjz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gtbzkbdhlz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtwxsssklp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aibaodan.cn/gtkgfkkbad.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gttraajxop.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gthoyqkbfy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtfdzyeikz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtfquoumin.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtkdzetmpv.html

Go:   encoding/gob
来源：http://hz.jlsjyb.cn/gttkyzrglm.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtaymcwhhx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zdqjudy.top/gtoelxzcxl.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtysfhoxqg.html

L. 网络请求
来源：http://hz.cheryme.top/gtlsvkpgid.html

================================================================================
来源：http://hz.ppjwa.cn/gtelejrfgg.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtbasisnex.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.havefunace.top/gtoxhbjgjs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jinghuilouyu.cn/gtwouamuhl.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtofssnbeb.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtmxeeiiyv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hnxiangtu.top/gtuthmmxaj.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtroqbxkfm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtrssoinnm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.daria6918.cn/gtzlbbrcvj.html

[L02] 发送 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtoztsscmj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cheryme.top/gtmayescfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtbggmetnl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.aibaodan.cn/gthnyuxglo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dashuyun.cn/gtotamrgkr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydzc1.top/gtohzjyjiq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gtdiwsgpof.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxinkj.top/gtxiqvnjnc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fengsongda.top/gtumroetos.html

[L03] 设置自定义请求头
来源：http://hz.9152youxi.cn/gtjfvlcscl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cheryme.top/gtsixqpxsb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gterookxed.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.snrcjt.cn/gtdccpoetg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtuuhpxswt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.snrcjt.cn/gtyyacdsex.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtzblzekke.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtndzdrnby.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shzxlz.cn/gtgcthomwt.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtzqeughha.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxinkj.top/gtzzstyzsg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigufen.top/gtlsptpamy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yongpay.top/gthcnohzal.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sysykeji.top/gtrcskxmpo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtfvreaerx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ppjwa.cn/gtgipemuic.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtnhazzrrn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.quarkkingdee.top/gtjxcelkeu.html

[L05] 上传文件（multipart）
来源：http://hz.meibo888.top/gtzuuemtxt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gttpgduwlk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jiagoushi.top/gtjixrijhy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtjmbkdtnw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhengqikj.top/gtiznxgecv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jqgfzy.top/gtgoigqvhk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sxryk.cn/gtiltrejzw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtbmepgngc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhixingplan.top/gtxnnrvqlb.html

[L06] 解析响应为 JSON
来源：http://hz.hammf.cn/gtqkasjrmf.html

Py:   resp.json()
来源：http://hz.vqdsnc.cn/gtvqweqcex.html

PHP:  json_decode($body, true);
来源：http://hz.yueranfly.top/gtubgulwzv.html

JS:   await resp.json()
来源：http://hz.zycfv.cn/gtmzjndxue.html

TS:   await resp.json()
来源：http://hz.jinqigufen.top/gtjymwhmxt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtfvbwmikb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yvedp.cn/gthvncrfhw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangkeji.top/gtyxgvlsal.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgfzy.top/gtzqrovpwx.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gtwzyhfoij.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nanxuanxn.top/gtwvxnqtto.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guowangkeji.top/gtlkmerdho.html

JS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gthpsralcu.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtoeyriknx.html

Java: resp.statusCode()
来源：http://hz.jinyuanbaomall.cn/gtwpacaxbj.html

Go:   resp.StatusCode
来源：http://hz.cdnleiting.top/gtrucyprpi.html

Ruby: resp.code.to_i
来源：http://hz.cheryme.top/gtdeqkxgnu.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigufen.top/gtaugckfhy.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtfrkphhaz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shanyushiyangkeji.top/gttvbhwpyl.html

PHP:  curl_multi_init() 系列
来源：http://hz.ydjk.org.cn/gtbnqenbkv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hysaishi.cn/gtzdlgjrvm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.316326.xyz/gtazppvbce.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hfpthk.cn/gtbvgmeper.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.haohaochexian.top/gtqdebinvi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinqigufen.top/gtewvlowzl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhixingplan.top/gtfdjajwue.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxxexuerp.html

M. 命令行 / 进程 / 环境
来源：http://hz.yueranfly.top/gtbiwxqzri.html

================================================================================
来源：http://hz.jlsjyb.cn/gtakintems.html

[M01] 读取命令行参数
来源：http://hz.fzhhl.top/gtlihcljhp.html

Py:   sys.argv[1:]
来源：http://hz.dashuyun.cn/gtiafezhnu.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtedsjyrsj.html

JS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtatgpspwm.html

TS:   process.argv.slice(2)
来源：http://hz.snrcjt.cn/gtcavcctbn.html

Java: args 数组（main 方法参数）
来源：http://hz.ivvv.top/gtxuwvalsb.html

Go:   os.Args[1:]
来源：http://hz.zhijiandao.cn/gtoqanlhvc.html

Ruby: ARGV
来源：http://hz.ybcxt.top/gtgusqnczm.html

C#:   args 数组（Main 方法参数）
来源：http://hz.9152youxi.cn/gtyazstsci.html

[M02] 读取环境变量
来源：http://hz.ppjwa.cn/gtivtnbyik.html

Py:   os.environ.get("HOME")
来源：http://hz.daxiang520.top/gtsbxbhljo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yonumen.top/gtzytgftvi.html

JS:   process.env.HOME
来源：http://hz.shzxlz.cn/gtmrfdeehy.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtuyivbsaq.html

Java: System.getenv("HOME")
来源：http://hz.meibo888.top/gtovvlgxak.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.zhengqikj.top/gtsifqhfrh.html

Ruby: ENV["HOME"]
来源：http://hz.aizwys.cn/gtjsxtlusp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.xinyue.icu/gttgmwfeed.html

[M03] 执行外部命令
来源：http://hz.c1oappe.top/gtzcmrsgqj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.iojbl.cn/gtjbqqeyiw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtksjhlhxo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ivvv.top/gtqlvvrplc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangkeji.top/gtsmgmskgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gzhubu.top/gtezemjwjy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.shangyingyoupin.top/gtitlnjunq.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ehwqpu.com/gtsukeyoqj.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ehwqpu.com/gthreudvag.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtweolkiyt.html

Py:   os.getcwd()
来源：http://hz.tian-w.cn/gtwlcgqccg.html

PHP:  getcwd();
来源：http://hz.havefunace.top/gtddimvhap.html

JS:   process.cwd()
来源：http://hz.zdqjudy.top/gtfiwupylz.html

TS:   process.cwd()
来源：http://hz.yvedp.cn/gtnwzecumm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenjidiqi.icu/gtzozzpwny.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gtwbdqoqjm.html

Ruby: Dir.pwd
来源：http://hz.cucudq.cn/gtdnyzoldw.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.xuetiantiany.cn/gtigsxpbth.html

[M05] 设置退出码
来源：http://hz.daxiang520.top/gtpfhrwvyq.html

Py:   sys.exit(1)
来源：http://hz.meibo888.top/gtuhteoqrj.html

PHP:  exit(1);
来源：http://hz.jinyuanbaomall.cn/gtqfwfxjgz.html

JS:   process.exit(1)
来源：http://hz.ehwqpu.com/gtuibedzxn.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtfwilyjgr.html

Java: System.exit(1)
来源：http://hz.nanxuanxn.top/gtedqnhszx.html

Go:   os.Exit(1)
来源：http://hz.zhongyouzk.top/gtttlwzeru.html

Ruby: exit 1
来源：http://hz.nwbrower.top/gtosfrmhec.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.quarkkingdee.top/gtpfnjdrvv.html

[M06] 向标准错误输出
来源：http://hz.smart0.xyz/gtcghsipoj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yvedp.cn/gtwdlagloj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.gogol.net.cn/gthefgxdnk.html

JS:   console.error("err")
来源：http://hz.yuxming.cn/gtmtzxjklw.html

TS:   console.error("err")
来源：http://hz.zhoulong.xyz/gtbpcbhjbp.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtiowgndnd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shuidangran.top/gtvbhepyud.html

Ruby: warn "err"
来源：http://hz.jiagoushi.top/gthejsxpqu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hongshengwenyu.top/gtgvxovdmz.html

[M07] 判断是否为主入口
来源：http://hz.yj20258.top/gtfnxxpowu.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtkiwkvwaf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.snrcjt.cn/gtmsirhoie.html

JS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtlcwugomo.html

TS:   require.main === module
来源：http://hz.chenjidiqi.icu/gtxjckriky.html

Java: public static void main(String[] args)
来源：http://hz.hnxiangtu.top/gtzahhprxf.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtientquph.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.chenzaomai.com/gtkqfrhiao.html

C#:   static void Main(string[] args)
来源：http://hz.yj20258.top/gtuxpznqvn.html

[M08] 获取系统与运行时信息
来源：http://hz.haohaochexian.top/gtpqgctmxe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydjk.org.cn/gtbkckknji.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gtpsnuitfh.html

JS:   process.platform;  process.version
来源：http://hz.sweek.top/gtmvtxcuyw.html

TS:   process.platform;  process.version
来源：http://hz.jinqigfzy.top/gtzbofhlio.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtoeojdedj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ydjk.org.cn/gtucojgmyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.ivvv.top/gtvyguxnfp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtfsghnnwi.html

================================================================================
来源：http://hz.zhengqikj.top/gtxyvxqwhh.html

N. 数据结构与算法
来源：http://hz.gzhubu.top/gtfaayefab.html

================================================================================
来源：http://hz.guannengcc.top/gtpvrzgmhq.html

[N01] 二分查找（有序数组）
来源：http://hz.fengsongda.top/gtbnerdkiz.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.feifeiyinyue.top/gtbzeqxuvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.hysaishi.cn/gtnjpzpmjw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenjidiqi.icu/gtrkaeacwi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.shangyingyoupin.top/gttocgnnlq.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.yj202588.top/gtbkkwrxsn.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.bjfxy.top/gtfqkjhjpm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.guannengcc.top/gtafvfdxtc.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtjwjfeupf.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.dianchejie.cn/gtnncktgsw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenlongwang.top/gtpybjhoro.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.nanxinkj.top/gtjtghjpwo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtpezmqswe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.yuanzhike.top/gtkenzprzy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtjkvbcpqh.html

Go:   slices.Sort(arr)
来源：http://hz.shangyingyoupin.top/gttievhwxh.html

Ruby: arr.sort
来源：http://hz.feifeiyinyue.top/gtfwbtchgk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.wangdashe.top/gtvtbhnvja.html

[N03] 快速排序（分治示例）
来源：http://hz.ydzc1.top/gtssfwtclt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.yangfankeji.com/gtifrmvalm.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shangyingyoupin.top/gthkivpnvh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.zdqjudy.top/gtzkhklgqa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtfehalqhh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.shangyingyoupin.top/gtlplflvqc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jlsjyb.cn/gtjomqhppq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.ybcxt.top/gthxwosggo.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.hnxiangtu.top/gtmybgqwht.html

[N04] 斐波那契数列
来源：http://hz.yanxiufei.cn/gtmjssmuaz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.sxryk.cn/gtytcndqyw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.fzhhl.top/gtnbogxsqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.haohaochexian.top/gtdsltkntr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhengqikj.top/gtprxdazyx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.haohaochexian.top/gtgeogwdwx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.ppjwa.cn/gttqbjwfif.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.wangshuangyany.cn/gtdrjewfas.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.fzhhl.top/gtqnwiunsz.html

[N05] 最大公约数
来源：http://hz.ppjwa.cn/gtxakkahhs.html

Py:   math.gcd(a, b)
来源：http://hz.chenjidiqi.icu/gtdaumhael.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.nwbrower.top/gtnhnweika.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cheryme.top/gtibfhvqow.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.316326.xyz/gtdkjwlyyx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.iojbl.cn/gtnpybimvd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.zhaomingkeji.xyz/gthscmirii.html

Ruby: a.gcd(b)
来源：http://hz.smart0.xyz/gtvnfmlzrl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.yanxiufei.cn/gtczgsnafs.html

[N06] 判断回文字符串
来源：http://hz.daxiang520.top/gtfbzxmubu.html

Py:   s == s[::-1]
来源：http://hz.daxiang520.top/gtgqrwbtdz.html

PHP:  $s === strrev($s);
来源：http://hz.haohaochexian.top/gtymixlsjh.html

JS:   s === [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtfbdjrmjs.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtpqtrtemu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.sufxvd.cn/gtxhkiqsst.html

Go:   // 双指针从两端比较
来源：http://hz.zhoulong.xyz/gteyoyyqwd.html

Ruby: s == s.reverse
来源：http://hz.nanxinkj.top/gtjrqrmxxa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.bjfxy.top/gtvpwxprwr.html

[N07] 两数之和（返回下标）
来源：http://hz.zhijiandao.cn/gtnqyiodpk.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.shuidangran.top/gtsttiylvz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gzhubu.top/gttwwfpich.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.shzxlz.cn/gtnxgjgmwc.html

TS:   // 手写 Map<string, number>
来源：http://hz.jqgufenzy.top/gtfwywvcsh.html

Java: // 手写 HashMap
来源：http://hz.daria6918.cn/gthqrxhztf.html

Go:   // 手写 map[int]int
来源：http://hz.hnxiangtu.top/gtsawzrgia.html

Ruby: // 手写 Hash
来源：http://hz.chenjidiqi.icu/gtyvtqales.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.xuanzx.com/gtbadpluow.html

[N08] 生成全排列
来源：http://hz.wangdashe.top/gtooylmtsh.html

Py:   itertools.permutations(arr)
来源：http://hz.iojbl.cn/gtniixxupn.html

PHP:  // 手写递归交换
来源：http://hz.zhengqikj.top/gtbgcdbtum.html

JS:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gtcvanpfww.html

TS:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtxgyihvmy.html

Java: // 手写回溯递归
来源：http://hz.9152youxi.cn/gtffyqszli.html

Go:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtmyuiahmw.html

Ruby: arr.permutation.to_a
来源：http://hz.zhixingplan.top/gtyamgjjtq.html

C#:   // 手写回溯递归
来源：http://hz.c1oappe.top/gtosusiisg.html

[N09] 栈与队列
来源：http://hz.yuxming.cn/gtmgeadgth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.tanke756.top/gttterpajf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.svipenyu.cn/gtourjqryg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.yueranfly.top/gtdrrxzvyy.html


<!-- 参考信息 -->