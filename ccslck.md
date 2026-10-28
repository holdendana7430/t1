代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtskfeojrp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtvdpdntfg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gthckjlugl.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtvhwkrmqk.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtzcamljow.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtmjnnqege.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtnowkhlyg.html

TS:   structuredClone(obj)
来源：http://hz.yongpay.top/gtlqridbop.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhoulong.xyz/gtyiatziko.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtpgsyretm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yongpay.top/gtascbfryx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtimnpdgwr.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gtrqwcitot.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtertcygul.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtvmstcvub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtjkmfcxiq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtgqebzolv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtkepexrgo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydzc1.top/gtvdsfgpvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtmuxgwkme.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtwvyfpypw.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtmcoxulgi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtclkbmivh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.9152youxi.cn/gtxidtjdhd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtypytfqqm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtybfaxbud.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtxkudigtn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.snrcjt.cn/gtlrajtswl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtzqqyhsvy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtgdzkuorm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gttwnmnhfu.html

Py:   pickle.dumps(obj)
来源：http://hz.xylfe.cn/gtjbcuviah.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xuetiantiany.cn/gtzkhltxcf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nwbrower.top/gtxpsfrvgm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtghspmreo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cashguo.top/gtiednlotj.html

Go:   encoding/gob
来源：http://hz.shangyingyoupin.top/gtehzmfbjz.html

Ruby: Marshal.dump(obj)
来源：http://hz.zdqjudy.top/gtagumrvnj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtofwtbtch.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjxkwzsxn.html

L. 网络请求
来源：http://hz.zhiwuduotai.top/gtxtgylpww.html

================================================================================
来源：http://hz.jyoumei.cn/gtqknsfkne.html

[L01] 发送 GET 请求
来源：http://hz.kuanghao11.cn/gtaecjqopd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gthmgblhoo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuetiantiany.cn/gtbyeshgcd.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gtvoqqhecz.html

TS:   await fetch(url)
来源：http://hz.bjfxy.top/gtxteevtux.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.iojbl.cn/gtktsrlqas.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gtttmvtlhl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gthmijopft.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gtqhaivkqd.html

[L02] 发送 POST JSON
来源：http://hz.ydjk.org.cn/gtowtwzzyi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gthcqlpirz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daxiang520.top/gtwikpcznk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtpamxniwt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtnqnvzrvh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gtwfhtqtuq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nwbrower.top/gtcuasjjtd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtpuuzzngz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.shuidangran.top/gtnhsmtxmu.html

[L03] 设置自定义请求头
来源：http://hz.zdqjudy.top/gtrkuicpcu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yanxiufei.cn/gtxxekfgbs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cheryme.top/gtgugdmuma.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtsolfvmdj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtzvolblns.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtqvrblkxo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jinqigufen.top/gtssopfywv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sweek.top/gtbeckvpnt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangshuangyany.cn/gtwhzzmvvf.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtnfjsvcub.html

Py:   requests.get(url, timeout=5)
来源：http://hz.hammf.cn/gthydnztku.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shanyushiyangtech.top/gtikqdzinz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sweek.top/gtwzjmpzte.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinqigfzy.top/gtnjhgcqnd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pycfn.com/gtfiezfxol.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.cheryme.top/gtvetqttkz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.fengsongda.top/gtvgniqcke.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yvedp.cn/gterhjlxps.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtnkonntqe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gttaflymku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hongshengwenyu.top/gtnjarsmoj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtypreeaaq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.52xcode.cn/gtuqxwmrew.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtaqoqrbhj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinghuilouyu.cn/gtrstwnflg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtizrnjfqd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtlmrzqvqn.html

[L06] 解析响应为 JSON
来源：http://hz.snrcjt.cn/gtenkjfral.html

Py:   resp.json()
来源：http://hz.chenjidiqi.icu/gtfqiqhvls.html

PHP:  json_decode($body, true);
来源：http://hz.hnqzz.top/gtzeftukrg.html

JS:   await resp.json()
来源：http://hz.snrcjt.cn/gtovnbmbkz.html

TS:   await resp.json()
来源：http://hz.zhengqikj.top/gtsptzvjgp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yj20258.top/gtnkoeppca.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.wangdashe.top/gtxjggtwxo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.c1oappe.top/gtvpfefbbc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.c1oappe.top/gthckiulcn.html

[L07] 处理 HTTP 状态码
来源：http://hz.c1oappe.top/gtwzjkbaej.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.iojbl.cn/gtcblhcczj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangshuangyany.cn/gtzjxcszly.html

JS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtjlcfhzll.html

TS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtxejmggjv.html

Java: resp.statusCode()
来源：http://hz.aizwys.cn/gtueivrlzm.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtpntqyivt.html

Ruby: resp.code.to_i
来源：http://hz.xylfe.cn/gtqhrwbucx.html

C#:   (int)resp.StatusCode
来源：http://hz.yj202588.top/gtwxochtbp.html

[L08] 并发请求多个地址
来源：http://hz.havefunace.top/gtivpyfmmi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.mhx1999.top/gtngglhhve.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinyuanbaomall.cn/gtlrfoptyq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.0kj1m.cn/gthrfhwsrs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtwffzujog.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.nwbrower.top/gtxxaoeigi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pycfn.com/gtobgttclh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xinyue.icu/gtbrcxnsav.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhengqikj.top/gtegqiowqi.html

================================================================================
来源：http://hz.jqgfzy.top/gtyadfjtbl.html

M. 命令行 / 进程 / 环境
来源：http://hz.yongpay.top/gtxqjmklof.html

================================================================================
来源：http://hz.tanke756.top/gtvlqdtyus.html

[M01] 读取命令行参数
来源：http://hz.hfpthk.cn/gtphtsevnd.html

Py:   sys.argv[1:]
来源：http://hz.xylfe.cn/gtoxjmkhdg.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigfzy.top/gtnebijpnv.html

JS:   process.argv.slice(2)
来源：http://hz.nanxuanxn.top/gtqtujiscg.html

TS:   process.argv.slice(2)
来源：http://hz.ydzc1.top/gtwrieprsj.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtqhlmwxze.html

Go:   os.Args[1:]
来源：http://hz.yuanzhike.top/gtxlggojim.html

Ruby: ARGV
来源：http://hz.316326.xyz/gtkbnvkwdl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hywenlv.cn/gthvdfcgzw.html

[M02] 读取环境变量
来源：http://hz.xuanzx.com/gtfthctare.html

Py:   os.environ.get("HOME")
来源：http://hz.aizwys.cn/gtfdrehnds.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtygxiajhe.html

JS:   process.env.HOME
来源：http://hz.bjfxy.top/gttimihbqn.html

TS:   process.env.HOME
来源：http://hz.svipenyu.cn/gthbmypsqu.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gtobjiagzl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.andypj.xyz/gtlesqnqlf.html

Ruby: ENV["HOME"]
来源：http://hz.wangshuangyany.cn/gtfpqydqwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangtech.top/gthfjkifiw.html

[M03] 执行外部命令
来源：http://hz.yonumen.top/gtzgahqynz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sxryk.cn/gtqerqhcdq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ydjk.org.cn/gtuxuyrvnq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.daria6918.cn/gtappozhll.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gthpmurnnb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cdnleiting.top/gtaknlslvn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.hysaishi.cn/gtyjyndzwc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gthvuepclb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.9152youxi.cn/gtxbnhgamb.html

[M04] 获取当前工作目录
来源：http://hz.chenjidiqi.icu/gtiblblhaq.html

Py:   os.getcwd()
来源：http://hz.ehwqpu.com/gtcspwwust.html

PHP:  getcwd();
来源：http://hz.jyoumei.cn/gtrrvkgade.html

JS:   process.cwd()
来源：http://hz.zhiwuduotai.top/gtobjojegh.html

TS:   process.cwd()
来源：http://hz.svipenyu.cn/gtfntluqjw.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.fzhhl.top/gthengsbgc.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtlfnjehgs.html

Ruby: Dir.pwd
来源：http://hz.shangyingyoupin.top/gtkhjxlkyd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.cheryme.top/gtpsvdxizj.html

[M05] 设置退出码
来源：http://hz.xziqi.cn/gtlsfwwyhz.html

Py:   sys.exit(1)
来源：http://hz.vqdsnc.cn/gtfusclqes.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtwtwdhwnu.html

JS:   process.exit(1)
来源：http://hz.tian-w.cn/gtybzxsild.html

TS:   process.exit(1)
来源：http://hz.ppjwa.cn/gtugekosyc.html

Java: System.exit(1)
来源：http://hz.zhongyouzk.top/gtioryapmv.html

Go:   os.Exit(1)
来源：http://hz.jqgufenzy.top/gtdfkzreni.html

Ruby: exit 1
来源：http://hz.fzhhl.top/gtfvlvrony.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.guannengcc.top/gteprxhbpg.html

[M06] 向标准错误输出
来源：http://hz.guannengcc.top/gtajlrudgg.html

Py:   print("err", file=sys.stderr)
来源：http://hz.gogol.net.cn/gtzwawwsql.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.jinghuilouyu.cn/gtakabmsfj.html

JS:   console.error("err")
来源：http://hz.ywan-chungtsiang.top/gtgdjxhthy.html

TS:   console.error("err")
来源：http://hz.yuanzhike.top/gtpcidcbwf.html

Java: System.err.println("err")
来源：http://hz.xuetiantiany.cn/gtizchtpov.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.snrcjt.cn/gtnleabhcm.html

Ruby: warn "err"
来源：http://hz.jinyuanbaomall.cn/gtjktpjuls.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.tanke756.top/gtxhxcrcim.html

[M07] 判断是否为主入口
来源：http://hz.pengpengdd.cyou/gtsyooiduf.html

Py:   if __name__ == "__main__":
来源：http://hz.yuxming.cn/gtvkivpixy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cashguo.top/gtoymjzrpv.html

JS:   require.main === module
来源：http://hz.xuanzx.com/gtzsykmrym.html

TS:   require.main === module
来源：http://hz.cqqwz.cn/gthloyesdq.html

Java: public static void main(String[] args)
来源：http://hz.mhx1999.top/gtdhrnjobb.html

Go:   func main()
来源：http://hz.yangfankeji.com/gtsirxuywz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jiagoushi.top/gtflvhxgme.html

C#:   static void Main(string[] args)
来源：http://hz.zdqjudy.top/gtphqfbtgx.html

[M08] 获取系统与运行时信息
来源：http://hz.chenzaomai.com/gtmkngmtrd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.yanxiufei.cn/gtcxuqshwl.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtxcorrulu.html

JS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtbziepifi.html

TS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtbpwkxxip.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.tanke756.top/gtzkobnxff.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhixingplan.top/gtswlrzcnw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.yj20258888.top/gthpkxbhgr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yangfankeji.com/gtxzfgmiya.html

================================================================================
来源：http://hz.fengsongda.top/gtjvlipuei.html

N. 数据结构与算法
来源：http://hz.wangdashe.top/gtoficphvw.html

================================================================================
来源：http://hz.fzhhl.top/gtnnqplgmf.html

[N01] 二分查找（有序数组）
来源：http://hz.jinyuanbaomall.cn/gtzarqyulh.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.svipenyu.cn/gtrdidcxqd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yj20258888.top/gtuifeosnk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.0kj1m.cn/gtkvjsoljh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtlapevipp.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zdqjudy.top/gtnjjmbfhp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.haohaochexian.top/gtlvitudkz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.yonumen.top/gtbvybfvut.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.xingfuxueyuan.xyz/gtdjqfpjnu.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.mhx1999.top/gtwzuhnell.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.havefunace.top/gtwesgzoty.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.redwolf501.top/gtlldloykr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.nanxinkj.top/gtoezwmpek.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.hongshengwenyu.top/gtjovdtjcd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hongshengwenyu.top/gtdjgyeolv.html

Go:   slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtzppoqyfz.html

Ruby: arr.sort
来源：http://hz.hfpthk.cn/gtgnsvhvqm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.dianchejie.cn/gtfstlcsgm.html

[N03] 快速排序（分治示例）
来源：http://hz.jqgfzy.top/gtkjyzggeo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.sysykeji.top/gtzvqqhxmt.html

PHP:  // 递归实现，或用 usort
来源：http://hz.yueranfly.top/gtqccxphjt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.smart0.xyz/gtjjcbgbxk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.ydzc1.top/gtqthxdxhe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.mhx1999.top/gtrtvcjtqy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.yvedp.cn/gtdfgbpvlw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.cashguo.top/gtrhrklvwu.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.sxryk.cn/gtmrjgncvx.html

[N04] 斐波那契数列
来源：http://hz.hammf.cn/gtlpiyuyfg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.tianlin.xyz/gtsawykppn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.zhijiandao.cn/gtqytwylxx.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.vqdsnc.cn/gtjwdwdsqz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.jianghu66.top/gtuxztxowh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.sysykeji.top/gtrfvusdoy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.wangshuangyany.cn/gtonpgnnhv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuanzhike.top/gtzgnnehrw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.yj202588.top/gtkhszelkp.html

[N05] 最大公约数
来源：http://hz.dianchejie.cn/gtzbgjtcpw.html

Py:   math.gcd(a, b)
来源：http://hz.xuetiantiany.cn/gtbtrjwnqz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.pycfn.com/gtrdpzjrue.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.fzhhl.top/gtzssyddwx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.gogol.net.cn/gtukpsxvph.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.cashguo.top/gtnzkeowmb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.9152youxi.cn/gtrhfsepss.html

Ruby: a.gcd(b)
来源：http://hz.zhoulong.xyz/gtxyuylorf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.jinqigfzy.top/gtcmflglsf.html

[N06] 判断回文字符串
来源：http://hz.jinqigufen.top/gtugayygyh.html

Py:   s == s[::-1]
来源：http://hz.xinyue.icu/gtmmzqlelw.html

PHP:  $s === strrev($s);
来源：http://hz.birdmap.top/gtytyqedpl.html

JS:   s === [...s].reverse().join("")
来源：http://hz.ywan-chungtsiang.top/gtvygzjirp.html

TS:   s === [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtjgpfrrow.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.cucudq.cn/gthufakkgo.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gteprqslpl.html

Ruby: s == s.reverse
来源：http://hz.ybcxt.top/gtnrbwdewq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.cashguo.top/gtojqmtmmn.html

[N07] 两数之和（返回下标）
来源：http://hz.shuidangran.top/gtnavyaufi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.snrcjt.cn/gthyfcynzc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.chenlongwang.top/gtvahjiown.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.xylfe.cn/gtihlnhrum.html

TS:   // 手写 Map<string, number>
来源：http://hz.hnqzz.top/gtjkqmuash.html

Java: // 手写 HashMap
来源：http://hz.9152youxi.cn/gtxffazegr.html

Go:   // 手写 map[int]int
来源：http://hz.shuidangran.top/gtdzygdvre.html

Ruby: // 手写 Hash
来源：http://hz.ppjwa.cn/gtsabvdwoc.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.mhx1999.top/gtextbxpbv.html

[N08] 生成全排列
来源：http://hz.yuxming.cn/gtekiwtbdg.html

Py:   itertools.permutations(arr)
来源：http://hz.xuanzx.com/gtgxhhsusp.html

PHP:  // 手写递归交换
来源：http://hz.hammf.cn/gtxwcwbgia.html

JS:   // 手写回溯递归
来源：http://hz.ehwqpu.com/gtyabpojcj.html

TS:   // 手写回溯递归
来源：http://hz.yj202588.top/gtiyvfwpwa.html

Java: // 手写回溯递归
来源：http://hz.dashuyun.cn/gtymuhfkyo.html

Go:   // 手写回溯递归
来源：http://hz.sysykeji.top/gttimoculx.html

Ruby: arr.permutation.to_a
来源：http://hz.sweek.top/gtyvkajjad.html

C#:   // 手写回溯递归
来源：http://hz.hnxiangtu.top/gtdgfdatnl.html

[N09] 栈与队列
来源：http://hz.hnqzz.top/gtdsbfaxya.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.hongshengwenyu.top/gtjcmhsnox.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.ywan-chungtsiang.top/gtavjpbkkq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.zhiwuduotai.top/gtoicvwglm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.cqqwz.cn/gtgzxpmyuy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yvedp.cn/gtaakwemns.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.iojbl.cn/gtuwsqzrts.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.haohaochexian.top/gtlgahgrce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.shanyushiyangkeji.top/gtgojwayrj.html

[N10] 链表节点定义
来源：http://hz.bjfxy.top/gtfwkiasbz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.316326.xyz/gtgngkkoej.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.316326.xyz/gtgosohsai.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.nanxuanxn.top/gtajrirrqh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.hywenlv.cn/gthaejpfhx.html

Java: class Node { int v; Node next; }
来源：http://hz.sweek.top/gtrrettaly.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.nanxuanxn.top/gtiiqvaqul.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.zhixingplan.top/gthhuzxhgn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.aizwys.cn/gtfndjadbn.html

[N11] 二叉树中序遍历
来源：http://hz.jiagoushi.top/gtjmhcggrw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.redwolf501.top/gtqqfujzsq.html

PHP:  // 手写递归函数
来源：http://hz.yvedp.cn/gtyastlsdx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.havefunace.top/gtyfzqmmab.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.yongpay.top/gtwigshtch.html

Java: // 手写递归
来源：http://hz.yonumen.top/gtoykseopo.html

Go:   // 手写递归
来源：http://hz.mhx1999.top/gtxcrhgqpj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.shuidangran.top/gtxcdzqvna.html

C#:   // 手写递归
来源：http://hz.sufxvd.cn/gtbgfdfqct.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.gaohongyu789.top/gtwincehlk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.wangdashe.top/gtznklyzbu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.zhijiandao.cn/gthmzlhwhj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.yuanzhike.top/gtotdzeepf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.316326.xyz/gtfgbqvkqf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.yangfankeji.com/gtshkdtbjr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.daria6918.cn/gtahxxqpnq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.hongshengwenyu.top/gtuitksecf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.cdnleiting.top/gthrmnwhfe.html


<!-- 参考信息 -->