代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gtarginvvk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtkvswtajb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jianghu66.top/gtcrvxyqcx.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtihusvyop.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtuuxaaker.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtidrmlbfv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtmcdjhmke.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtsckkxmir.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtruyggynk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtaogsporc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yongpay.top/gtnibhxgoe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jianghu66.top/gtcxunzlik.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuetiantiany.cn/gtguakgpym.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gttqcjxmfg.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtnulkkvrl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtodfjhgfh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuxming.cn/gtwgvyyujj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtgcwkomft.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtqbsnbhbe.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtortzfvgt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtkiuwyacf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtrabcoisj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gttxxttzoh.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtogkgbjge.html

Py:   copy.deepcopy(obj)
来源：http://hz.iojbl.cn/gtkbvqtevv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtdldkhiam.html

JS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtcixochqo.html

TS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtvhkrxdgh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhaomingkeji.xyz/gtpqiqzkma.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ivvv.top/gtgwrcicbb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtcrzfmxhu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.daria6918.cn/gturrspzsc.html

[K06] 解析 URL 查询串
来源：http://hz.gogol.net.cn/gtpedoutlf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gtbruflmya.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pycfn.com/gtpqxhsikz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtxkmhwdrl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtmsmsjemm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtyzifpzgy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenlongwang.top/gtngyiytxl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gthdsrakcw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtdkrijgwe.html

[K07] 进制转换
来源：http://hz.0kj1m.cn/gtavzwxtie.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtfmvgypwm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daxiang520.top/gtetqhuykk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtvkuxkbsc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtzbqsvped.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtrqmdflzs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtalqvzoju.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtvfjyscjj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtidtnedfo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guannengcc.top/gtcpzwrjxu.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgfzy.top/gtmjfsmzgp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cdnleiting.top/gtppsibxeg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtsnvpczcc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtbkpjsnnc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cdnleiting.top/gthetqsefq.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtlanknqaq.html

Ruby: Marshal.dump(obj)
来源：http://hz.daria6918.cn/gtzchzwttf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtkwcoeerh.html

================================================================================
来源：http://hz.xziqi.cn/gtnlawcdou.html

L. 网络请求
来源：http://hz.yueranfly.top/gtkguyojqu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttonhmsvn.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtfdlhwons.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jianghu66.top/gtgzbeacvf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gtwpplensj.html

JS:   await fetch(url)
来源：http://hz.hnqzz.top/gtzghzoxgg.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtkzriadkk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.havefunace.top/gtmcozwoad.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtuncmavgh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtprisgbvp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ywan-chungtsiang.top/gtpxiihpma.html

[L02] 发送 POST JSON
来源：http://hz.cashguo.top/gtbgkzgqrp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtvwctsbec.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gthuxlqrjb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtfbfkcpvo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtyxbipdgo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.52xcode.cn/gtazwiyhsr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hammf.cn/gtkgjblqms.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ppjwa.cn/gtmzvkmpwq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtdjiquoub.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtwdtechnb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.meibo888.top/gtvbimhkao.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtuwxtiznz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtjmjzchwl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtuthceiaf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtdwpsalqb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hywenlv.cn/gtyezmirse.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtfgowzqvt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtiyxqdsct.html

[L04] 设置超时
来源：http://hz.ivvv.top/gtmrvmaszi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.andypj.xyz/gtkbimhuce.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtqumtsyln.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hfpthk.cn/gtepcqstgp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.havefunace.top/gtzdnmmwnp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cheryme.top/gtdhhtxpeg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daria6918.cn/gtysllsvny.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgufenzy.top/gtdlpchaux.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xuetiantiany.cn/gtemmheake.html

[L05] 上传文件（multipart）
来源：http://hz.bjfxy.top/gtdobtrpho.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxuanxn.top/gtxywiamqo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.havefunace.top/gtlvoeomqn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hfpthk.cn/gtnjuhnddt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtslwtefpj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtlwetogmg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tian-w.cn/gttkixqyby.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhijiandao.cn/gtxktvvdbo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jiagoushi.top/gtnpohrjuq.html

[L06] 解析响应为 JSON
来源：http://hz.shuidangran.top/gtvfqmwpgb.html

Py:   resp.json()
来源：http://hz.fengsongda.top/gtrlumdwup.html

PHP:  json_decode($body, true);
来源：http://hz.0kj1m.cn/gtadyxloey.html

JS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtmcmgnovv.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtneiaaved.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtnyfcajnh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtyrkfzjdo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhixingplan.top/gtkrmmpfgl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtpqmwquzn.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtjueyedyw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.yanxiufei.cn/gtsskrpvcy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gttrtgxvro.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtqnqisyvd.html

TS:   resp.ok;  resp.status
来源：http://hz.xuanzx.com/gtwfzvjqqs.html

Java: resp.statusCode()
来源：http://hz.fengsongda.top/gtmckicvap.html

Go:   resp.StatusCode
来源：http://hz.shzxlz.cn/gtleordzrw.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtbfrwayns.html

C#:   (int)resp.StatusCode
来源：http://hz.jinqigfzy.top/gtawygdocr.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtltimtnzd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtfktlnpbm.html

PHP:  curl_multi_init() 系列
来源：http://hz.aizwys.cn/gtabaerkob.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtdxtivhdz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jiagoushi.top/gtpqpzzqvx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtzgjurrfg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.vqdsnc.cn/gtuognfnbr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yj20258888.top/gtyflhkfdr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.nwbrower.top/gthuffyzdx.html

================================================================================
来源：http://hz.sweek.top/gtmkukjggj.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuanzx.com/gttbofhdkb.html

================================================================================
来源：http://hz.havefunace.top/gtthvlmxjy.html

[M01] 读取命令行参数
来源：http://hz.hammf.cn/gtxtztayqn.html

Py:   sys.argv[1:]
来源：http://hz.xuanzx.com/gtrgunmvew.html

PHP:  $argv;  $argc;
来源：http://hz.wangdashe.top/gtcplvlpqd.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtsoljtfjn.html

TS:   process.argv.slice(2)
来源：http://hz.fengsongda.top/gtnyleshyy.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gtumrawmwm.html

Go:   os.Args[1:]
来源：http://hz.snrcjt.cn/gtllbnppzu.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtfccbppko.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtmfxuxjpa.html

[M02] 读取环境变量
来源：http://hz.hnxiangtu.top/gtsexabmwt.html

Py:   os.environ.get("HOME")
来源：http://hz.xuetiantiany.cn/gtagwealbe.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtqgmhgthw.html

JS:   process.env.HOME
来源：http://hz.jqgfzy.top/gtvcolndqu.html

TS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtiaxmvndz.html

Java: System.getenv("HOME")
来源：http://hz.ehwqpu.com/gtrvfojlwe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtozpdbhke.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtnvxhkhlr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cdnleiting.top/gtsuwlixzt.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtwgfcltxb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtuaqhjkfj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtmndqvbui.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gttzmrmonw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.chenlongwang.top/gtsyaszjpg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.shangyingyoupin.top/gtwmfgetcn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.zycfv.cn/gtipdgqfpk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuetiantiany.cn/gtezdzjvgu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.c1oappe.top/gtambqjvun.html

[M04] 获取当前工作目录
来源：http://hz.quarkkingdee.top/gtpfrxisnv.html

Py:   os.getcwd()
来源：http://hz.gogol.net.cn/gtmykdicvi.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtzsdizxob.html

JS:   process.cwd()
来源：http://hz.xylfe.cn/gtliqevbaq.html

TS:   process.cwd()
来源：http://hz.xziqi.cn/gtpgrmmjma.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hnqzz.top/gtjaqyrtez.html

Go:   os.Getwd()
来源：http://hz.hnqzz.top/gttozooejc.html

Ruby: Dir.pwd
来源：http://hz.haohaochexian.top/gtqbyhtrye.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.gotoacloud.top/gtzkvkqbvc.html

[M05] 设置退出码
来源：http://hz.hywenlv.cn/gtvzblqjnh.html

Py:   sys.exit(1)
来源：http://hz.tian-w.cn/gtgaipqgrm.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gtrmtpwyag.html

JS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gtovtuuixs.html

TS:   process.exit(1)
来源：http://hz.hnxiangtu.top/gttggsewbs.html

Java: System.exit(1)
来源：http://hz.jlsjyb.cn/gtjxennqmt.html

Go:   os.Exit(1)
来源：http://hz.cdnleiting.top/gtfglihmrr.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gtqhwpirzf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigfzy.top/gtefohppgr.html

[M06] 向标准错误输出
来源：http://hz.shanyushiyangtech.top/gtnqdozmva.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigufen.top/gtrqkeqkhl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gtwhovvyxh.html

JS:   console.error("err")
来源：http://hz.hywenlv.cn/gtertzfbcv.html

TS:   console.error("err")
来源：http://hz.316326.xyz/gtisganiyg.html

Java: System.err.println("err")
来源：http://hz.cheryme.top/gtomgkmzje.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.guowangkeji.top/gttbwmkxtx.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtlrpmpzjo.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.sysykeji.top/gtdbchroxy.html

[M07] 判断是否为主入口
来源：http://hz.ydjk.org.cn/gtyxutapmf.html

Py:   if __name__ == "__main__":
来源：http://hz.gotoacloud.top/gtmrlgfpjb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenzaomai.com/gtkdgslpwn.html

JS:   require.main === module
来源：http://hz.smart0.xyz/gtmxdmyscz.html

TS:   require.main === module
来源：http://hz.aizwys.cn/gtnylajnsg.html

Java: public static void main(String[] args)
来源：http://hz.cheryme.top/gttiwagtfw.html

Go:   func main()
来源：http://hz.jinqigfzy.top/gtyivsygls.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigfzy.top/gtxsjkmojr.html

C#:   static void Main(string[] args)
来源：http://hz.pengpengdd.cyou/gtggqyqjtt.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtxyrybbtu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtogtshoyl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.hywenlv.cn/gtuwmdbgye.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtrookbbms.html

TS:   process.platform;  process.version
来源：http://hz.meibo888.top/gtxzmomakt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.sufxvd.cn/gtdicpxrmx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.ehwqpu.com/gtxgobmzzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258.top/gtdczyazsb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yuanzhike.top/gtodyrpmmp.html

================================================================================
来源：http://hz.haohaochexian.top/gtjyuhbmaq.html

N. 数据结构与算法
来源：http://hz.xinyue.icu/gthskkgzvg.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtuwydnjtd.html

[N01] 二分查找（有序数组）
来源：http://hz.mhx1999.top/gtgxpjbabd.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.shzxlz.cn/gtqiualyie.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.cheryme.top/gtuhymqgla.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jinghuilouyu.cn/gtyaeziyah.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jyoumei.cn/gtswvoxmne.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.hnqzz.top/gtfwvaducz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.cqqwz.cn/gtqdebrqjf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhaomingkeji.xyz/gtxsrsgqbj.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.dianchejie.cn/gtkhmmjbrt.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.ivvv.top/gtpqgphfuk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtzkehvopx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.guannengcc.top/gtuncnbpds.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.cheryme.top/gtvefwpagj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nwbrower.top/gtucabcxcw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.sysykeji.top/gtxaoqekqe.html

Go:   slices.Sort(arr)
来源：http://hz.hnqzz.top/gtcsuawdxe.html

Ruby: arr.sort
来源：http://hz.xingfuxueyuan.xyz/gtyspyoxhm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dashuyun.cn/gtpfwnesft.html

[N03] 快速排序（分治示例）
来源：http://hz.chenlongwang.top/gtcriavhoh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.quarkkingdee.top/gtjcbmbhux.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtdrjdlwwc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.birdmap.top/gtkkarsoal.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tanke756.top/gtxyiegzhq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.daria6918.cn/gttbabbamt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.birdmap.top/gtmzqruvda.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.pycfn.com/gtcszuucuz.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sufxvd.cn/gtyjoysbpx.html

[N04] 斐波那契数列
来源：http://hz.nanxuanxn.top/gtoaapjagj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.cdnleiting.top/gtumilqcxb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.aibaodan.cn/gtqduwhohf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.ydjk.org.cn/gttlbpkakj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.pengpengdd.cyou/gtahsctmep.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.tian-w.cn/gtdpjzycmm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.zhixingplan.top/gtezbaxydl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.meibo888.top/gttddwoxls.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yvedp.cn/gttyjaaeld.html

[N05] 最大公约数
来源：http://hz.yj20258888.top/gthowqykgy.html

Py:   math.gcd(a, b)
来源：http://hz.cashguo.top/gttrxctadi.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.yj20258.top/gtegrnfabk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xylfe.cn/gtlaoqyfnl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.chenzaomai.com/gtmcppvohu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cucudq.cn/gtsrqrkmwl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.yvedp.cn/gtqtcpxugp.html

Ruby: a.gcd(b)
来源：http://hz.gaohongyu789.top/gtkjlpdpvo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhongyouzk.top/gtmklmlvyr.html

[N06] 判断回文字符串
来源：http://hz.hammf.cn/gtbnvqdkxh.html

Py:   s == s[::-1]
来源：http://hz.jlsjyb.cn/gtjageqrth.html

PHP:  $s === strrev($s);
来源：http://hz.52xcode.cn/gttgynpord.html

JS:   s === [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtxactjxwd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtqdrkxazo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.chenzaomai.com/gtaeobtqmm.html

Go:   // 双指针从两端比较
来源：http://hz.andypj.xyz/gtlmcfpdnu.html

Ruby: s == s.reverse
来源：http://hz.xuanzx.com/gtwxajuqld.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtpltgzyod.html

[N07] 两数之和（返回下标）
来源：http://hz.daxiang520.top/gtreqdoqjt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.0kj1m.cn/gtbrjhojez.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.yuanzhike.top/gtpbvuakum.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.0kj1m.cn/gtwvkruloy.html

TS:   // 手写 Map<string, number>
来源：http://hz.jinyuanbaomall.cn/gtgdvqwqqc.html

Java: // 手写 HashMap
来源：http://hz.jyoumei.cn/gtjdlrqqkx.html

Go:   // 手写 map[int]int
来源：http://hz.ydzc1.top/gtpelqgrrl.html

Ruby: // 手写 Hash
来源：http://hz.smart0.xyz/gtogsvrxab.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtyzvcyxdp.html

[N08] 生成全排列
来源：http://hz.havefunace.top/gtdbgfyyix.html

Py:   itertools.permutations(arr)
来源：http://hz.jinqigfzy.top/gtmkjujeet.html

PHP:  // 手写递归交换
来源：http://hz.xingfuxueyuan.xyz/gtfubqqrbk.html

JS:   // 手写回溯递归
来源：http://hz.andypj.xyz/gtsiukevcl.html

TS:   // 手写回溯递归
来源：http://hz.guowangkeji.top/gtamutowtl.html

Java: // 手写回溯递归
来源：http://hz.shuidangran.top/gtltkhfhro.html

Go:   // 手写回溯递归
来源：http://hz.jlsjyb.cn/gtrkqwtydq.html

Ruby: arr.permutation.to_a
来源：http://hz.cdnleiting.top/gtnogpnpkz.html

C#:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtqxhpwktj.html

[N09] 栈与队列
来源：http://hz.jinghuilouyu.cn/gtqtebrvwd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.yj202588.top/gtfndhmolm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.iojbl.cn/gtvtqbdjgj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.ydzc1.top/gttimyfzgk.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.daria6918.cn/gtetltmglz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hysaishi.cn/gtigefcdcv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zdqjudy.top/gtjrtyjscw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sysykeji.top/gtbbmluzda.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangtech.top/gtbwihxgth.html

[N10] 链表节点定义
来源：http://hz.shuidangran.top/gtktohdqqn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtfaooemas.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtmtbgybpj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.snrcjt.cn/gtnpzctlok.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.fzhhl.top/gtfvrrpopx.html

Java: class Node { int v; Node next; }
来源：http://hz.jyoumei.cn/gtuxlqsutc.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.ydjk.org.cn/gtkmcwfsoo.html


<!-- 参考信息 -->