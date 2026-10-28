代发 wailian999

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gttjfqzngh.html

JS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtigajkavz.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtqmjapslj.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtazuyauxj.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gthaiodzlj.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtjlvywdle.html

C#:   string.Join(",", items)
来源：http://hz.yj20258888.top/gtouptojhh.html

[E09] 去除所有空白字符
来源：http://hz.yueranfly.top/gtylotachj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hongshengwenyu.top/gtopjdsfly.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtnxjzsomz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtekzsclko.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hysaishi.cn/gtrtymeomr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.snrcjt.cn/gtxryaieag.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtdfvpnkbe.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yanxiufei.cn/gtfgehfkxr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.nwbrower.top/gthmjfbfpw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pycfn.com/gtsnyuvjvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtwrqihcxg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ywan-chungtsiang.top/gtuswkhtmj.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhongyouzk.top/gtqgfddhzm.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtsshlxtha.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtufluedby.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gtplmxkvhd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gttpgyroio.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cucudq.cn/gtrydvspir.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtmsdpfvtp.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtqjogbsso.html

PHP:  strrev($s);
来源：http://hz.ybcxt.top/gtwdzqhywf.html

JS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtdmulspjh.html

TS:   [...s].reverse().join("")
来源：http://hz.hongshengwenyu.top/gtwtgdgqma.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.0kj1m.cn/gtykzbxfhd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xziqi.cn/gthaeyverq.html

Ruby: s.reverse
来源：http://hz.ehwqpu.com/gtujcmvpfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dianchejie.cn/gtsdwhbmoy.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtmaaedrtv.html

Py:   s.count("a")
来源：http://hz.chenjidiqi.icu/gtkeiduiyg.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgfzy.top/gtozezlcpe.html

JS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtdnqyomes.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtckiwogwy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.9152youxi.cn/gtfvgnrnee.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtfjmlrjsr.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtiuqvedws.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aizwys.cn/gtgmwpkhoc.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtzqmdqera.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtkonhmzif.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.daria6918.cn/gtudumyxjf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtfldswvvj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.fengsongda.top/gtkohmdjom.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fzhhl.top/gtauabggla.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuanzx.com/gtcmjjhmip.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtvayinwfz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtwaagobdt.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtgnwvbmsn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtsstwpbqd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.bjfxy.top/gtbwwsxhca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtwkslighc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gthwjeshvq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtbdpeklex.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangshuangyany.cn/gtlhazpuyx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.quarkkingdee.top/gtvhvjzrgm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenzaomai.com/gtxtohlzwb.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtlfjejsim.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.nanxinkj.top/gtxcfaeqwe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shanyushiyangkeji.top/gtouuprngx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtbxywzxit.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ehwqpu.com/gtndkfvjkm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dianchejie.cn/gtwwcjjfti.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtcioyaxcz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtbdehfcnh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.feifeiyinyue.top/gtwhntkgbd.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtvrcbovht.html

Py:   f"{1234567:,}"
来源：http://hz.meibo888.top/gtiqzvecyj.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtqcyqsswz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtivheqtmp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtffjeiqgl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shuidangran.top/gtttjuqjni.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gtqvhpdmiu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtcmlmpark.html

C#:   1234567.ToString("N0")
来源：http://hz.cqqwz.cn/gtjruiodvo.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtnxzdbkcn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinghuilouyu.cn/gtkvtskuzr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gthqonsgti.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtkailbgil.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtmdcjqqhr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nanxuanxn.top/gtrtvfurjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtypspvjos.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtjuprehyr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.aibaodan.cn/gtgkpydsmi.html

[E18] 模板占位符替换
来源：http://hz.shangyingyoupin.top/gtzwhkjcae.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.kuanghao11.cn/gtpshnnyil.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinghuilouyu.cn/gtennzkjpj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hongshengwenyu.top/gtimhmuqkd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gturabypny.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtsamnaejd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sxryk.cn/gtbbsalcqq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guannengcc.top/gtmkzaoijo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhongyouzk.top/gtjsmvolik.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtwisutqdo.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gtmocowlmg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dianchejie.cn/gtbvkszaky.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhiwuduotai.top/gtfwaakvnb.html

TS:   s.split(/\r?\n/)
来源：http://hz.vqdsnc.cn/gtnlzdbyrn.html

Java: s.lines().toList()
来源：http://hz.jinqigfzy.top/gtbegtltik.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtdgwaiuha.html

Ruby: s.lines
来源：http://hz.gogol.net.cn/gtqhsqlncm.html

C#:   s.Split('\n')
来源：http://hz.hnqzz.top/gtahtfhwem.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtwzgrxymy.html

Py:   if not s:
来源：http://hz.ybcxt.top/gtgoecrser.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.meibo888.top/gtqfdpfdyo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.52xcode.cn/gtydvotqyr.html

TS:   if (s === "") {}
来源：http://hz.hywenlv.cn/gthtsqxexs.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj202588.top/gtggvpusok.html

Go:   if s == "" {}
来源：http://hz.hnqzz.top/gtrnzirsih.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtkpksciai.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jianghu66.top/gtlxkmboit.html

[E21] 超长截断加省略号
来源：http://hz.iojbl.cn/gtfrwgitea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtfvktynnk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.kuanghao11.cn/gthtfwciym.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtvvjnfoiu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtbkzqodpg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtcwngymel.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ehwqpu.com/gtzsnjcujj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gttomqzcds.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.redwolf501.top/gtninfzkhd.html

[E22] 字节长度与字符长度
来源：http://hz.zycfv.cn/gtflasmddv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.0kj1m.cn/gtmqdpfhep.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtkmelxzew.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtycbtecvg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtjmmjxbmy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hfpthk.cn/gtbslphwmd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dashuyun.cn/gtqmnjpnsk.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgufenzy.top/gtywmxvrjz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhoulong.xyz/gtvuytfbpp.html

================================================================================
来源：http://hz.c1oappe.top/gtllpbpzky.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtqiwgrjjw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwwdhlsme.html

[F01] 读取整个文件
来源：http://hz.jianghu66.top/gtnuqyalyn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtsqrchziz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtyyzfnyrl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtrbdwsdlq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtyercrdbb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtgrbhdzuy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtqsscswzl.html

Ruby: File.read("a.txt")
来源：http://hz.xuetiantiany.cn/gtaqtayqsh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yonumen.top/gtrmsdhamu.html

[F02] 逐行读取文件
来源：http://hz.sweek.top/gtkwmoyxyg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.kuanghao11.cn/gtghqxzmkv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinqigufen.top/gtfhyjywzp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtnnfixlwv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtdeoifqfr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yongpay.top/gtsupffsoo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gtngbbsyjr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yongpay.top/gtzoorxrlh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtdmdlanyl.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtdfqwvqvh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tanke756.top/gtplnigitm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.birdmap.top/gtysvfgaek.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hongshengwenyu.top/gtenciwqnd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dashuyun.cn/gtltpqamtr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtnjxawewz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtsnnyrjtq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.shangyingyoupin.top/gttsusdsoy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtavyqjkpz.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtjxducmnm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuanzx.com/gtfdpipyqt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.andypj.xyz/gttozhlwwa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cashguo.top/gtuykmueun.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinyuanbaomall.cn/gtyjlosxgh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtgklbpvkn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgfzy.top/gterxmqlle.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtdixbctzv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pengpengdd.cyou/gtcgdzpyqx.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtgyyonmxy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nwbrower.top/gthtkkozlx.html

PHP:  file_exists("a.txt");
来源：http://hz.yanxiufei.cn/gteacngorc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.dashuyun.cn/gtbdwszgbr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtwzhnaahk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtopdddmpq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtookindfv.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gtvztrhpch.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtzavanwxg.html

[F06] 删除文件
来源：http://hz.ehwqpu.com/gtngnbvtjz.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtgcjogutm.html

PHP:  unlink("a.txt");
来源：http://hz.cucudq.cn/gticszxbym.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtcibujsxw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtsttxlplf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtigcqlfqk.html

Go:   os.Remove("a.txt")
来源：http://hz.ppjwa.cn/gtypauyziu.html

Ruby: File.delete("a.txt")
来源：http://hz.shanyushiyangtech.top/gtpnekecyw.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtbyqgxssw.html

[F07] 创建目录（含多级）
来源：http://hz.ivvv.top/gtmkjwpqtu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nanxinkj.top/gtmqzbbgsz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.meibo888.top/gtgiujvbfb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.andypj.xyz/gtyjmrmnzu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtcsfluash.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.kuanghao11.cn/gtuerorwta.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gtsdswkkmz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.cdnleiting.top/gtjxbqocew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gotoacloud.top/gtjvjyhuyz.html

[F08] 遍历目录
来源：http://hz.nanxuanxn.top/gtleqwjnqa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yangfankeji.com/gtvmfksbdp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gogol.net.cn/gtgumflxqm.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtnuhvfngk.html

TS:   fs.readdirSync("dir")
来源：http://hz.gotoacloud.top/gtxvzziafp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtdmnfrqpu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtujrjlahf.html

Ruby: Dir.children("dir")
来源：http://hz.vqdsnc.cn/gtxdytubut.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gtmvcsaijx.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtzbeokmbc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.wangdashe.top/gtqsiirgse.html

PHP:  filesize("a.txt");
来源：http://hz.hnqzz.top/gtxxswslma.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtgzoqajan.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtxtlhmtah.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtgrmgndtg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtmqpjglna.html

Ruby: File.size("a.txt")
来源：http://hz.feifeiyinyue.top/gtbmpnhaub.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aibaodan.cn/gtbppczkmn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gtpsynsxyy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pycfn.com/gttfyfkcom.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yj202588.top/gtytkdefyj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtsmlgzupk.html

TS:   path.extname("a.txt")
来源：http://hz.dianchejie.cn/gtchtrhuug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.feifeiyinyue.top/gtpzkvokcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shzxlz.cn/gtquvhudba.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtottcqkdx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtsfzzfbwx.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtljgkixjy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtzhoqtvbm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gogol.net.cn/gtszcouwbs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtiqtevpqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtgfmxxvfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.haohaochexian.top/gtydopokxc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.tian-w.cn/gtpqnoqupb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.316326.xyz/gthrxcyunw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cqqwz.cn/gtsacclkhj.html

[F12] CSV 读写
来源：http://hz.tianlin.xyz/gtccihcmsx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj20258.top/gtnrhnbeuh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.svipenyu.cn/gtsqtdsied.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtizzcxdkp.html

TS:   // 同上
来源：http://hz.yvedp.cn/gtoehcaxml.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.andypj.xyz/gtomzmakck.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258.top/gtqgtkruqx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtdtpkbhig.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtxcwmfgsk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjwflfmvi.html

G. 面向对象
来源：http://hz.yueranfly.top/gtvgpbwcsc.html

================================================================================
来源：http://hz.xuanzx.com/gtfupdlnza.html

[G01] 定义类
来源：http://hz.yuxming.cn/gtulpicmss.html

Py:   class User: pass
来源：http://hz.nanxinkj.top/gtgojicdvy.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtqnstjumz.html

JS:   class User {}
来源：http://hz.chenlongwang.top/gtjpetzkbm.html

TS:   class User { name: string = ""; }
来源：http://hz.snrcjt.cn/gtpjysrqpr.html

Java: class User {}
来源：http://hz.hywenlv.cn/gtygwqqlvx.html

Go:   type User struct { Name string }
来源：http://hz.zhijiandao.cn/gtlixvqhbj.html

Ruby: class User; end
来源：http://hz.kuanghao11.cn/gtfrqdhceq.html

C#:   class User {}
来源：http://hz.xziqi.cn/gtawrmnmje.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtbnsqyfgo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xuanzx.com/gtpfqdlofv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nwbrower.top/gtqteeaovs.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xinyue.icu/gtpvlemlea.html

TS:   constructor(public name: string) {}
来源：http://hz.zhoulong.xyz/gtzbvcczwb.html

Java: User(String name) { this.name = name; }
来源：http://hz.fzhhl.top/gtiiiguzzw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tanke756.top/gtuzqyuhgq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nwbrower.top/gttmdfottd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydjk.org.cn/gtnspkpycw.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtutijhczq.html

Py:   self.name = "x"
来源：http://hz.chenjidiqi.icu/gtptxjaglk.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gtxvcwqzap.html

JS:   this.name = "x";
来源：http://hz.zhijiandao.cn/gtvyideyba.html

TS:   name: string = "x";
来源：http://hz.hongshengwenyu.top/gtpulnapuy.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtkwlcvlzl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.quarkkingdee.top/gtyirubnlc.html

Ruby: @name = "x"
来源：http://hz.ydjk.org.cn/gtzwnwowrm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ppjwa.cn/gtvbhkxljl.html

[G04] 定义方法
来源：http://hz.nanxinkj.top/gtgcxwxokk.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtgsgccebv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtchuddhvf.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtthaijfha.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydzc1.top/gtaaxfxrps.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtieeauzmb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gthbgbvqqz.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtnsdotvvy.html

C#:   public string Greet() => Name;
来源：http://hz.zhiwuduotai.top/gtvknlcsqh.html

[G05] 继承
来源：http://hz.chenlongwang.top/gtksculnas.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtugzdjrge.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtenkskzmk.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtzxawfvpc.html

TS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtnhdcizgu.html

Java: class Admin extends User {}
来源：http://hz.birdmap.top/gtamylkyqn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydzc1.top/gtjgcypbsd.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtdrzrprnc.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtbxyccrmz.html

[G06] 重写方法
来源：http://hz.xuetiantiany.cn/gtkqzonqqh.html

Py:   def greet(self): return "admin"
来源：http://hz.yuanzhike.top/gtuctwgnga.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtenyofhdl.html

JS:   greet() { return "admin"; }
来源：http://hz.pycfn.com/gtcoxwnqrl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xingfuxueyuan.xyz/gttboujufv.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gteazmnjct.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtaexbvcny.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtiydjqbom.html


<!-- 参考信息 -->