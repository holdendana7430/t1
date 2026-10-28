代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtzyrbqywr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtzkgdcgnr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtzbhhbuia.html

Ruby: JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtwrydtkgb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtgbocomro.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtvkhxxjlg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtdrdtquix.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtibbpydrf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtrfjmxitn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhoulong.xyz/gtdxsuvlia.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtmharrdbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gtrgdcfryq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtfvoajxxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gteebqvhvl.html

[K04] 读取 JSON 文件
来源：http://hz.zdqjudy.top/gtwqiuenbj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhengqikj.top/gtkcgvnioq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shuidangran.top/gtysgoiqpn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtkqbownct.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtofoamfwa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hammf.cn/gtxidyizhc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtsnkcnbqe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.c1oappe.top/gtitdiejdy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xylfe.cn/gtyjvddiqy.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtfjnhwgse.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtsaixyhbk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.quarkkingdee.top/gtfrnxekhw.html

JS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtvbohxxrl.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtsyfysanl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigfzy.top/gtpyplvwln.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhixingplan.top/gtemuzyesb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ywan-chungtsiang.top/gtudqdjyiy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jianghu66.top/gtykyixynw.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtejalpnar.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xinyue.icu/gtzvolvntq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtcofnhlii.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtwhwhhzzu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtbcrcmwzy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtdlqnhdjk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtpwvzdtjy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtmprnoqko.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.smart0.xyz/gteqksause.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtucyaiaqk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtnymawtgx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtrqzpzfcy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gteysqlifj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtfxfebbce.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtyuksxvtz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuxming.cn/gtcqtkovet.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtxesnkyvu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtebuuirge.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yj20258888.top/gtfvkhzsnm.html

Py:   pickle.dumps(obj)
来源：http://hz.zhaomingkeji.xyz/gtbfhecown.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtnjrvgiyy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtrtqeuxyz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtauxzhqme.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.shangyingyoupin.top/gtsqeklleo.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtdtiafdxj.html

Ruby: Marshal.dump(obj)
来源：http://hz.shanyushiyangkeji.top/gtexsiuriz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtfxcmxmjf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtawzqdjrq.html

L. 网络请求
来源：http://hz.guannengcc.top/gtlduxesnn.html

================================================================================
来源：http://hz.yuxming.cn/gtcbsehakt.html

[L01] 发送 GET 请求
来源：http://hz.hnqzz.top/gtvizgxntt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yongpay.top/gtodpqtuzh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.dashuyun.cn/gtabtonnku.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtxceaohva.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gturbjxper.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dashuyun.cn/gtuvqpgemo.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhoulong.xyz/gtdbxxbzrn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shangyingyoupin.top/gtypzgaiag.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.nwbrower.top/gtvytiuclx.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtjvncawko.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtpkudxjba.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jianghu66.top/gtzxpvgief.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sufxvd.cn/gtrvwgmupf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtqihsfdki.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtgrfzijht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtnonhatxd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dashuyun.cn/gtndfgmusa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shzxlz.cn/gtxiesrxlb.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gthtibmema.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yonumen.top/gtiiqxlinm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.snrcjt.cn/gtilcagplm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuanzx.com/gtgtgwfcah.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zdqjudy.top/gtfcxnagtm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.hnxiangtu.top/gtjwniiuwe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtsrghafme.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtbajbehen.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtunheegit.html

[L04] 设置超时
来源：http://hz.hammf.cn/gtfqrbkbjf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtmvbgfvje.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtqtgxzhvo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cdnleiting.top/gtpmhcjqof.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtkttjwsty.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.nwbrower.top/gtdnypcrsz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.9152youxi.cn/gtfqroojlj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtfxlaixsa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shuidangran.top/gtukvevdkq.html

[L05] 上传文件（multipart）
来源：http://hz.jinqigfzy.top/gtgqluuzat.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.52xcode.cn/gteosvjsio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhongyouzk.top/gtuaylkxqs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtcpmzvyse.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhoulong.xyz/gtxsqbngbz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.kuanghao11.cn/gtxeexuxrq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fengsongda.top/gtsihzgeep.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtenwlmbua.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.chenzaomai.com/gttnwkvqsr.html

[L06] 解析响应为 JSON
来源：http://hz.wangshuangyany.cn/gtfyhxyddv.html

Py:   resp.json()
来源：http://hz.yj20258888.top/gtcxjgijsw.html

PHP:  json_decode($body, true);
来源：http://hz.nanxinkj.top/gtzhvddcer.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtfnbibcew.html

TS:   await resp.json()
来源：http://hz.yanxiufei.cn/gtfjyzpbez.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhiwuduotai.top/gtuzkwbvlj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtximlfixd.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtanrmklgj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ppjwa.cn/gtyxbooexf.html

[L07] 处理 HTTP 状态码
来源：http://hz.redwolf501.top/gtltrpukgz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtsxpsacaq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nanxuanxn.top/gtnirlnuwc.html

JS:   resp.ok;  resp.status
来源：http://hz.daria6918.cn/gttvussxom.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtcsehectq.html

Java: resp.statusCode()
来源：http://hz.haohaochexian.top/gtynsaupua.html

Go:   resp.StatusCode
来源：http://hz.aizwys.cn/gtixrgbmxw.html

Ruby: resp.code.to_i
来源：http://hz.cucudq.cn/gtwwhhubtk.html

C#:   (int)resp.StatusCode
来源：http://hz.aibaodan.cn/gtfdlxuptq.html

[L08] 并发请求多个地址
来源：http://hz.yj20258888.top/gtgrbjeokw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtzomdfonb.html

PHP:  curl_multi_init() 系列
来源：http://hz.yuanzhike.top/gtslagcxka.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zhixingplan.top/gtivyhvsve.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jlsjyb.cn/gtpvcfgbuv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hammf.cn/gtpdnhgmxm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.xylfe.cn/gtxitnszdg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yvedp.cn/gtnwjlrzzp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jqgufenzy.top/gtcflecrat.html

================================================================================
来源：http://hz.yuxming.cn/gteonlvvbk.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtebabrssv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtbtjsbcwn.html

[M01] 读取命令行参数
来源：http://hz.jqgfzy.top/gtszafjgjy.html

Py:   sys.argv[1:]
来源：http://hz.ydzc1.top/gtelryesvt.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtogqkgtyv.html

JS:   process.argv.slice(2)
来源：http://hz.jiagoushi.top/gtjlhwlvgi.html

TS:   process.argv.slice(2)
来源：http://hz.xziqi.cn/gtgaeeofai.html

Java: args 数组（main 方法参数）
来源：http://hz.gogol.net.cn/gtftnvohgb.html

Go:   os.Args[1:]
来源：http://hz.pycfn.com/gtvuykkegb.html

Ruby: ARGV
来源：http://hz.tianlin.xyz/gtdhkrcxif.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnqzz.top/gtlpnazluk.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtayjppdba.html

Py:   os.environ.get("HOME")
来源：http://hz.zdqjudy.top/gtepvcvskh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pycfn.com/gtoznfkgfi.html

JS:   process.env.HOME
来源：http://hz.xylfe.cn/gtsbjvvcyo.html

TS:   process.env.HOME
来源：http://hz.jinyuanbaomall.cn/gtmrplgimx.html

Java: System.getenv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtpbgknief.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.dianchejie.cn/gtjsazfwih.html

Ruby: ENV["HOME"]
来源：http://hz.sxryk.cn/gtddbuyjwd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.guannengcc.top/gtpfgwfzns.html

[M03] 执行外部命令
来源：http://hz.gaohongyu789.top/gtiavsdgth.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shangyingyoupin.top/gtklxqrsrq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ivvv.top/gtoswqhqom.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yj20258888.top/gthmslsjku.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.dianchejie.cn/gtgtoduqzt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yonumen.top/gtondeijll.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.jqgufenzy.top/gtfcopuxjo.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.andypj.xyz/gthebsvkdy.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ivvv.top/gtspugvbgy.html

[M04] 获取当前工作目录
来源：http://hz.ehwqpu.com/gtzpspgdfk.html

Py:   os.getcwd()
来源：http://hz.ppjwa.cn/gttbntymnq.html

PHP:  getcwd();
来源：http://hz.jinqigufen.top/gtvzpkcnrr.html

JS:   process.cwd()
来源：http://hz.jinghuilouyu.cn/gtggzmtnhw.html

TS:   process.cwd()
来源：http://hz.zhengqikj.top/gtzzajogrs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.wangdashe.top/gtuashbrph.html

Go:   os.Getwd()
来源：http://hz.xylfe.cn/gtnlpotfci.html

Ruby: Dir.pwd
来源：http://hz.pengpengdd.cyou/gtfzdjefdh.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.c1oappe.top/gtilhdzxne.html

[M05] 设置退出码
来源：http://hz.fzhhl.top/gtkhtldhdl.html

Py:   sys.exit(1)
来源：http://hz.jqgufenzy.top/gtdonjroaz.html

PHP:  exit(1);
来源：http://hz.ybcxt.top/gtwppmqxdk.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gteeajuxdh.html

TS:   process.exit(1)
来源：http://hz.sxryk.cn/gtjgnmiugg.html

Java: System.exit(1)
来源：http://hz.wangshuangyany.cn/gtaywuhsca.html

Go:   os.Exit(1)
来源：http://hz.bjfxy.top/gtafjhqxxl.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtnohztnav.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yuxming.cn/gtwfvsfchv.html

[M06] 向标准错误输出
来源：http://hz.ywan-chungtsiang.top/gtpotocazh.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gaohongyu789.top/gtiopunedi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.xingfuxueyuan.xyz/gtmzkpnlfh.html

JS:   console.error("err")
来源：http://hz.hongshengwenyu.top/gtusjbbevp.html

TS:   console.error("err")
来源：http://hz.sweek.top/gteiadaqcz.html

Java: System.err.println("err")
来源：http://hz.daria6918.cn/gtfbcdvgkj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.gzhubu.top/gtoaikfhje.html

Ruby: warn "err"
来源：http://hz.jqgfzy.top/gtreyfbzok.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.52xcode.cn/gtsfhwfccv.html

[M07] 判断是否为主入口
来源：http://hz.andypj.xyz/gtpyqtrbhj.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtqhccmsuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sxryk.cn/gtqgonzntw.html

JS:   require.main === module
来源：http://hz.xuetiantiany.cn/gtkzbncknp.html

TS:   require.main === module
来源：http://hz.jlsjyb.cn/gtrioskbqp.html

Java: public static void main(String[] args)
来源：http://hz.nwbrower.top/gthzwlsdst.html

Go:   func main()
来源：http://hz.tian-w.cn/gtpiszasxm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.zdqjudy.top/gtvxouibpt.html

C#:   static void Main(string[] args)
来源：http://hz.nwbrower.top/gtksnkaoal.html

[M08] 获取系统与运行时信息
来源：http://hz.cashguo.top/gtbjxihdmt.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yuxming.cn/gtmnpzdqbe.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.haohaochexian.top/gtgkvrdlfw.html

JS:   process.platform;  process.version
来源：http://hz.ybcxt.top/gtzovgbuld.html

TS:   process.platform;  process.version
来源：http://hz.gaohongyu789.top/gtxovqobps.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.fzhhl.top/gtwijwluqs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yonumen.top/gtvqwfurop.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.kuanghao11.cn/gtgmuwfbks.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.shuidangran.top/gtxplclozt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdsudapzx.html

N. 数据结构与算法
来源：http://hz.jinqigfzy.top/gtjksdptao.html

================================================================================
来源：http://hz.xinyue.icu/gtnaefuzwc.html

[N01] 二分查找（有序数组）
来源：http://hz.quarkkingdee.top/gtzyvnvxss.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtgwvbhxmo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.0kj1m.cn/gtegvxuxys.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenlongwang.top/gtagctlhak.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.feifeiyinyue.top/gtufaociav.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gtgpejrshk.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtsyzswwob.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.fzhhl.top/gtzsjqhgfu.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.birdmap.top/gttmujvnws.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.52xcode.cn/gtpyaaauzg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhixingplan.top/gtwtbhgcxr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.quarkkingdee.top/gtgiafhkrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtxtboqoan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.chenzaomai.com/gtaamqcopf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenzaomai.com/gtvsxurvfp.html

Go:   slices.Sort(arr)
来源：http://hz.chenjidiqi.icu/gtluverytr.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtegkpnjgn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.jqgfzy.top/gtuzvhuolg.html

[N03] 快速排序（分治示例）
来源：http://hz.wangdashe.top/gtkaaclayc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.iojbl.cn/gtlebhbxia.html

PHP:  // 递归实现，或用 usort
来源：http://hz.nanxuanxn.top/gtllrggqut.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.wangshuangyany.cn/gtntnofteq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.gzhubu.top/gtexbysgxa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.yvedp.cn/gtrdgpeelw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.aizwys.cn/gtysqknqwu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.sxryk.cn/gtswexyxtp.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.iojbl.cn/gtlfnctbws.html

[N04] 斐波那契数列
来源：http://hz.316326.xyz/gtblkphsus.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.xinyue.icu/gtcakkvmpb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.xziqi.cn/gtisidymuf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.meibo888.top/gtxpqdvjrq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.gaohongyu789.top/gttwidaqxt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.zycfv.cn/gtoimqmnwo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.vqdsnc.cn/gthkixgmqc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.jinghuilouyu.cn/gtpwfhnonn.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.hammf.cn/gtfdmthhyc.html

[N05] 最大公约数
来源：http://hz.sysykeji.top/gtuadtcajc.html

Py:   math.gcd(a, b)
来源：http://hz.nanxuanxn.top/gtcbuypxuk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinyuanbaomall.cn/gtfnexqspk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.zhongyouzk.top/gtobygkiul.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.andypj.xyz/gtszecxpuv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.hfpthk.cn/gtavayuqgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.gotoacloud.top/gtuggjwumi.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtrnzzkunn.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.kuanghao11.cn/gtcxbqzzrm.html

[N06] 判断回文字符串
来源：http://hz.yuanzhike.top/gtinxldkfw.html

Py:   s == s[::-1]
来源：http://hz.chenjidiqi.icu/gtdwddodkp.html

PHP:  $s === strrev($s);
来源：http://hz.yj202588.top/gthpaixrip.html

JS:   s === [...s].reverse().join("")
来源：http://hz.fzhhl.top/gtgardilfr.html

TS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtdjaemhib.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zhixingplan.top/gtfxydstry.html

Go:   // 双指针从两端比较
来源：http://hz.yuanzhike.top/gtmxcnlsqw.html

Ruby: s == s.reverse
来源：http://hz.shangyingyoupin.top/gtoduuexgr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.iojbl.cn/gtiytlfxzt.html

[N07] 两数之和（返回下标）
来源：http://hz.yonumen.top/gtxvlretls.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.smart0.xyz/gtzbmlyywn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.gotoacloud.top/gtqvkodtsz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.guowangkeji.top/gttkiohrvx.html

TS:   // 手写 Map<string, number>
来源：http://hz.jlsjyb.cn/gtswntywaq.html

Java: // 手写 HashMap
来源：http://hz.wangdashe.top/gttcpqibvd.html

Go:   // 手写 map[int]int
来源：http://hz.cucudq.cn/gtlkfbiisr.html

Ruby: // 手写 Hash
来源：http://hz.cdnleiting.top/gtjkqeeahw.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.redwolf501.top/gtdgutfvlc.html

[N08] 生成全排列
来源：http://hz.jyoumei.cn/gtzgdohgsw.html

Py:   itertools.permutations(arr)
来源：http://hz.svipenyu.cn/gtayhaupov.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtvpyioisb.html

JS:   // 手写回溯递归
来源：http://hz.nanxinkj.top/gtsnpynxjt.html

TS:   // 手写回溯递归
来源：http://hz.jianghu66.top/gtdjxgnuqu.html

Java: // 手写回溯递归
来源：http://hz.jqgfzy.top/gtimhqxayd.html

Go:   // 手写回溯递归
来源：http://hz.cheryme.top/gttiupxkis.html

Ruby: arr.permutation.to_a
来源：http://hz.52xcode.cn/gttevqxneh.html

C#:   // 手写回溯递归
来源：http://hz.fzhhl.top/gtgkncyidk.html

[N09] 栈与队列
来源：http://hz.gogol.net.cn/gtlmhporrt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.andypj.xyz/gtpevvrmdx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hnxiangtu.top/gtlaxduzas.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.cashguo.top/gtmftpnidi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.meibo888.top/gttkwcifad.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.redwolf501.top/gtqtmaffji.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.chenzaomai.com/gttzqplify.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.cdnleiting.top/gtkyirctpq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.dashuyun.cn/gtrefqgbxd.html

[N10] 链表节点定义
来源：http://hz.quarkkingdee.top/gtikbmrvsx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.aizwys.cn/gtwvqumfsa.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.dashuyun.cn/gtrngjnbcd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cdnleiting.top/gtuujlyjkt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.zhongyouzk.top/gtzprbrwgu.html

Java: class Node { int v; Node next; }
来源：http://hz.jqgufenzy.top/gtxtxqwvmu.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yangfankeji.com/gthdvxiyzc.html


<!-- 参考信息 -->