代发 wailian999

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtrbuqnruu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtobnsjvie.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtoireewvn.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258888.top/gtifiemhoi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zycfv.cn/gtkhdhzncr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xingfuxueyuan.xyz/gtvsbehyni.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtboltbsox.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtctqsebdx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtrjycvxnu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtgcnkhtgb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aibaodan.cn/gtnfzzzbbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtjfvdmyre.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gzhubu.top/gtvtltzwow.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtvbjxfnye.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gtvrxyahor.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhongyouzk.top/gtdalruaqi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gttarcvwxq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtmkaudlsd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtmszkfees.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxuanxn.top/gtsuhmrrst.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gthmeoauvz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtaememlvm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtbiyknnnm.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gthrdqccpb.html

Py:   copy.deepcopy(obj)
来源：http://hz.birdmap.top/gthdlrutsf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gtvdllhqvq.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtyjzkyzhd.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtquhtjkvw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.kuanghao11.cn/gtugqogxxp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtrxbjhtii.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yongpay.top/gtbksfddty.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinghuilouyu.cn/gtbjnjnwyv.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gtxvsykonx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jlsjyb.cn/gtmblefldk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtrlylhqgy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtswqmkwhm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gthcmyhyic.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cashguo.top/gtinyjjzyb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ivvv.top/gtlweflesb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.meibo888.top/gtdiwnfrmn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ybcxt.top/gtdoaawuow.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtaqhkicuj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.kuanghao11.cn/gttofqhgks.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhengqikj.top/gtgyhwtkyk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtrcvlyqlm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtxfsqlkmn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gteduznymz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gttlicsipg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj202588.top/gtqeizyogn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.9152youxi.cn/gtlxlliiog.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gttwubtvtz.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtzqmrliwz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shangyingyoupin.top/gtgsbegltv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtgxupmoba.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gthehmauft.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hongshengwenyu.top/gtplyqydfl.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtnzcwfsnz.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtsowviqnw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.wangshuangyany.cn/gtgioolfzk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwvxwwnsk.html

L. 网络请求
来源：http://hz.yonumen.top/gtmwpckmbo.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwichmzra.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtvuxhjcty.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.redwolf501.top/gtuwwsldyw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ppjwa.cn/gthtuwsblp.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtbxzmpwie.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtdtybsqwk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtxlfxcufg.html

Go:   resp, err := http.Get(url)
来源：http://hz.0kj1m.cn/gtxjteoscv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtbhiietev.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gteazyxuhd.html

[L02] 发送 POST JSON
来源：http://hz.smart0.xyz/gtgghvoifv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yvedp.cn/gtwfbttkhb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtoojeejxg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtmdjihaqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtacikvzkr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtjqufnqzi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xingfuxueyuan.xyz/gtqizlgupo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.quarkkingdee.top/gtpjqpsqcz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.cucudq.cn/gtryqslxmg.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtqlqczcds.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.0kj1m.cn/gtwcddrkrr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ydzc1.top/gtrgyfvgeh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gthnubnzxi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtxvvhrfnd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gtsmkmdcci.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jianghu66.top/gtwkkbetyl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daxiang520.top/gtdnugjzoy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shuidangran.top/gtqxvlettc.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtboeeuhfp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gthhsswlxy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtrtnimafj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtxmffsbau.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xingfuxueyuan.xyz/gtqckfjomd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.9152youxi.cn/gtmfdrfaru.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guowangkeji.top/gtuhtxdazy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.wangshuangyany.cn/gtkefwfosu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yuanzhike.top/gtxxqucfot.html

[L05] 上传文件（multipart）
来源：http://hz.andypj.xyz/gtncrlsevo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jqgfzy.top/gtzbwgvfad.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ivvv.top/gtslkfgpgh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxinkj.top/gtlomxnjpz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtlwnagrhi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sxryk.cn/gtohvakwhj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtkuooiljx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.svipenyu.cn/gtkidraxmv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guannengcc.top/gtwatlhsbv.html

[L06] 解析响应为 JSON
来源：http://hz.redwolf501.top/gtszpcqvrd.html

Py:   resp.json()
来源：http://hz.aibaodan.cn/gtdzkmbszd.html

PHP:  json_decode($body, true);
来源：http://hz.hongshengwenyu.top/gtbhdrumwv.html

JS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtkkiqgcur.html

TS:   await resp.json()
来源：http://hz.jqgufenzy.top/gthblpmoij.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtwcvhrvik.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jyoumei.cn/gtbpskrsry.html

Ruby: JSON.parse(resp.body)
来源：http://hz.haohaochexian.top/gtjkfvexhu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtwtsvkjif.html

[L07] 处理 HTTP 状态码
来源：http://hz.xylfe.cn/gtjzceuqvl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gtfxoyxyue.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gaohongyu789.top/gtillqdeuu.html

JS:   resp.ok;  resp.status
来源：http://hz.jinyuanbaomall.cn/gtnlsqiirn.html

TS:   resp.ok;  resp.status
来源：http://hz.svipenyu.cn/gtascumkpm.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtazxkkdxl.html

Go:   resp.StatusCode
来源：http://hz.hnxiangtu.top/gtuqgcyiqk.html

Ruby: resp.code.to_i
来源：http://hz.gaohongyu789.top/gtuugfqnvv.html

C#:   (int)resp.StatusCode
来源：http://hz.9152youxi.cn/gtnpwoheqn.html

[L08] 并发请求多个地址
来源：http://hz.yonumen.top/gtzzjirpne.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.xuetiantiany.cn/gtcbwxoryk.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhongyouzk.top/gtdapfquhv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtbaqhxvsj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtlkasayor.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.chenjidiqi.icu/gtieqwlkgo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.svipenyu.cn/gtcbbrmejw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jlsjyb.cn/gtufxsjfmy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.fzhhl.top/gtuhzydkfv.html

================================================================================
来源：http://hz.tianlin.xyz/gtfzwffrrq.html

M. 命令行 / 进程 / 环境
来源：http://hz.ivvv.top/gtgboasglf.html

================================================================================
来源：http://hz.redwolf501.top/gtnhmwqive.html

[M01] 读取命令行参数
来源：http://hz.zhiwuduotai.top/gtrsglmoed.html

Py:   sys.argv[1:]
来源：http://hz.pycfn.com/gtqgkooklm.html

PHP:  $argv;  $argc;
来源：http://hz.birdmap.top/gtkkwxytao.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtqbbxkhak.html

TS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtcqxcdfoo.html

Java: args 数组（main 方法参数）
来源：http://hz.shuidangran.top/gtjxhmvunc.html

Go:   os.Args[1:]
来源：http://hz.iojbl.cn/gtlprmcsrd.html

Ruby: ARGV
来源：http://hz.52xcode.cn/gtpgvgwqfx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.cucudq.cn/gtrhoquelp.html

[M02] 读取环境变量
来源：http://hz.9152youxi.cn/gtqlxdmspw.html

Py:   os.environ.get("HOME")
来源：http://hz.sxryk.cn/gtjiueuqac.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtenkzdfjy.html

JS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtyomrdeby.html

TS:   process.env.HOME
来源：http://hz.redwolf501.top/gttgkiwhom.html

Java: System.getenv("HOME")
来源：http://hz.zycfv.cn/gtpvgangdp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtxyhjrpsi.html

Ruby: ENV["HOME"]
来源：http://hz.yj20258888.top/gthjxxyxsw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.ehwqpu.com/gtiirydpww.html

[M03] 执行外部命令
来源：http://hz.zhijiandao.cn/gtfupobjyy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shanyushiyangkeji.top/gtipoencsx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jyoumei.cn/gtapaidirb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.zycfv.cn/gtoagnebhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtyqqyviuf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.smart0.xyz/gtuztiwujw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.smart0.xyz/gttfeqomoh.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangdashe.top/gtgtqwazor.html

C#:   Process.Start("ls", "-l");
来源：http://hz.gogol.net.cn/gtjvxhwvnq.html

[M04] 获取当前工作目录
来源：http://hz.ydzc1.top/gtpzzrxwua.html

Py:   os.getcwd()
来源：http://hz.tanke756.top/gtbaaickic.html

PHP:  getcwd();
来源：http://hz.xuanzx.com/gtgwewlqkr.html

JS:   process.cwd()
来源：http://hz.ivvv.top/gtmjxqbrwe.html

TS:   process.cwd()
来源：http://hz.ivvv.top/gtygqbapkp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xinyue.icu/gtonnonhzy.html

Go:   os.Getwd()
来源：http://hz.ppjwa.cn/gtndtaadpu.html

Ruby: Dir.pwd
来源：http://hz.316326.xyz/gtgylbuudt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shangyingyoupin.top/gtbrtozcxp.html

[M05] 设置退出码
来源：http://hz.gogol.net.cn/gttxpjzdmf.html

Py:   sys.exit(1)
来源：http://hz.sxryk.cn/gtupxnzmns.html

PHP:  exit(1);
来源：http://hz.xuanzx.com/gtjzqnwwci.html

JS:   process.exit(1)
来源：http://hz.tanke756.top/gtjgbbewal.html

TS:   process.exit(1)
来源：http://hz.jianghu66.top/gtxvrlfwrv.html

Java: System.exit(1)
来源：http://hz.pycfn.com/gtidbnmjlx.html

Go:   os.Exit(1)
来源：http://hz.vqdsnc.cn/gtkfixfzeo.html

Ruby: exit 1
来源：http://hz.zhongyouzk.top/gtbqcpibbz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ydjk.org.cn/gtenlzecgo.html

[M06] 向标准错误输出
来源：http://hz.nanxinkj.top/gtrkvwnwdg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yongpay.top/gtluorqmdt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.haohaochexian.top/gtujwuqdxo.html

JS:   console.error("err")
来源：http://hz.ydjk.org.cn/gttsneaqfn.html

TS:   console.error("err")
来源：http://hz.svipenyu.cn/gtvsmdorln.html

Java: System.err.println("err")
来源：http://hz.wangdashe.top/gtlzadvhbs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jqgfzy.top/gtebwqjhmp.html

Ruby: warn "err"
来源：http://hz.zdqjudy.top/gtoxbpcpfu.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.dashuyun.cn/gtrxhjhgxo.html

[M07] 判断是否为主入口
来源：http://hz.hammf.cn/gtzxazgudk.html

Py:   if __name__ == "__main__":
来源：http://hz.yongpay.top/gtnyvuqkoh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.haohaochexian.top/gtioslqmnq.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gtcxcacjkb.html

TS:   require.main === module
来源：http://hz.zhijiandao.cn/gtaxnfdhwv.html

Java: public static void main(String[] args)
来源：http://hz.ivvv.top/gtwbcwewka.html

Go:   func main()
来源：http://hz.gzhubu.top/gtrjyehiqs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.hammf.cn/gtrvsjdawk.html

C#:   static void Main(string[] args)
来源：http://hz.cucudq.cn/gtqyrugihm.html

[M08] 获取系统与运行时信息
来源：http://hz.vqdsnc.cn/gtkgefhkpx.html

Py:   platform.system();  platform.python_version()
来源：http://hz.0kj1m.cn/gtxjazrgmu.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.zhaomingkeji.xyz/gtklffahqk.html

JS:   process.platform;  process.version
来源：http://hz.bjfxy.top/gtkgmpapcb.html

TS:   process.platform;  process.version
来源：http://hz.hfpthk.cn/gtyxwfekwl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gthcpvbnny.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.nanxuanxn.top/gtlutqdkau.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.52xcode.cn/gtsmgrbfbu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xinyue.icu/gtoqjgcwcc.html

================================================================================
来源：http://hz.52xcode.cn/gtubufmknr.html

N. 数据结构与算法
来源：http://hz.sweek.top/gtaidfdhrv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtbhppwmhl.html

[N01] 二分查找（有序数组）
来源：http://hz.tianlin.xyz/gtocfozlmo.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.sxryk.cn/gtaddfrgyy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtbsthuqzd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xingfuxueyuan.xyz/gtucngaqca.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xinyue.icu/gtcdtbqhcj.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.wangdashe.top/gtjnpbkdic.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.yuanzhike.top/gtmjcmehnx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.xziqi.cn/gtmszebghi.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.shzxlz.cn/gtzsqipczz.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.jianghu66.top/gtjrisvtvz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtivontics.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.tian-w.cn/gtajphxbod.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhoulong.xyz/gtejsvlzke.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.feifeiyinyue.top/gtbcmodhxy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.chenlongwang.top/gtnflvanau.html

Go:   slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtpcxlhzjk.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtvrytyeqs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.tanke756.top/gtmarocdcl.html

[N03] 快速排序（分治示例）
来源：http://hz.sysykeji.top/gtwiufsqzu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.chenlongwang.top/gttnidcnti.html

PHP:  // 递归实现，或用 usort
来源：http://hz.shanyushiyangtech.top/gtjocdtbuw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gtpwyfvyfg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.haohaochexian.top/gthucjbnsx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.quarkkingdee.top/gtggtgelkd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.jinqigufen.top/gtomryoiiy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.yj202588.top/gtwmzdafpu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.fengsongda.top/gtkkuzvbod.html

[N04] 斐波那契数列
来源：http://hz.aibaodan.cn/gtolodepnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtdujyetug.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.0kj1m.cn/gtvcsnewgn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jqgufenzy.top/gtlzwxffzf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.guannengcc.top/gtqovhqlbv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.feifeiyinyue.top/gtxxcinvga.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.52xcode.cn/gtmmcomnth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.zhongyouzk.top/gtjebkbcdb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj20258888.top/gtxfnsucov.html

[N05] 最大公约数
来源：http://hz.smart0.xyz/gtmwcmgdhd.html

Py:   math.gcd(a, b)
来源：http://hz.pycfn.com/gtkyrweqsj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.snrcjt.cn/gtsddahhqm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.nanxuanxn.top/gteivepmek.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.havefunace.top/gtadrlpikk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.mhx1999.top/gtnvpxvhqg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sufxvd.cn/gtodwwyvoc.html

Ruby: a.gcd(b)
来源：http://hz.zdqjudy.top/gtihufobsa.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.pengpengdd.cyou/gtybesyuvj.html

[N06] 判断回文字符串
来源：http://hz.sxryk.cn/gtgzblripc.html

Py:   s == s[::-1]
来源：http://hz.316326.xyz/gtpjpjsvrx.html

PHP:  $s === strrev($s);
来源：http://hz.cashguo.top/gtyhxgrmou.html

JS:   s === [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtypntekbd.html

TS:   s === [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtpeuleuwr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cdnleiting.top/gtxujpakvv.html

Go:   // 双指针从两端比较
来源：http://hz.hysaishi.cn/gtthirmhhn.html

Ruby: s == s.reverse
来源：http://hz.jinyuanbaomall.cn/gtwqhtouga.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtqbxdprqt.html

[N07] 两数之和（返回下标）
来源：http://hz.hysaishi.cn/gtvacpvzbq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.feifeiyinyue.top/gtueubvzfn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.cashguo.top/gtpdtpvfry.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.tianlin.xyz/gtsoxmgflr.html

TS:   // 手写 Map<string, number>
来源：http://hz.cdnleiting.top/gtlonaqmzb.html

Java: // 手写 HashMap
来源：http://hz.shangyingyoupin.top/gtcyvilaxb.html

Go:   // 手写 map[int]int
来源：http://hz.chenzaomai.com/gtsuchkfxu.html

Ruby: // 手写 Hash
来源：http://hz.yuxming.cn/gtijarxhvy.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.jiagoushi.top/gtywuxfnzc.html

[N08] 生成全排列
来源：http://hz.xingfuxueyuan.xyz/gtzbfysjeg.html

Py:   itertools.permutations(arr)
来源：http://hz.yj20258888.top/gtnssreaes.html

PHP:  // 手写递归交换
来源：http://hz.cqqwz.cn/gtetfjwbgw.html

JS:   // 手写回溯递归
来源：http://hz.kuanghao11.cn/gtkcgczmsv.html

TS:   // 手写回溯递归
来源：http://hz.chenlongwang.top/gtqlgbydwx.html

Java: // 手写回溯递归
来源：http://hz.tian-w.cn/gtrrjnzdvy.html

Go:   // 手写回溯递归
来源：http://hz.hongshengwenyu.top/gttaoxkfkp.html

Ruby: arr.permutation.to_a
来源：http://hz.jiagoushi.top/gtxisvpadl.html

C#:   // 手写回溯递归
来源：http://hz.hfpthk.cn/gtjjmtwknq.html

[N09] 栈与队列
来源：http://hz.quarkkingdee.top/gtnsrhhitv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.xinyue.icu/gtwinnidzt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.mhx1999.top/gtgzxeltbp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtzscodloo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.zycfv.cn/gthvfbgxvm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.hywenlv.cn/gtzhghgrrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtxvysbayn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.sweek.top/gtecierqrw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.jinyuanbaomall.cn/gtrxjfmuud.html

[N10] 链表节点定义
来源：http://hz.redwolf501.top/gtnwybnxiu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.quarkkingdee.top/gtsqehjdhh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.xylfe.cn/gtlqgwlbjx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.xuanzx.com/gtchlvlkgg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.yongpay.top/gtmplaizzw.html

Java: class Node { int v; Node next; }
来源：http://hz.zhengqikj.top/gtkibqbxws.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.yj20258.top/gtzimaserg.html


<!-- 参考信息 -->