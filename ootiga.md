代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtbzhpcsjp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtuuxyriqq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtnyzhowmh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtwkflycod.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jqgufenzy.top/gtesxlhxyt.html

[K07] 进制转换
来源：http://hz.yueranfly.top/gtokgceglg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtoodcxwyz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sxryk.cn/gtolwuskwu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtyhuttwwm.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtuswmvdnj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtncdanenb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sxryk.cn/gtwmduvjec.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cashguo.top/gtuuqvqpjs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hfpthk.cn/gtzxmjypao.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nanxinkj.top/gthkyihafi.html

Py:   pickle.dumps(obj)
来源：http://hz.shzxlz.cn/gtahpaozpo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtyzzhpmou.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenlongwang.top/gtycsdvhyj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtcvcsbvru.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sufxvd.cn/gtaxaymnte.html

Go:   encoding/gob
来源：http://hz.c1oappe.top/gtpsfilnyp.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtfbjfwrwi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinyuanbaomall.cn/gtqciomnzv.html

================================================================================
来源：http://hz.yueranfly.top/gtzzhzczsy.html

L. 网络请求
来源：http://hz.daxiang520.top/gtnfeyttag.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkkmzmmne.html

[L01] 发送 GET 请求
来源：http://hz.sufxvd.cn/gtfimzpdds.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtqrgbiyqq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gtwipzlcnr.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtbbsplqfl.html

TS:   await fetch(url)
来源：http://hz.jinqigfzy.top/gtpwlafueb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.guowangkeji.top/gtplrzkfrg.html

Go:   resp, err := http.Get(url)
来源：http://hz.bjfxy.top/gttquhylhh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xinyue.icu/gtwzvhecqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.mhx1999.top/gtuyvkaeov.html

[L02] 发送 POST JSON
来源：http://hz.andypj.xyz/gtgybzzyso.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hammf.cn/gtkccskoxg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.daria6918.cn/gtcqoarblr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtowxmqgbr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtotxadrgc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtagnlgyxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jinqigfzy.top/gtfuhkuntv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gotoacloud.top/gttmezzbmo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hysaishi.cn/gtygzmxrry.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtfnmjeryp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtnzkhalkx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtvxsrqulg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtjhjilknv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.daria6918.cn/gtumcqtolb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zdqjudy.top/gtnbpozkyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtwecdvagl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.bjfxy.top/gtrtybtxrd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hnxiangtu.top/gtragvgmol.html

[L04] 设置超时
来源：http://hz.redwolf501.top/gtdzygnavi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgfzy.top/gtlrfzmedb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ywan-chungtsiang.top/gtdatspuqp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtvyjkxcmt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtmfnpnofk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.svipenyu.cn/gtxtyqrwah.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtdcldevmu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.gaohongyu789.top/gtcsfprezn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gogol.net.cn/gtartlaqug.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtzbocdxmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.pengpengdd.cyou/gtdxgqwhqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gotoacloud.top/gtrtoarczl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtfyycqnjl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.sweek.top/gtbludlzha.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gttreryumc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ydjk.org.cn/gtaftlkwav.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.cqqwz.cn/gtsrphtzsd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gtnlgzcaew.html

[L06] 解析响应为 JSON
来源：http://hz.pycfn.com/gtqqxwbpdr.html

Py:   resp.json()
来源：http://hz.wangdashe.top/gtrfkwpcfm.html

PHP:  json_decode($body, true);
来源：http://hz.fzhhl.top/gtcyrgrqbh.html

JS:   await resp.json()
来源：http://hz.hnqzz.top/gtnuyhpfgm.html

TS:   await resp.json()
来源：http://hz.yueranfly.top/gtknwsrpzf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhongyouzk.top/gtsxdfkdjg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ywan-chungtsiang.top/gtpwukwexj.html

Ruby: JSON.parse(resp.body)
来源：http://hz.sweek.top/gtroezwnhx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hammf.cn/gtnqfkfavh.html

[L07] 处理 HTTP 状态码
来源：http://hz.yonumen.top/gtarhtttjb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xinyue.icu/gtvkendwtn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtytysfwgu.html

JS:   resp.ok;  resp.status
来源：http://hz.gzhubu.top/gtcpzqotsm.html

TS:   resp.ok;  resp.status
来源：http://hz.sufxvd.cn/gtbbrirvvp.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtbloespud.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtfcofazft.html

Ruby: resp.code.to_i
来源：http://hz.dianchejie.cn/gtpxggelmh.html

C#:   (int)resp.StatusCode
来源：http://hz.xuanzx.com/gtnbegedvm.html

[L08] 并发请求多个地址
来源：http://hz.nwbrower.top/gtktgqlzmg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gtzwoqqwmm.html

PHP:  curl_multi_init() 系列
来源：http://hz.wangdashe.top/gtjvzehdgp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.pengpengdd.cyou/gthwafyced.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.dianchejie.cn/gthtnzlmvl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.vqdsnc.cn/gtonxqmwjh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sysykeji.top/gtmyragydq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ppjwa.cn/gtkrneqxos.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtudugfmuq.html

================================================================================
来源：http://hz.bjfxy.top/gtfcclbdcs.html

M. 命令行 / 进程 / 环境
来源：http://hz.hysaishi.cn/gttcaxzwtb.html

================================================================================
来源：http://hz.birdmap.top/gtenltywua.html

[M01] 读取命令行参数
来源：http://hz.tianlin.xyz/gtaweejrqb.html

Py:   sys.argv[1:]
来源：http://hz.zhiwuduotai.top/gtttwksckl.html

PHP:  $argv;  $argc;
来源：http://hz.guowangkeji.top/gtqtowilmw.html

JS:   process.argv.slice(2)
来源：http://hz.cheryme.top/gtotzdysak.html

TS:   process.argv.slice(2)
来源：http://hz.dashuyun.cn/gtmknqvgxs.html

Java: args 数组（main 方法参数）
来源：http://hz.aibaodan.cn/gtjgposzwt.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gtcrapbzfx.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtomwpjupl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xylfe.cn/gtvmufhvrt.html

[M02] 读取环境变量
来源：http://hz.zhiwuduotai.top/gtmkjfhjti.html

Py:   os.environ.get("HOME")
来源：http://hz.hfpthk.cn/gtsfgrqwvd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtdukqznln.html

JS:   process.env.HOME
来源：http://hz.hnqzz.top/gtkbpzrwgd.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtvttqrzyb.html

Java: System.getenv("HOME")
来源：http://hz.gogol.net.cn/gtuyfcimyg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.gzhubu.top/gteyrvkrwj.html

Ruby: ENV["HOME"]
来源：http://hz.yj202588.top/gtzetkqpcu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gthcaqrgxp.html

[M03] 执行外部命令
来源：http://hz.xylfe.cn/gtrzzzauhm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhijiandao.cn/gtwkeoluya.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.nwbrower.top/gthxmtowqx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gteobdlgli.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.kuanghao11.cn/gtnjfpwmea.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.iojbl.cn/gtyixevglw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.yuxming.cn/gtzivzilbk.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.bjfxy.top/gtieszqztu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.mhx1999.top/gtuzugwdod.html

[M04] 获取当前工作目录
来源：http://hz.chenlongwang.top/gthxfnbxnx.html

Py:   os.getcwd()
来源：http://hz.haohaochexian.top/gtbgybplsw.html

PHP:  getcwd();
来源：http://hz.jinghuilouyu.cn/gttselxmls.html

JS:   process.cwd()
来源：http://hz.feifeiyinyue.top/gtjrbuugdh.html

TS:   process.cwd()
来源：http://hz.wangdashe.top/gtbqtxkxbs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ivvv.top/gtcghbhjhv.html

Go:   os.Getwd()
来源：http://hz.zhixingplan.top/gtarlzxiyk.html

Ruby: Dir.pwd
来源：http://hz.wangshuangyany.cn/gtdudhwxti.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.quarkkingdee.top/gthojdgjra.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gttvpbbupb.html

Py:   sys.exit(1)
来源：http://hz.ehwqpu.com/gtjxkdswzn.html

PHP:  exit(1);
来源：http://hz.sweek.top/gtdkuqlmuz.html

JS:   process.exit(1)
来源：http://hz.birdmap.top/gtprfpkmrn.html

TS:   process.exit(1)
来源：http://hz.iojbl.cn/gtkgeevucv.html

Java: System.exit(1)
来源：http://hz.yvedp.cn/gtyxrglapn.html

Go:   os.Exit(1)
来源：http://hz.shuidangran.top/gtpnisjyuh.html

Ruby: exit 1
来源：http://hz.shzxlz.cn/gtbgjfhicj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.redwolf501.top/gtptjqpoga.html

[M06] 向标准错误输出
来源：http://hz.ivvv.top/gtcguihybf.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nanxinkj.top/gtfxgvydec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.shzxlz.cn/gtybqucyyi.html

JS:   console.error("err")
来源：http://hz.zhixingplan.top/gtlaffscwj.html

TS:   console.error("err")
来源：http://hz.svipenyu.cn/gtakuhnrxo.html

Java: System.err.println("err")
来源：http://hz.cdnleiting.top/gtxptvxtte.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.tianlin.xyz/gtnjudtcjg.html

Ruby: warn "err"
来源：http://hz.ppjwa.cn/gtfoymdpqm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yuxming.cn/gtojrpgfrf.html

[M07] 判断是否为主入口
来源：http://hz.sweek.top/gtblytjqwl.html

Py:   if __name__ == "__main__":
来源：http://hz.xylfe.cn/gtpgwudpmw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtxchqumao.html

JS:   require.main === module
来源：http://hz.hongshengwenyu.top/gtqceunbcl.html

TS:   require.main === module
来源：http://hz.zhixingplan.top/gtujtsctsv.html

Java: public static void main(String[] args)
来源：http://hz.jqgufenzy.top/gtgkhideps.html

Go:   func main()
来源：http://hz.yuxming.cn/gtnumjiyjj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtfkjgwdqw.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtmbmrwvsv.html

[M08] 获取系统与运行时信息
来源：http://hz.zhaomingkeji.xyz/gtbwhqlwrq.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhongyouzk.top/gtjvvddpce.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cucudq.cn/gthnayigzw.html

JS:   process.platform;  process.version
来源：http://hz.jinghuilouyu.cn/gtwionttqn.html

TS:   process.platform;  process.version
来源：http://hz.hysaishi.cn/gtgqfkfxad.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.feifeiyinyue.top/gtxychodif.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.jinqigfzy.top/gtigqqzpsl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.redwolf501.top/gtoivoehvt.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yvedp.cn/gtpyvhvtyh.html

================================================================================
来源：http://hz.xinyue.icu/gtaeddjqof.html

N. 数据结构与算法
来源：http://hz.meibo888.top/gtwxzwcdjq.html

================================================================================
来源：http://hz.mhx1999.top/gtngdfaygq.html

[N01] 二分查找（有序数组）
来源：http://hz.gogol.net.cn/gtkvhcvfqj.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zycfv.cn/gtzxvgpiyz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.bjfxy.top/gtjypszquo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtmepfbdek.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.xuetiantiany.cn/gtzmnxjdus.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.aibaodan.cn/gtagpcbzqf.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.nanxinkj.top/gtvensvvig.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.snrcjt.cn/gtointpenz.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.sufxvd.cn/gtfotclfxo.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.cucudq.cn/gtsmutluss.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.quarkkingdee.top/gtrjnbalvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.ppjwa.cn/gtejbbjgte.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.zhongyouzk.top/gtscakquuj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.mhx1999.top/gtanwlvawk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.ydzc1.top/gtiemlyehx.html

Go:   slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtswxnvpcv.html

Ruby: arr.sort
来源：http://hz.52xcode.cn/gtiyjaqoqz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.guowangkeji.top/gtzwfnyrmt.html

[N03] 快速排序（分治示例）
来源：http://hz.sxryk.cn/gtzscldozv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.fengsongda.top/gtawjkcper.html

PHP:  // 递归实现，或用 usort
来源：http://hz.zhongyouzk.top/gtnuyzveip.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.tian-w.cn/gtusfrmrhg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hz.shzxlz.cn/gtziiftwxm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hz.jinqigufen.top/gtdjmfdcxn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hz.cashguo.top/gtmtmghmcm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hz.dashuyun.cn/gtvmdglbtb.html

C#:   // 手写递归，或 Array.Sort
来源：http://hz.shuidangran.top/gtcqmaihrc.html

[N04] 斐波那契数列
来源：http://hz.pycfn.com/gtmrjlkxpu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtnvtuiiyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hz.svipenyu.cn/gtnexobpul.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.zhaomingkeji.xyz/gtrfxfiplp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hz.xylfe.cn/gtscbvwjnh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hz.xinyue.icu/gtxnwcgklk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hz.hnxiangtu.top/gticioulpo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hz.yuxming.cn/gtphcarxtr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hz.smart0.xyz/gtcuwzoobq.html

[N05] 最大公约数
来源：http://hz.jyoumei.cn/gtxzobviit.html

Py:   math.gcd(a, b)
来源：http://hz.dashuyun.cn/gtnpgwvneq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hz.jinqigfzy.top/gtqxqqufln.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.xuanzx.com/gtefygtzok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hz.cqqwz.cn/gtcpmpgwqs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hz.ppjwa.cn/gtmxztcgrv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hz.sweek.top/gtzzzfowbe.html

Ruby: a.gcd(b)
来源：http://hz.jinghuilouyu.cn/gtoqxxhkxx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hz.zhaomingkeji.xyz/gtpgrwxbbi.html

[N06] 判断回文字符串
来源：http://hz.yvedp.cn/gtypcdcjlf.html

Py:   s == s[::-1]
来源：http://hz.ehwqpu.com/gttysqpycl.html

PHP:  $s === strrev($s);
来源：http://hz.sufxvd.cn/gtnaqiupfi.html

JS:   s === [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtecfloiri.html

TS:   s === [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtfbeyjlkk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hz.zycfv.cn/gtfpaklwwq.html

Go:   // 双指针从两端比较
来源：http://hz.zdqjudy.top/gtqpwajyah.html

Ruby: s == s.reverse
来源：http://hz.jqgfzy.top/gtbzsbzkrg.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://hz.0kj1m.cn/gtgqhfzies.html

[N07] 两数之和（返回下标）
来源：http://hz.yueranfly.top/gtusrkmbqt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hz.316326.xyz/gtbwctauus.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hz.shangyingyoupin.top/gtpoynsqhk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://hz.nanxinkj.top/gtklbopmfj.html

TS:   // 手写 Map<string, number>
来源：http://hz.xingfuxueyuan.xyz/gtsbocccgg.html

Java: // 手写 HashMap
来源：http://hz.hfpthk.cn/gtxltihkvk.html

Go:   // 手写 map[int]int
来源：http://hz.cheryme.top/gtnpncmzqf.html

Ruby: // 手写 Hash
来源：http://hz.c1oappe.top/gtqdubghil.html

C#:   // 手写 Dictionary<int, int>
来源：http://hz.52xcode.cn/gtnifkaegj.html

[N08] 生成全排列
来源：http://hz.hnqzz.top/gtrkroqjkc.html

Py:   itertools.permutations(arr)
来源：http://hz.zhijiandao.cn/gtynhqlvxu.html

PHP:  // 手写递归交换
来源：http://hz.gogol.net.cn/gtqfskzjtj.html

JS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtrcfpvmhi.html

TS:   // 手写回溯递归
来源：http://hz.fengsongda.top/gtconujuem.html

Java: // 手写回溯递归
来源：http://hz.zdqjudy.top/gtlmfjyrwc.html

Go:   // 手写回溯递归
来源：http://hz.xylfe.cn/gtpcxvgsgm.html

Ruby: arr.permutation.to_a
来源：http://hz.sysykeji.top/gtvjqmxxvd.html

C#:   // 手写回溯递归
来源：http://hz.gzhubu.top/gtjhxozpet.html

[N09] 栈与队列
来源：http://hz.yongpay.top/gtzqocckmf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hz.zhijiandao.cn/gtvifzzlpj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hz.hywenlv.cn/gtzfuwqpye.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hz.gotoacloud.top/gtwdgmphju.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hz.jlsjyb.cn/gtovqwqlwq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hz.yuanzhike.top/gtiytxrjge.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hz.pycfn.com/gtpgiazeqy.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hz.shanyushiyangkeji.top/gtocrnibty.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hz.yongpay.top/gtedczlwaf.html

[N10] 链表节点定义
来源：http://hz.jqgufenzy.top/gtzhbfswgm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hz.zycfv.cn/gtorbebafh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://hz.hnqzz.top/gtmzndvese.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hz.cqqwz.cn/gtfrrzyvch.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hz.ydjk.org.cn/gtfhlqsnwx.html

Java: class Node { int v; Node next; }
来源：http://hz.jianghu66.top/gthhikhmtb.html

Go:   type Node struct { V int; Next *Node }
来源：http://hz.dianchejie.cn/gtcxlcuaxx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://hz.shanyushiyangtech.top/gtninhlljk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://hz.gotoacloud.top/gtjcamtpwa.html

[N11] 二叉树中序遍历
来源：http://hz.zhiwuduotai.top/gtxezokkzj.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hz.sweek.top/gtrzcprybj.html

PHP:  // 手写递归函数
来源：http://hz.nanxinkj.top/gtorjqtsnl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.zycfv.cn/gtgwygsuwr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hz.bjfxy.top/gtvtxzbhao.html

Java: // 手写递归
来源：http://hz.sxryk.cn/gtdquyhwya.html

Go:   // 手写递归
来源：http://hz.cucudq.cn/gtyhvxuepx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hz.c1oappe.top/gtaomuxafc.html

C#:   // 手写递归
来源：http://hz.havefunace.top/gtuyyfvqyl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hz.yvedp.cn/gthkhquarb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hz.andypj.xyz/gtctznyzzq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hz.iojbl.cn/gthnnifwmi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.ehwqpu.com/gthtigwhkt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hz.birdmap.top/gtrnyihspg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.9152youxi.cn/gtjtlmhlpa.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hz.snrcjt.cn/gtxkewdczw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hz.jianghu66.top/gtaukqueeu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hz.redwolf501.top/gtfgiifwas.html

================================================================================
来源：http://hz.zdqjudy.top/gtdwtuwgxy.html

O. 并发与异步
来源：http://hz.xinyue.icu/gtjlmmktdh.html

================================================================================
来源：http://hz.ppjwa.cn/gtggnwpiol.html

[O01] 启动一个线程
来源：http://hz.9152youxi.cn/gtcsncooxb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hz.sufxvd.cn/gtvmwvfrxp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hz.c1oappe.top/gtdukciaid.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hz.cqqwz.cn/gtqegyaxsc.html

TS:   // 同 JS
来源：http://hz.shangyingyoupin.top/gthiqjnjxl.html

Java: new Thread(() -> f()).start()
来源：http://hz.dianchejie.cn/gtgmgexklg.html

Go:   go f()
来源：http://hz.guowangkeji.top/gtbqkisgpq.html

Ruby: Thread.new { f }
来源：http://hz.gogol.net.cn/gttuoyytiv.html

C#:   Task.Run(() => F());
来源：http://hz.gzhubu.top/gttuyhaajm.html

[O02] 使用线程池
来源：http://hz.fengsongda.top/gtaysjodao.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hz.cucudq.cn/gtpbrvwvwf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hz.jqgufenzy.top/gtylbnceoq.html

JS:   // worker_threads 线程池
来源：http://hz.tanke756.top/gtgalizbgx.html


<!-- 参考信息 -->