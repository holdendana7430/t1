代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.xylfe.cn/gthxpfzybo.html

Ruby: items.join(",")
来源：http://hz.52xcode.cn/gtkpxxxrrd.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtlxdnnjac.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtvcrjqunz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigufen.top/gtzitkayoq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hfpthk.cn/gteocmxiku.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtisuunkyj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtwkhzjlzu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.kuanghao11.cn/gtjcijfgyn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtgmmslxyt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhongyouzk.top/gthhkovjpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gtxklfvrkp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtptptcicm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtnavxaksl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangkeji.top/gtbwkdjhiu.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxuanxn.top/gtzncwdhln.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtptfmsski.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtztnkxyzu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hywenlv.cn/gtmnvhkgwr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtqvpkfolg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtarzsgijq.html

[E11] 反转字符串
来源：http://hz.chenjidiqi.icu/gtebmczoqe.html

Py:   s[::-1]
来源：http://hz.chenzaomai.com/gtyapkpyio.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtgprqkbsn.html

JS:   [...s].reverse().join("")
来源：http://hz.xylfe.cn/gtwleltkor.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtnelqafyg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gtcxwfoawz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dianchejie.cn/gtkvierrup.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtcvnvdwrk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gzhubu.top/gtbjwicets.html

[E12] 统计某字符出现次数
来源：http://hz.yueranfly.top/gtxtjfmxwz.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtwxbidfmh.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtuzsttokz.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtvhvvcurw.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gtrptlaxmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.meibo888.top/gttxqdkexo.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtwjotzyuy.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtvxdtdmoj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tianlin.xyz/gtmhrmpmkr.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtnmbfajub.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtvzniddhi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cucudq.cn/gtkkwqkydu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgfzy.top/gtaryozquw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aizwys.cn/gtdizwnuxa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hysaishi.cn/gtoonhggju.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hammf.cn/gtiiriexqq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.andypj.xyz/gtfvynjgib.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xziqi.cn/gtcfyexqbw.html

[E14] URL 编码与 Base64
来源：http://hz.xinyue.icu/gtfahbyraw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtuyzgzqto.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cqqwz.cn/gtimvegees.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pengpengdd.cyou/gtgojqufej.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gttzgbpwtp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gttstqscth.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.dianchejie.cn/gtpwluxzpb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtuofkcplk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ywan-chungtsiang.top/gthfihnfnv.html

[E15] HTML 转义 / 反转义
来源：http://hz.kuanghao11.cn/gtwuqaqxhy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtdlxrwpmq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtxzqukual.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sysykeji.top/gtiincrlby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtrgoixlpr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.quarkkingdee.top/gtpyuydwvr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtwwyohvjh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtlkgrxkxf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.havefunace.top/gtexbpsoay.html

[E16] 数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtlddybbog.html

Py:   f"{1234567:,}"
来源：http://hz.chenzaomai.com/gtkeahslxv.html

PHP:  number_format(1234567);
来源：http://hz.xinyue.icu/gtuphypenx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.feifeiyinyue.top/gtthcellur.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtxoesxtek.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aibaodan.cn/gtwdkubtli.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtkdtcwpav.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtmmyrspej.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtgwtdgkgw.html

[E17] 首字母大写
来源：http://hz.shangyingyoupin.top/gtiopbowmj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtorippcft.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pycfn.com/gtqzqpxjxz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtxnpzbrgp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtzkinqdsc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtsnhekqsz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtpepwbget.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtiobgamxi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtbzyonjvq.html

[E18] 模板占位符替换
来源：http://hz.xziqi.cn/gtscagbdvc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtyzdnuump.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hfpthk.cn/gtkbgqojji.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.redwolf501.top/gtydqutkru.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtgfqzsoxx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.316326.xyz/gtinizbvhi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tian-w.cn/gtwpdlzexj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gttrotplty.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shangyingyoupin.top/gtkydwbrkn.html

[E19] 多行文本按行拆分
来源：http://hz.zhongyouzk.top/gtdsydabhd.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangtech.top/gtajvxsddf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ivvv.top/gtgplgtrrm.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtisfyyoct.html

TS:   s.split(/\r?\n/)
来源：http://hz.gotoacloud.top/gtutowdqmp.html

Java: s.lines().toList()
来源：http://hz.snrcjt.cn/gtqldkucjc.html

Go:   strings.Split(s, "\n")
来源：http://hz.wangdashe.top/gtfbywospz.html

Ruby: s.lines
来源：http://hz.ppjwa.cn/gtrtejukkd.html

C#:   s.Split('\n')
来源：http://hz.jinghuilouyu.cn/gtdwleieev.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gttagzeufs.html

Py:   if not s:
来源：http://hz.hammf.cn/gtfuplhlsx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.vqdsnc.cn/gtwpyutyom.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhengqikj.top/gtzmlflcdx.html

TS:   if (s === "") {}
来源：http://hz.fzhhl.top/gttisezrza.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gtmwuwjtzq.html

Go:   if s == "" {}
来源：http://hz.hnxiangtu.top/gtcoxtpslh.html

Ruby: if s.empty?
来源：http://hz.snrcjt.cn/gtvvhyzbin.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.iojbl.cn/gtubvcheta.html

[E21] 超长截断加省略号
来源：http://hz.shuidangran.top/gtvszofdkj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj20258.top/gtyngnumfp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.redwolf501.top/gttmmouqtz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtvrvdrldm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jianghu66.top/gtuvbmutsd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtwvptjybw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtneatmmra.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.52xcode.cn/gtaqwwpihv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtduiffkwr.html

[E22] 字节长度与字符长度
来源：http://hz.ehwqpu.com/gteszuopig.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtczdounyf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtozkadfkr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtuhzopves.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigufen.top/gtjblktxyl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gthzctemjt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fzhhl.top/gtlvypvotd.html

Ruby: s.bytesize;  s.length
来源：http://hz.52xcode.cn/gtddnozkqe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.smart0.xyz/gtnpxkmpxo.html

================================================================================
来源：http://hz.andypj.xyz/gtjsijykwk.html

F. 文件与目录
来源：http://hz.ywan-chungtsiang.top/gtcgcbiwiv.html

================================================================================
来源：http://hz.jqgfzy.top/gtmfojgohr.html

[F01] 读取整个文件
来源：http://hz.guannengcc.top/gtdjueqrfa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtqevkqpjh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xuetiantiany.cn/gtubgstrfs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuxming.cn/gthzguiall.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ehwqpu.com/gtrcjytzvf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtrfjvugmj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtkdttwdki.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtzorfkqia.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtkcorkcfg.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtmvvahhme.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xylfe.cn/gtnqovdxho.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shuidangran.top/gtwjnneeuw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtewowjcie.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtlbfkwjnr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtxfsrldlo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtennngzuw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtgwwdtmgu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangshuangyany.cn/gtevjssezp.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtrvizkwsr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtelktdxwd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtpmilmqmo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtxyvxmcjn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtomamhnly.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtamsyuxhk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yonumen.top/gtlafgqgyj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtnzgtlhtb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuxming.cn/gtndufksfh.html

[F04] 追加写入文件
来源：http://hz.sweek.top/gtnrnohvqd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sweek.top/gtdgrjvqbz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jianghu66.top/gtgkugqcfd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtwqoydtse.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.svipenyu.cn/gtqbojndjh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gtjcegvvhs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.snrcjt.cn/gtefefoudl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shangyingyoupin.top/gtlqrgpknz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.redwolf501.top/gtvfdtfhkk.html

[F05] 判断文件或目录是否存在
来源：http://hz.hongshengwenyu.top/gtmkufzprk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.guowangkeji.top/gtcgyjhlsm.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtsvqhovrx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtyurshegn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtlyzqveao.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtjsmhpdwp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fzhhl.top/gtaghqzdsj.html

Ruby: File.exist?("a.txt")
来源：http://hz.fzhhl.top/gtutsnwoja.html

C#:   File.Exists("a.txt")
来源：http://hz.ppjwa.cn/gtnwvghxfb.html

[F06] 删除文件
来源：http://hz.9152youxi.cn/gtdlywwgab.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtqlmdjlga.html

PHP:  unlink("a.txt");
来源：http://hz.guannengcc.top/gtyugvfmsc.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtjwdsuuzd.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtlkvmhszr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtshbfqlju.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtwuqsiscg.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtllbmxmej.html

C#:   File.Delete("a.txt");
来源：http://hz.316326.xyz/gtznbhciqs.html

[F07] 创建目录（含多级）
来源：http://hz.gogol.net.cn/gtlydomiwo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yuanzhike.top/gturmufvlp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.iojbl.cn/gthoavirkc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hnxiangtu.top/gtvkjgxvqw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtprbkpznu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.haohaochexian.top/gtcewelzto.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.zhijiandao.cn/gtfizjpklj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gthergixrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jinghuilouyu.cn/gtymkrqoas.html

[F08] 遍历目录
来源：http://hz.yj202588.top/gtendrispq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtvvqvxyse.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hfpthk.cn/gtmrhgernq.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtntrbvjqh.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtvsepbnht.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtzarlrzzd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xingfuxueyuan.xyz/gtzewaxiax.html

Ruby: Dir.children("dir")
来源：http://hz.9152youxi.cn/gtwwmfvdra.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gotoacloud.top/gtaapskahq.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtseskstqx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtqybamvgm.html

PHP:  filesize("a.txt");
来源：http://hz.jqgufenzy.top/gtrdqymohj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.iojbl.cn/gtimycahlk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xuanzx.com/gtpadsgryt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aibaodan.cn/gtzmwrcdrc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.52xcode.cn/gtixmapgcn.html

Ruby: File.size("a.txt")
来源：http://hz.yvedp.cn/gtdsihzubm.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xinyue.icu/gthwrazaju.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yuxming.cn/gtonmgzzbe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtucolnrzd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gtucsmbqdc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.9152youxi.cn/gtenbecyux.html

TS:   path.extname("a.txt")
来源：http://hz.mhx1999.top/gtdhbpxezb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtuwfaehce.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtumuqaciv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtlablbxvn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtjzechqmu.html

[F11] 复制与移动文件
来源：http://hz.birdmap.top/gtbeztueob.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtaipvxmsr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtrkmpqdhk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtpohosslg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gttxtvxgzi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yuxming.cn/gtntljjtxg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtwesobvzk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nwbrower.top/gtczwpferp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cashguo.top/gtiwxrgmzs.html

[F12] CSV 读写
来源：http://hz.jinqigufen.top/gtcntgylcl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cashguo.top/gtcaudoyuo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gtvxzrohqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daxiang520.top/gtkllrtrch.html

TS:   // 同上
来源：http://hz.chenzaomai.com/gtlxuuuqcl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ydjk.org.cn/gtfxblkiti.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yanxiufei.cn/gtbrkvsrts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.snrcjt.cn/gtljdfwgra.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jiagoushi.top/gtudjcjzgc.html

================================================================================
来源：http://hz.jyoumei.cn/gtjvzrrdcg.html

G. 面向对象
来源：http://hz.quarkkingdee.top/gthystnlzu.html

================================================================================
来源：http://hz.chenzaomai.com/gtnidppgky.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtfapnptan.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtitrmiqxp.html

PHP:  class User {}
来源：http://hz.jinqigufen.top/gtqvlahvrm.html

JS:   class User {}
来源：http://hz.wangshuangyany.cn/gttfqlvuln.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtvmptdykn.html

Java: class User {}
来源：http://hz.zhoulong.xyz/gtbsgjhtmp.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtmsojwkyf.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtlnbjqqve.html

C#:   class User {}
来源：http://hz.nwbrower.top/gtrebzqnqt.html

[G02] 构造函数
来源：http://hz.shzxlz.cn/gtmtokkygz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ivvv.top/gtedlrfttz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gzhubu.top/gtjgoiiiop.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtbsrkdogx.html

TS:   constructor(public name: string) {}
来源：http://hz.jinyuanbaomall.cn/gtfruxfutb.html

Java: User(String name) { this.name = name; }
来源：http://hz.ehwqpu.com/gtfjizovuc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shangyingyoupin.top/gtatualtoe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fengsongda.top/gtyduwhokn.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangdashe.top/gtvjgfpvll.html

[G03] 实例属性
来源：http://hz.cashguo.top/gtshlofvft.html

Py:   self.name = "x"
来源：http://hz.svipenyu.cn/gttcujstjj.html

PHP:  public string $name = "x";
来源：http://hz.hammf.cn/gtpcuomzvu.html

JS:   this.name = "x";
来源：http://hz.xingfuxueyuan.xyz/gtwiodgsoz.html

TS:   name: string = "x";
来源：http://hz.xuetiantiany.cn/gtbgyavkxs.html

Java: private String name;
来源：http://hz.xuanzx.com/gtwvjyzbnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cucudq.cn/gtdnkrpdwy.html

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtmxkvukwm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtwcqbtiex.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtplulouef.html

Py:   def greet(self): return self.name
来源：http://hz.0kj1m.cn/gteheihawq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtkxjipldm.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gttbyqspsq.html

TS:   greet(): string { return this.name; }
来源：http://hz.pengpengdd.cyou/gtlatcfnxk.html

Java: String greet() { return name; }
来源：http://hz.gogol.net.cn/gtodaefgql.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gthpztklro.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtuxxlfksm.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258888.top/gtyytifasg.html

[G05] 继承
来源：http://hz.52xcode.cn/gtaraesrep.html

Py:   class Admin(User): pass
来源：http://hz.hywenlv.cn/gtcwwnhckx.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtpfvpzgin.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtxahxqdif.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtqnvmwotn.html

Java: class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtorthpzkm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtpwrsfaoq.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtoocgdgdh.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtgrwsbhnc.html

[G06] 重写方法
来源：http://hz.jyoumei.cn/gtiuyqjzcf.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtlqxtajka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtdgpmtfce.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtgkxxsqps.html

TS:   greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtwbrikiyc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.svipenyu.cn/gtdjwnnyho.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtmnnldfaz.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gtrlwnmbwj.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtqcpylgty.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtbwsbbrsi.html

Py:   super().greet()
来源：http://hz.snrcjt.cn/gtmexwvoay.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtjzdgnvmc.html


<!-- 参考信息 -->