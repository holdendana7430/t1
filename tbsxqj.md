代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hz.bjfxy.top/gteobdsbjd.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtqxsemded.html

C#:   string.Join(",", items)
来源：http://hz.gzhubu.top/gtyiknjsjz.html

[E09] 去除所有空白字符
来源：http://hz.chenzaomai.com/gtunqggxnx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jiagoushi.top/gtficryapt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gtyvrarygt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtvcsjooub.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtkpqorvrr.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gthtzfqgpg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnxiangtu.top/gtxbybsfgz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yonumen.top/gtwcztoddw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gtkdtrsxab.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sysykeji.top/gtcoxtcxvr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ehwqpu.com/gtdabyyyhw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxuanxn.top/gthwxkzjsr.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtbgnaiyab.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtmqwwsiwr.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gttrbrkpgz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtmxdmmpqp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gttlgiialk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxinkj.top/gtovhquirq.html

[E11] 反转字符串
来源：http://hz.ywan-chungtsiang.top/gtjdbljgwc.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtodihfbfc.html

PHP:  strrev($s);
来源：http://hz.jinghuilouyu.cn/gtsyeowuko.html

JS:   [...s].reverse().join("")
来源：http://hz.iojbl.cn/gtneleqqpd.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtoozzrxji.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtfmowtirq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhoulong.xyz/gtltojhjop.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtooydsgab.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtllmxenuw.html

[E12] 统计某字符出现次数
来源：http://hz.mhx1999.top/gtblwaabwi.html

Py:   s.count("a")
来源：http://hz.hongshengwenyu.top/gtjhewgkbx.html

PHP:  substr_count($s, "a");
来源：http://hz.tanke756.top/gtbcuanyzo.html

JS:   s.split("a").length - 1
来源：http://hz.zhongyouzk.top/gtvyalstxb.html

TS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtgvjheqjn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtvgslmvhr.html

Go:   strings.Count(s, "a")
来源：http://hz.hnxiangtu.top/gthcnrkaji.html

Ruby: s.count("a")
来源：http://hz.yongpay.top/gtjnxhyvcd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnqzz.top/gtqzrrscsy.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtktjlhsca.html

Py:   for ch in s: print(ch)
来源：http://hz.zdqjudy.top/gtxsbmwjzw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cucudq.cn/gttsisjmjr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gthnjnuwcn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tian-w.cn/gtbnbdvegm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtwwsjherw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.kuanghao11.cn/gtmirnjpuz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xinyue.icu/gtieavtwot.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtovdyqyiu.html

[E14] URL 编码与 Base64
来源：http://hz.yonumen.top/gtitefppwn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxuanxn.top/gtibbxfkly.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangtech.top/gttstweazp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinqigfzy.top/gtzgziadtj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtuobxkltg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xuanzx.com/gtjexsvtqi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gtrqfbpccn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ehwqpu.com/gtgbrbsxre.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhijiandao.cn/gtwkazlrbg.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtbnktdoau.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtmipabkxj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gtmvxwcefs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtsmpudwua.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtvoyalqck.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gtjkilgxfo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hfpthk.cn/gtrpwysczo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jiagoushi.top/gtpdgemkib.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cashguo.top/gtavugtmeo.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtjqhywczx.html

Py:   f"{1234567:,}"
来源：http://hz.daria6918.cn/gthvkdwlag.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtvshpxbdo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtlgojgmxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shuidangran.top/gtchjgwxez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gtdjfaigrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.fengsongda.top/gtpikgfile.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.kuanghao11.cn/gthjxyvkrq.html

C#:   1234567.ToString("N0")
来源：http://hz.gogol.net.cn/gtfercqznb.html

[E17] 首字母大写
来源：http://hz.nwbrower.top/gtfqxndldg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yanxiufei.cn/gtqirqektt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtyegjjmto.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtheqixpje.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtidvwgmba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigfzy.top/gtjalfvdka.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtsisoxcqs.html

Ruby: s.capitalize
来源：http://hz.dianchejie.cn/gtqijvwubc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.pengpengdd.cyou/gtqsctoujy.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gthttothwe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gtyvsrccfr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtydtwhbyi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtddmwkjfd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtkymqgsxo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtlzflygxd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtjxhrpuwn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhengqikj.top/gtnhmyndhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nwbrower.top/gtuuffanxk.html

[E19] 多行文本按行拆分
来源：http://hz.nwbrower.top/gtxnounjsr.html

Py:   s.splitlines()
来源：http://hz.daxiang520.top/gtbpfcfkpn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtfocosgqu.html

JS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtznxepxxb.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtqwllbmom.html

Java: s.lines().toList()
来源：http://hz.cucudq.cn/gtuapkrfqr.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtlxiorfxn.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtvraalyic.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtdoojjojn.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gtehmicmbc.html

Py:   if not s:
来源：http://hz.ivvv.top/gthtawoztk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.316326.xyz/gttdauuorb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtdyzssswn.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gtiodhkkqw.html

Java: if (s.isEmpty()) {}
来源：http://hz.shanyushiyangkeji.top/gtuvuwtnaj.html

Go:   if s == "" {}
来源：http://hz.tianlin.xyz/gtzdyhtmgk.html

Ruby: if s.empty?
来源：http://hz.ydzc1.top/gtplnurbnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sysykeji.top/gtrqhpezym.html

[E21] 超长截断加省略号
来源：http://hz.dashuyun.cn/gtzmhgkpzs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hysaishi.cn/gtchsprgbq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.quarkkingdee.top/gtevgejvun.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gogol.net.cn/gtdtsirinm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtismtklkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtcwmswwfs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hysaishi.cn/gtwfthnctu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.haohaochexian.top/gtuvzvjumi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtwhtvvrbo.html

[E22] 字节长度与字符长度
来源：http://hz.dashuyun.cn/gtttaopyqq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gtprptvrvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtlndsphsz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yvedp.cn/gtclhsvajw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtiqwfifhm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtqkabwbuc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.bjfxy.top/gtiqqfzdgf.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtvcvpxnfb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fengsongda.top/gtskkjjqrn.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtgiurnfet.html

F. 文件与目录
来源：http://hz.zhaomingkeji.xyz/gtckwelfke.html

================================================================================
来源：http://hz.jyoumei.cn/gthhyynslc.html

[F01] 读取整个文件
来源：http://hz.cqqwz.cn/gtuxiqadxh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtniyujqly.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yuanzhike.top/gtffcfoyip.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtegshmtkw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtqsymufac.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtwjrnuumw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhixingplan.top/gtqvgocfxb.html

Ruby: File.read("a.txt")
来源：http://hz.zhengqikj.top/gtemhvrped.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxinkj.top/gtlhqobswb.html

[F02] 逐行读取文件
来源：http://hz.havefunace.top/gtwblcdjbw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtfjkswxgd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhijiandao.cn/gtqwknbhga.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtjzzwoaqn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtgqetcvst.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tanke756.top/gtwnairdaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guowangkeji.top/gtkihvmlno.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gtpiapcoxi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtxgmxotci.html

[F03] 写入文件（覆盖）
来源：http://hz.yonumen.top/gtqkpaampj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.guannengcc.top/gtxrgpjtgq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtmvzttuxp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtnsosynza.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtkdnwfvji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gtircpndlt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xziqi.cn/gtnumrdgdy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hysaishi.cn/gtncgrspto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tanke756.top/gtarbnsddg.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtwvqqneka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zdqjudy.top/gtyodrnjzd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fzhhl.top/gtcsozncem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtqinxbxfl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtvpkigblg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtxrveijwj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtimjhiqim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtdyspwpuy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fzhhl.top/gtpwxmygdn.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtyvcjttmj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.redwolf501.top/gtvaczuogq.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtausjabjy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gthprodfsr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.dianchejie.cn/gtumdqovuy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtmfqbzfev.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtoxehqywn.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtcvlshyph.html

C#:   File.Exists("a.txt")
来源：http://hz.gzhubu.top/gtjqbokuqo.html

[F06] 删除文件
来源：http://hz.ydzc1.top/gtsjvrecuh.html

Py:   os.remove("a.txt")
来源：http://hz.mhx1999.top/gtkfmfzdgl.html

PHP:  unlink("a.txt");
来源：http://hz.svipenyu.cn/gtckfymwpg.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtuimupwns.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtrwrmvhxc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gotoacloud.top/gtdmxrghxh.html

Go:   os.Remove("a.txt")
来源：http://hz.jqgufenzy.top/gtmwjlbuho.html

Ruby: File.delete("a.txt")
来源：http://hz.andypj.xyz/gtcrcfzjmi.html

C#:   File.Delete("a.txt");
来源：http://hz.sysykeji.top/gtpskgbrqm.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtbkhztwbn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtipjcpers.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pengpengdd.cyou/gtcwqesmxb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zdqjudy.top/gtbwnkxnin.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtfnkxsdmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zhaomingkeji.xyz/gtgricvtfj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jlsjyb.cn/gthfisnpvi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yueranfly.top/gtiipfgkif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sysykeji.top/gthxwmovjm.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtdyqsiugz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtqswdjmwk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtubzugdmm.html

JS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtrxwndlcv.html

TS:   fs.readdirSync("dir")
来源：http://hz.yonumen.top/gtrcpmnxaw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtkqmiqixc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ydzc1.top/gtuahwnzys.html

Ruby: Dir.children("dir")
来源：http://hz.sweek.top/gtobcedxan.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtxhtszwpq.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtwklxhiuf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtnphmcuvl.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtjixxmllu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gthzgmorhl.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtxczxctjv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hongshengwenyu.top/gtxsfuvcfd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtmscsphpb.html

Ruby: File.size("a.txt")
来源：http://hz.0kj1m.cn/gtzbbolgid.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fzhhl.top/gtxorlhprx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.feifeiyinyue.top/gtgducnypn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ivvv.top/gtbldtflup.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.shanyushiyangkeji.top/gtfihqloow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yangfankeji.com/gtnztpvysf.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gtleliixrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangdashe.top/gtwkmsblbh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtopzzdtcs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtrisrxpki.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jianghu66.top/gtqwtwwqcq.html

[F11] 复制与移动文件
来源：http://hz.shzxlz.cn/gtielmrfei.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yonumen.top/gtupilfavx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.chenjidiqi.icu/gtqcvtsocd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gtefgqrunj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yueranfly.top/gthbbgbnpb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtfcgvejii.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sufxvd.cn/gtiqrgqdli.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtsnwxreyg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cqqwz.cn/gtghnfzvjo.html

[F12] CSV 读写
来源：http://hz.nanxinkj.top/gterdzkzpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinyuanbaomall.cn/gtvphsrbnz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zhongyouzk.top/gtlqjrqhgu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shuidangran.top/gtxxulkpvj.html

TS:   // 同上
来源：http://hz.ydjk.org.cn/gthqyfhlxi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.sufxvd.cn/gtfancuxew.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yj20258888.top/gtmfxccmhk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ydzc1.top/gtxwbhjbky.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangshuangyany.cn/gtqgtyrsxt.html

================================================================================
来源：http://hz.gzhubu.top/gtwgsjtnua.html

G. 面向对象
来源：http://hz.smart0.xyz/gtzmnwtnme.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyoepvgwj.html

[G01] 定义类
来源：http://hz.cashguo.top/gtnzkrjmov.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtvrcxkpln.html

PHP:  class User {}
来源：http://hz.ywan-chungtsiang.top/gtxoxcholq.html

JS:   class User {}
来源：http://hz.yonumen.top/gtphaddffe.html

TS:   class User { name: string = ""; }
来源：http://hz.gogol.net.cn/gtiiufmysi.html

Java: class User {}
来源：http://hz.yvedp.cn/gtmnqrgssu.html

Go:   type User struct { Name string }
来源：http://hz.birdmap.top/gthzbgfvab.html

Ruby: class User; end
来源：http://hz.zhoulong.xyz/gthodwetxx.html

C#:   class User {}
来源：http://hz.ppjwa.cn/gtxirctjju.html

[G02] 构造函数
来源：http://hz.shangyingyoupin.top/gtvyajovso.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jinyuanbaomall.cn/gtqtfmopij.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ybcxt.top/gtdsqerpck.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tanke756.top/gtioonsxkm.html

TS:   constructor(public name: string) {}
来源：http://hz.andypj.xyz/gtvmzwfxok.html

Java: User(String name) { this.name = name; }
来源：http://hz.xylfe.cn/gtcbakbnet.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.cashguo.top/gtltbizfhv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shanyushiyangtech.top/gtdjiwctvl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtldkxdkwn.html

[G03] 实例属性
来源：http://hz.yj20258.top/gtroitfdmp.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtaevhrwkn.html

PHP:  public string $name = "x";
来源：http://hz.zhaomingkeji.xyz/gtvpjfgmtj.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtmwqaoaej.html

TS:   name: string = "x";
来源：http://hz.wangdashe.top/gtwwwuhdpz.html

Java: private String name;
来源：http://hz.sxryk.cn/gtlszowfis.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtmwpszfsb.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gtpykhgdjm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cheryme.top/gtluecqrou.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtbxvmdopl.html

Py:   def greet(self): return self.name
来源：http://hz.jianghu66.top/gtswzqoelt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yongpay.top/gtkpawjqae.html

JS:   greet() { return this.name; }
来源：http://hz.gogol.net.cn/gtdxxdyfmu.html

TS:   greet(): string { return this.name; }
来源：http://hz.birdmap.top/gtfcaluhqo.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtcnlssaih.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gthxqpsske.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gteihdtazo.html

C#:   public string Greet() => Name;
来源：http://hz.shzxlz.cn/gtfukjqwme.html

[G05] 继承
来源：http://hz.sweek.top/gtqjivxynr.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gtmahpsbin.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtjrfwyygw.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtuhnrsqbe.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtvvrofzsq.html

Java: class Admin extends User {}
来源：http://hz.xinyue.icu/gtbirbpnpd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtpldumoad.html

Ruby: class Admin < User; end
来源：http://hz.nanxuanxn.top/gtadyvhvkc.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gtdejlpzpm.html

[G06] 重写方法
来源：http://hz.9152youxi.cn/gtewqqvred.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtmqvxiduh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtdqajnkzs.html

JS:   greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtfizxmbtk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtiomhfuun.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtkftgibmc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.0kj1m.cn/gtthkukkxd.html

Ruby: def greet; "admin"; end
来源：http://hz.zycfv.cn/gtvupfxano.html

C#:   public override string Greet() => "admin";
来源：http://hz.shuidangran.top/gtlzmrzgyo.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtaasjvuwp.html

Py:   super().greet()
来源：http://hz.yonumen.top/gtclpjdtta.html

PHP:  parent::greet();
来源：http://hz.zhijiandao.cn/gtrmiiqmwf.html


<!-- 参考信息 -->