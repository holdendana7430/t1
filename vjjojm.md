代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtfeqlulbi.html

[E11] 反转字符串
来源：http://hz.ybcxt.top/gtnnqcmvia.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtxytommds.html

PHP:  strrev($s);
来源：http://hz.jianghu66.top/gtamhznamt.html

JS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtwguzmhcs.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtjaisbboc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtvdvlsjyw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yangfankeji.com/gtnuyxinuk.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtehuywxhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtyqbcplbf.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtjszelhyq.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtowfsnpjo.html

PHP:  substr_count($s, "a");
来源：http://hz.tianlin.xyz/gtdeeenrqh.html

JS:   s.split("a").length - 1
来源：http://hz.daxiang520.top/gtsqecnrgo.html

TS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gtxpzwhdrl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.snrcjt.cn/gtggvdxced.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtynlxqjer.html

Ruby: s.count("a")
来源：http://hz.52xcode.cn/gteranqgqu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtyemrnvtd.html

[E13] 逐字符遍历
来源：http://hz.jyoumei.cn/gttvsmnjgn.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gtumblowka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenjidiqi.icu/gtihtuvyeh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtljyyfbsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gttgsszbrx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.0kj1m.cn/gtfkssoeyi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sweek.top/gtdscrnhjv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.kuanghao11.cn/gtwpqshzow.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gtlozgbvyc.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtcbjdtbop.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtczfmtwky.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gtuwjmguns.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.svipenyu.cn/gtsbysebhn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gogol.net.cn/gtlmqfakhy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ivvv.top/gtcjxhiwka.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.316326.xyz/gtvgszwksq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtyvqyjnyh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gtbsuswqxj.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhengqikj.top/gtqcoayyqk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtbjjzsuqm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtutwyacmb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtgfjscrkx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtjuxhizgq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gtjazmojxx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gteyamcsfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sysykeji.top/gterkbiwvf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtdthjqxkb.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtswjpuuqk.html

Py:   f"{1234567:,}"
来源：http://hz.daxiang520.top/gtacnekwul.html

PHP:  number_format(1234567);
来源：http://hz.yueranfly.top/gtecnmpoue.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtvjrjqfkm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtotmytwhc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtloyortsl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gtfzvbmhwm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtutjhstvd.html

C#:   1234567.ToString("N0")
来源：http://hz.redwolf501.top/gtlcgigary.html

[E17] 首字母大写
来源：http://hz.iojbl.cn/gtsswgmcxp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gthwgtxaca.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtrzcofqje.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gthuhactdt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhiwuduotai.top/gtfyzowjoq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinghuilouyu.cn/gtqrlrzqjg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.c1oappe.top/gttrnwgcfh.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtpngbxvkv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtcmwahdui.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtgczxdqhc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.svipenyu.cn/gtrqlvdshb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gtogfywlxa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtcnyjkchi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtwrikutfw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhijiandao.cn/gtxjcvsfsk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtbntysrni.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gtkzinouel.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxuanxn.top/gtajuexakn.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtbhlcgwsr.html

Py:   s.splitlines()
来源：http://hz.meibo888.top/gtsnshfdjt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hysaishi.cn/gtosmiagmz.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtogucfwrp.html

TS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtbwujoxdw.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtnlqndisb.html

Go:   strings.Split(s, "\n")
来源：http://hz.ybcxt.top/gtbidfvtoj.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtilvbuidl.html

C#:   s.Split('\n')
来源：http://hz.zhijiandao.cn/gtzqbrdphh.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtzfmsaljf.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtxafintsu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtzgzphsxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gtcsncssyz.html

TS:   if (s === "") {}
来源：http://hz.zhiwuduotai.top/gtmgvayesm.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gtlejjesxi.html

Go:   if s == "" {}
来源：http://hz.jinghuilouyu.cn/gtnrwhhjtk.html

Ruby: if s.empty?
来源：http://hz.0kj1m.cn/gtbdghbmin.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fengsongda.top/gtwhvcimqm.html

[E21] 超长截断加省略号
来源：http://hz.cdnleiting.top/gtiytanhig.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtfhbwyhdz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ybcxt.top/gthqwqzyno.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtfrzknxiu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gtjudknkak.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtnvgidjfh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtavcfuomz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtjdwccuxv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.birdmap.top/gtdszztwky.html

[E22] 字节长度与字符长度
来源：http://hz.shanyushiyangkeji.top/gtqyhxxlpl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gaohongyu789.top/gtodsxdlbb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtavnjqnqx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtklgryjhm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtjvgzjygu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xuetiantiany.cn/gtionjhzwt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yongpay.top/gtqsgcktws.html

Ruby: s.bytesize;  s.length
来源：http://hz.ivvv.top/gtklpnwcak.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtgcwkdpjd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtbmmpwdgg.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtjsoypbeb.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwvoorzrk.html

[F01] 读取整个文件
来源：http://hz.jqgfzy.top/gtefzhwuqn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtofujnbov.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtqhozgcvf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtsgwhmvkh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sxryk.cn/gtbpjauyus.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtnyvtijxx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hnxiangtu.top/gtvqlybjlo.html

Ruby: File.read("a.txt")
来源：http://hz.chenlongwang.top/gtrcoanbdy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xylfe.cn/gttrijtfpn.html

[F02] 逐行读取文件
来源：http://hz.cqqwz.cn/gtbqajxtxo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gttswkuelj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.nanxuanxn.top/gtnbamrwuh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtlmbvumnv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtjlpekzcl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtoqugwtmw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gttvqephvw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sweek.top/gtsifgecak.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.aibaodan.cn/gtzrqpohlw.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtkthzfyob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnqzz.top/gtstzekjij.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.guowangkeji.top/gtmtbylolr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtdievgopy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtkgwwuhts.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinghuilouyu.cn/gtsnjilsft.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtbcenzmsj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtwmnjpoqq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtpvekvtrk.html

[F04] 追加写入文件
来源：http://hz.shangyingyoupin.top/gtzhwvevnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guannengcc.top/gtynwboicb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sysykeji.top/gtgetgeiny.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtzgsdkufz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtqyzdgjar.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gtlsiqajko.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cashguo.top/gtkhfkforr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nwbrower.top/gtlhoalooz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenjidiqi.icu/gtuuuicfpn.html

[F05] 判断文件或目录是否存在
来源：http://hz.xylfe.cn/gtutjvdodi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtwqlemudl.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtcuayihah.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cqqwz.cn/gthfingfzv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ybcxt.top/gtzszvoyfp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtkfmcrimv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shzxlz.cn/gtdcnlfcam.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gtkyswiekg.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gtwgmzeanf.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtcuziciet.html

Py:   os.remove("a.txt")
来源：http://hz.vqdsnc.cn/gtenqypbpx.html

PHP:  unlink("a.txt");
来源：http://hz.jiagoushi.top/gtlqnblxxu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtjyaxxpqa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtqudglfwg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtizywvofj.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtmulwuwks.html

Ruby: File.delete("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjuxabffk.html

C#:   File.Delete("a.txt");
来源：http://hz.ywan-chungtsiang.top/gteyglwhir.html

[F07] 创建目录（含多级）
来源：http://hz.yuanzhike.top/gthucxaeeh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtzlanuuhy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ehwqpu.com/gtejdscots.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtosobfqvj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtpaxzcong.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.smart0.xyz/gtnvoyysrk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtzkglfopw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenzaomai.com/gtvjuijyre.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guannengcc.top/gtajzpprug.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtqxcfzxfd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ybcxt.top/gtrohubkze.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jianghu66.top/gtzppcfnzq.html

JS:   fs.readdirSync("dir")
来源：http://hz.9152youxi.cn/gtdmdbvqli.html

TS:   fs.readdirSync("dir")
来源：http://hz.haohaochexian.top/gttjsmahzs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtljkihcqk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtihedwbaj.html

Ruby: Dir.children("dir")
来源：http://hz.yuxming.cn/gtlepmjgxx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.svipenyu.cn/gtvftwdljl.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtajsirvgc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtnhxoqbvn.html

PHP:  filesize("a.txt");
来源：http://hz.zhongyouzk.top/gtewpujryw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtlsnxvden.html

TS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtqyhnqgmx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtimazgpsi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtoxxeiemk.html

Ruby: File.size("a.txt")
来源：http://hz.quarkkingdee.top/gtyprtafhu.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtflgsbsuc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gthkicaolp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtgwvijxcn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xuetiantiany.cn/gtwnvydshg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daxiang520.top/gtxiwdtocw.html

TS:   path.extname("a.txt")
来源：http://hz.hnqzz.top/gtvvaozpjd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhixingplan.top/gtwrjogpvb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtcmlrhggt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.316326.xyz/gtidjzdgdz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zdqjudy.top/gtnylglngs.html

[F11] 复制与移动文件
来源：http://hz.daria6918.cn/gtkmytmatv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtfxteiajs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hysaishi.cn/gtidemvxxe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtychsklkr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtfrkrpduy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtchzycznd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.iojbl.cn/gtxkkeqgtr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtnqnnnhqm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtmxvqdksc.html

[F12] CSV 读写
来源：http://hz.gaohongyu789.top/gtanbqcxsn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.vqdsnc.cn/gtloayrvij.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.aizwys.cn/gtkyrampzb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gttjmbsjmu.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtkpmknmef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtyynfgnpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtkhgkkuun.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dianchejie.cn/gtkgtzgpge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zycfv.cn/gtjjoawdel.html

================================================================================
来源：http://hz.daxiang520.top/gtpfegwnzw.html

G. 面向对象
来源：http://hz.316326.xyz/gtzqgxksfg.html

================================================================================
来源：http://hz.yvedp.cn/gtcmwwdsuo.html

[G01] 定义类
来源：http://hz.hnxiangtu.top/gtcvrxkmft.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtulooxxqz.html

PHP:  class User {}
来源：http://hz.ivvv.top/gtrqlvnxzf.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtkmeqyjzh.html

TS:   class User { name: string = ""; }
来源：http://hz.jinghuilouyu.cn/gtnfuuijrp.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtfvcqjabe.html

Go:   type User struct { Name string }
来源：http://hz.hysaishi.cn/gtwzmxpoiy.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtfjaexfni.html

C#:   class User {}
来源：http://hz.tian-w.cn/gtrfcaqkih.html

[G02] 构造函数
来源：http://hz.zhaomingkeji.xyz/gtjhzyuxvd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cashguo.top/gtszfgffdc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.pycfn.com/gteyqgpiwr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.52xcode.cn/gtaxrfwttu.html

TS:   constructor(public name: string) {}
来源：http://hz.zhengqikj.top/gtxqstevby.html

Java: User(String name) { this.name = name; }
来源：http://hz.svipenyu.cn/gtgjpvzrhl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtvhgavbtb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtcfchilnx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gogol.net.cn/gthnxodpmi.html

[G03] 实例属性
来源：http://hz.zdqjudy.top/gtxwwphscy.html

Py:   self.name = "x"
来源：http://hz.zhijiandao.cn/gtewdlkpgm.html

PHP:  public string $name = "x";
来源：http://hz.yangfankeji.com/gtcwygsyzm.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtwlxfhkiw.html

TS:   name: string = "x";
来源：http://hz.mhx1999.top/gtnihgpbho.html

Java: private String name;
来源：http://hz.nanxinkj.top/gtvzhncugd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.chenzaomai.com/gtyzdypzyr.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtvuraxwld.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cashguo.top/gtjjrovqjv.html

[G04] 定义方法
来源：http://hz.jinqigfzy.top/gtactaoihs.html

Py:   def greet(self): return self.name
来源：http://hz.ehwqpu.com/gtavhqylui.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtusspbbmn.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtligdzvsi.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtgazhhvtu.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gtvlcditxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xinyue.icu/gtbxpmpwhk.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtpuvmwlxb.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtjumcyubt.html

[G05] 继承
来源：http://hz.ydzc1.top/gtgawfcogg.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtotjdxaoe.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtgowpoiuk.html

JS:   class Admin extends User {}
来源：http://hz.cheryme.top/gtcjnemdfi.html

TS:   class Admin extends User {}
来源：http://hz.cdnleiting.top/gtkmnxizzq.html

Java: class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtatzyetwb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.redwolf501.top/gtjrcibmfa.html

Ruby: class Admin < User; end
来源：http://hz.cucudq.cn/gtvrxycuca.html

C#:   class Admin : User {}
来源：http://hz.zhengqikj.top/gtovwlhjff.html

[G06] 重写方法
来源：http://hz.iojbl.cn/gtdyfpvntg.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigfzy.top/gtdilmcusf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtvimkpnpq.html

JS:   greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtpchzynws.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtpaktpwbm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtbklvylug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shzxlz.cn/gtifegqduy.html

Ruby: def greet; "admin"; end
来源：http://hz.jiagoushi.top/gtbywaupoh.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtyjirwcuh.html

[G07] 调用父类方法
来源：http://hz.hnqzz.top/gtgyaoatda.html

Py:   super().greet()
来源：http://hz.hfpthk.cn/gtyduuokkn.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtxfjzbzgi.html

JS:   super.greet();
来源：http://hz.shanyushiyangkeji.top/gtysxqzazp.html

TS:   super.greet();
来源：http://hz.mhx1999.top/gtkpccpgzb.html

Java: super.greet();
来源：http://hz.52xcode.cn/gtptevakfr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gtyfrjunju.html

Ruby: super
来源：http://hz.chenlongwang.top/gtzsnpwucl.html

C#:   base.Greet();
来源：http://hz.jlsjyb.cn/gtbkvaampb.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtcefrgtmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhongyouzk.top/gtqiwrslbx.html

PHP:  public static function f() {}
来源：http://hz.yj20258.top/gtfofwkecn.html

JS:   static f() {}
来源：http://hz.havefunace.top/gtpxaolypl.html

TS:   static f(): void {}
来源：http://hz.sweek.top/gtkbewkcxu.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gtmzwwyhjr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nwbrower.top/gtertezpiv.html

Ruby: def self.f; end
来源：http://hz.ivvv.top/gtdxocdurz.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtroydzxlk.html

[G09] 接口 / 抽象类
来源：http://hz.jlsjyb.cn/gtioosqgpf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtdkftdyll.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.haohaochexian.top/gtmoadjoxf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtslzguxux.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtdwldwymn.html


<!-- 参考信息 -->