代发 wailian999

[K02] JSON 字符串转对象
来源：http://hz.meibo888.top/gtpsorcete.html

Py:   json.loads(s)
来源：http://hz.zhixingplan.top/gtgfslxebn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtjahavksy.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtjjzuwfeb.html

TS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtlvsxiqyb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtxlelcljz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtqqqawqqb.html

Ruby: JSON.parse(s)
来源：http://hz.cashguo.top/gtetnzxcnx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhongyouzk.top/gtxdlydymf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtwitbcthf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtyuvkcejt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtvmqeafbp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtumvlxzgi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtfekpccpv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtlzgeakkc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yueranfly.top/gthlefmvwi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhiwuduotai.top/gtlataysab.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangkeji.top/gtvsjrrqlz.html

[K04] 读取 JSON 文件
来源：http://hz.jyoumei.cn/gteudoktaq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gttbzwpjcc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtrxprkdei.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtmmvcofwf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtiecsacnb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aizwys.cn/gtvvburnsy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gttgyodxkw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gaohongyu789.top/gtsucnwrww.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gaohongyu789.top/gtmsjbugkg.html

[K05] 深拷贝对象
来源：http://hz.sxryk.cn/gtnuhetwjv.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtjdgdpdbu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtxkjpanjv.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtqazxjpir.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gttepqxxsp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangtech.top/gtgjaihpsr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gtsdrytrbh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhaomingkeji.xyz/gtypqoovhr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtocajczpi.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gthwlcgfen.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhijiandao.cn/gtbwfulycv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtjrenrnmq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtujkkyzve.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtnaxpfjpj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gttliigsfr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtmwazkhps.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gtpmopvwln.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigufen.top/gtitxbnjft.html

[K07] 进制转换
来源：http://hz.yj202588.top/gtsqtlrmbh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtqgjjbcii.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtssblvouv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtnmlqytfh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtnkvmbotz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gttcukncor.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtatrtnepk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtkvdtbhit.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.havefunace.top/gtmkddnqvd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtuzpqqqhw.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtplbuvvpu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnqzz.top/gtlicczlcw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gttfhbqhsz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtponzlbxi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtipdtpvhn.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtgyckhwpl.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtgrzvqwuq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtxfawnyji.html

================================================================================
来源：http://hz.redwolf501.top/gtkyhmfbfv.html

L. 网络请求
来源：http://hz.bjfxy.top/gtyhurotoy.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyhjtyswm.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtlhvnbsty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtpwpfdkjv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yvedp.cn/gtamlkrzqx.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtxhinokrc.html

TS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtwefmbnxy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.chenlongwang.top/gtapapkrqs.html

Go:   resp, err := http.Get(url)
来源：http://hz.ydjk.org.cn/gtmgkoucia.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtlwqbyxwr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtjoeikizm.html

[L02] 发送 POST JSON
来源：http://hz.pengpengdd.cyou/gtstacqtzk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tianlin.xyz/gtrowojtye.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangdashe.top/gtklhgqauv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtwqapsmcg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yangfankeji.com/gtdimqznew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtagociruk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtggppqtck.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xuetiantiany.cn/gtyflwtqyo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.sxryk.cn/gtyxyqjxka.html

[L03] 设置自定义请求头
来源：http://hz.jiagoushi.top/gtxsqsfcah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtsmyxxqgt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtmiywiaaa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtkqbazbtx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtuwsclxhf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hywenlv.cn/gtxiwurowy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtuhvucdaa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cashguo.top/gtwhjtannl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.meibo888.top/gtfqexidof.html

[L04] 设置超时
来源：http://hz.yongpay.top/gtjmyhckpj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jlsjyb.cn/gtycapcppg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtjtibqzfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.svipenyu.cn/gtqecqjufq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gttuskaaxf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nanxinkj.top/gtsqaezgiz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sxryk.cn/gtjmfltmrd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinyuanbaomall.cn/gtczqinpgy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.9152youxi.cn/gtppgrpiey.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gtvfiqdekw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.gotoacloud.top/gtrlfckavm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hnxiangtu.top/gtosxifsum.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtimginoos.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.haohaochexian.top/gtvpnjrdxn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.gaohongyu789.top/gtkeetdedu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jyoumei.cn/gteqliqbba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shangyingyoupin.top/gtprarzxug.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hammf.cn/gtaicytpac.html

[L06] 解析响应为 JSON
来源：http://hz.jinghuilouyu.cn/gtkljmhemk.html

Py:   resp.json()
来源：http://hz.kuanghao11.cn/gtstpkutqf.html

PHP:  json_decode($body, true);
来源：http://hz.havefunace.top/gtczejizns.html

JS:   await resp.json()
来源：http://hz.yvedp.cn/gtikpdvqxv.html

TS:   await resp.json()
来源：http://hz.shuidangran.top/gtljxgeiop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xziqi.cn/gtymyqrjjo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtkmnusjhd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.fengsongda.top/gtrbkqdjdl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.aizwys.cn/gtzpxrwvdx.html

[L07] 处理 HTTP 状态码
来源：http://hz.hammf.cn/gtjcjkkfji.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtsiguzsfm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gttsnvembg.html

JS:   resp.ok;  resp.status
来源：http://hz.nwbrower.top/gtyzyuqesb.html

TS:   resp.ok;  resp.status
来源：http://hz.feifeiyinyue.top/gtsgoufbxt.html

Java: resp.statusCode()
来源：http://hz.xziqi.cn/gtsngzdrxs.html

Go:   resp.StatusCode
来源：http://hz.hysaishi.cn/gtegkvonnp.html

Ruby: resp.code.to_i
来源：http://hz.zdqjudy.top/gtdsabywjh.html

C#:   (int)resp.StatusCode
来源：http://hz.svipenyu.cn/gtsoelsrqd.html

[L08] 并发请求多个地址
来源：http://hz.cucudq.cn/gtegdzkldk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.iojbl.cn/gtztulwqle.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gthyjzpria.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtvbyethfu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.nwbrower.top/gtdfyshvyf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhiwuduotai.top/gtxxlahhti.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.gogol.net.cn/gtbqxukgas.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ydzc1.top/gtrerlmkih.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhoulong.xyz/gtwvyonkpr.html

================================================================================
来源：http://hz.zdqjudy.top/gtgxahnvzs.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtollzpswe.html

================================================================================
来源：http://hz.yj202588.top/gtofoejsit.html

[M01] 读取命令行参数
来源：http://hz.316326.xyz/gtmammzouy.html

Py:   sys.argv[1:]
来源：http://hz.yj202588.top/gtnbfpncpf.html

PHP:  $argv;  $argc;
来源：http://hz.ydjk.org.cn/gtttlsesyl.html

JS:   process.argv.slice(2)
来源：http://hz.yanxiufei.cn/gtibunlqhr.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtjmsfqyyf.html

Java: args 数组（main 方法参数）
来源：http://hz.nanxuanxn.top/gtetdbblbc.html

Go:   os.Args[1:]
来源：http://hz.ivvv.top/gtzrkdwwwq.html

Ruby: ARGV
来源：http://hz.yanxiufei.cn/gtchblgdio.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtzqvzzndh.html

[M02] 读取环境变量
来源：http://hz.guowangkeji.top/gtcjyjvjru.html

Py:   os.environ.get("HOME")
来源：http://hz.yuanzhike.top/gtoxzovitr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hnxiangtu.top/gtmtfsdcph.html

JS:   process.env.HOME
来源：http://hz.cashguo.top/gtinfblbye.html

TS:   process.env.HOME
来源：http://hz.yuxming.cn/gtpcacsaft.html

Java: System.getenv("HOME")
来源：http://hz.bjfxy.top/gtvhmxfwud.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.snrcjt.cn/gthfufxgou.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtowstdxwa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ydjk.org.cn/gthwflorre.html

[M03] 执行外部命令
来源：http://hz.gogol.net.cn/gtrcblrpvo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yj20258.top/gtohhcwvnq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.svipenyu.cn/gtafzgymyx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shzxlz.cn/gtqtkllvsg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xuetiantiany.cn/gtugplneep.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinqigfzy.top/gtoyapcjdw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuanzhike.top/gtenuwtjwe.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jinqigufen.top/gtvdbzzczn.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ppjwa.cn/gtorxlollq.html

[M04] 获取当前工作目录
来源：http://hz.yj20258888.top/gtzanmnmvv.html

Py:   os.getcwd()
来源：http://hz.ivvv.top/gtgtjhogao.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtvwblwnlw.html

JS:   process.cwd()
来源：http://hz.quarkkingdee.top/gtrmqrdvje.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gttyentfxk.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.havefunace.top/gtnslpjsah.html

Go:   os.Getwd()
来源：http://hz.52xcode.cn/gtiadmnbuz.html

Ruby: Dir.pwd
来源：http://hz.zhiwuduotai.top/gtazvcqeph.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.zhongyouzk.top/gtbgepbvjw.html

[M05] 设置退出码
来源：http://hz.sweek.top/gtksapisdd.html

Py:   sys.exit(1)
来源：http://hz.hfpthk.cn/gtwlkjdqsi.html

PHP:  exit(1);
来源：http://hz.zhijiandao.cn/gtdeztbhvm.html

JS:   process.exit(1)
来源：http://hz.52xcode.cn/gtjabptgfc.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtfiootszi.html

Java: System.exit(1)
来源：http://hz.jinqigfzy.top/gtwwntwbsn.html

Go:   os.Exit(1)
来源：http://hz.gaohongyu789.top/gtkwgtwuzr.html

Ruby: exit 1
来源：http://hz.sxryk.cn/gtwinbjopf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtawulioho.html

[M06] 向标准错误输出
来源：http://hz.yvedp.cn/gtifgvaufc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.sysykeji.top/gtibtngwme.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ywan-chungtsiang.top/gtkmyhmyij.html

JS:   console.error("err")
来源：http://hz.ydzc1.top/gtterrokfj.html

TS:   console.error("err")
来源：http://hz.hysaishi.cn/gtzwycfmtt.html

Java: System.err.println("err")
来源：http://hz.tian-w.cn/gtodzkoixg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jiagoushi.top/gtenhinulj.html

Ruby: warn "err"
来源：http://hz.fengsongda.top/gttqleqpjb.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ivvv.top/gtlxxurjao.html

[M07] 判断是否为主入口
来源：http://hz.tanke756.top/gtejgmipsm.html

Py:   if __name__ == "__main__":
来源：http://hz.ybcxt.top/gteadhigkx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtibtizopf.html

JS:   require.main === module
来源：http://hz.jiagoushi.top/gtrqcpgazr.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtgeqzxela.html

Java: public static void main(String[] args)
来源：http://hz.chenjidiqi.icu/gtgjlfqucn.html

Go:   func main()
来源：http://hz.chenzaomai.com/gthzteuswb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.guannengcc.top/gtetiysyeo.html

C#:   static void Main(string[] args)
来源：http://hz.iojbl.cn/gtyatzxhuv.html

[M08] 获取系统与运行时信息
来源：http://hz.cdnleiting.top/gtzqbwimez.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtnhbdzwjr.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.sweek.top/gtmqxowxuw.html

JS:   process.platform;  process.version
来源：http://hz.snrcjt.cn/gtdnwsxdht.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtahpugngf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hongshengwenyu.top/gtptwlwvax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.gotoacloud.top/gtqhoobsqt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yongpay.top/gtugndgfaf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xuanzx.com/gtznijfbhi.html

================================================================================
来源：http://hz.andypj.xyz/gtrqhycjvc.html

N. 数据结构与算法
来源：http://hz.iojbl.cn/gtlmsoakcq.html

================================================================================
来源：http://hz.shzxlz.cn/gtywqfpdpa.html

[N01] 二分查找（有序数组）
来源：http://hz.hywenlv.cn/gtsczfyzwe.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.chenjidiqi.icu/gtzyhsrqjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.chenlongwang.top/gtodcablpd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.52xcode.cn/gtyoghhjjf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.haohaochexian.top/gtfqtzlokc.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangshuangyany.cn/gtdyhjorrp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtlgdwqhyp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xingfuxueyuan.xyz/gtjrqvfgmm.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gthcbtspqg.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.xziqi.cn/gtiftagcte.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hfpthk.cn/gtwvbambvt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.aibaodan.cn/gtjdeqtpcw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.jlsjyb.cn/gtvbliybee.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhaomingkeji.xyz/gtkmuqrevm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ybcxt.top/gtgwuleyqq.html

Go:   slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gtrveczbev.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtmqjjkgaa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.chenzaomai.com/gtuaffbckj.html

[N03] 快速排序（分治示例）
来源：http://hz.svipenyu.cn/gthpkikwzi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.0kj1m.cn/gtaducprgn.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yuxming.cn/gtykuitevr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.daria6918.cn/gtffitopsv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tianlin.xyz/gtqbnzllnh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.chenjidiqi.icu/gtgwnqfzhp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yuxming.cn/gtiucmnmun.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.zhaomingkeji.xyz/gtngddizng.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.yueranfly.top/gtbihvrmay.html

[N04] 斐波那契数列
来源：http://hz.sysykeji.top/gthljetnqh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.ppjwa.cn/gtfgvswnbc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.mhx1999.top/gtuotwpuea.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jinqigufen.top/gtwvzsvdmh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtzrzpdapl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.jqgfzy.top/gtmxujddjl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.nanxinkj.top/gtwpaqdbkm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.gaohongyu789.top/gtprgzxpcm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.shangyingyoupin.top/gtqflwhcoz.html

[N05] 最大公约数
来源：http://hz.hywenlv.cn/gtdtdndgit.html

Py:   math.gcd(a, b)
来源：http://hz.nwbrower.top/gtnnozhyni.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.sysykeji.top/gtachzmwxd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.jianghu66.top/gtcrpbdyrk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.yonumen.top/gtrhossmhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.zhaomingkeji.xyz/gtlpbphpqj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.0kj1m.cn/gtlltwoqtr.html

Ruby: a.gcd(b)
来源：http://hz.ydzc1.top/gtceaxfeyv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.tianlin.xyz/gtziehsubb.html

[N06] 判断回文字符串
来源：http://hz.yangfankeji.com/gtmpoqlssg.html

Py:   s == s[::-1]
来源：http://hz.nanxuanxn.top/gtvrdkfyhb.html

PHP:  $s === strrev($s);
来源：http://hz.hnxiangtu.top/gtgnupwvod.html

JS:   s === [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtwpryurei.html

TS:   s === [...s].reverse().join("")
来源：http://hz.aizwys.cn/gtxmuafotn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.yj20258888.top/gtvaygswyg.html

Go:   // 双指针从两端比较
来源：http://hz.cheryme.top/gtfxwpsnlz.html

Ruby: s == s.reverse
来源：http://hz.cashguo.top/gtrpzkajex.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtqkrkbkis.html

[N07] 两数之和（返回下标）
来源：http://hz.52xcode.cn/gtqromilnx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.guowangkeji.top/gtybrtikwn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.nanxuanxn.top/gtozolddwp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.ywan-chungtsiang.top/gtoahnveix.html

TS:   // 手写 Map<string, number>
来源：http://hz.chenzaomai.com/gtjfhtvajy.html

Java: // 手写 HashMap
来源：http://hz.sysykeji.top/gtwywbctxy.html

Go:   // 手写 map[int]int
来源：http://hz.jinghuilouyu.cn/gtuazrhcab.html

Ruby: // 手写 Hash
来源：http://hz.yanxiufei.cn/gtqdwxnppw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.yanxiufei.cn/gtalhrzuph.html

[N08] 生成全排列
来源：http://hz.cheryme.top/gtfipbgzyu.html

Py:   itertools.permutations(arr)
来源：http://hz.cqqwz.cn/gtabfzlolo.html

PHP:  // 手写递归交换
来源：http://hz.pycfn.com/gtovfegugr.html

JS:   // 手写回溯递归
来源：http://hz.haohaochexian.top/gtahbdtpkk.html

TS:   // 手写回溯递归
来源：http://hz.wangshuangyany.cn/gtoeadfymz.html

Java: // 手写回溯递归
来源：http://hz.ydzc1.top/gtpioygslg.html

Go:   // 手写回溯递归
来源：http://hz.mhx1999.top/gtyjfhndof.html

Ruby: arr.permutation.to_a
来源：http://hz.shzxlz.cn/gtqkeeiuym.html

C#:   // 手写回溯递归
来源：http://hz.yvedp.cn/gtgctysvvp.html

[N09] 栈与队列
来源：http://hz.cheryme.top/gthlqgmvtc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.mhx1999.top/gtugdrrpak.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ehwqpu.com/gtskdekabu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.jyoumei.cn/gtginjgpcb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.tian-w.cn/gtrowrmdma.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.xziqi.cn/gtiheedxys.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.zhengqikj.top/gthozcqbzw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.zhongyouzk.top/gtiszflhmj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.xziqi.cn/gtcopqmbnt.html

[N10] 链表节点定义
来源：http://hz.yj20258.top/gteguibisa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.cdnleiting.top/gtvsffqsex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.bjfxy.top/gtbifhdwvj.html


<!-- 参考信息 -->