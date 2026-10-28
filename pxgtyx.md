代发 wailian999

C#:   s.Replace("a", "b")
来源：http://hz.yuxming.cn/gtoxixulgi.html

[E07] 按分隔符拆分
来源：http://hz.ydzc1.top/gtjtcoqcng.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuetiantiany.cn/gtajowwdot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangtech.top/gtvsqlwtdo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtvpnfzwkf.html

TS:   s.split(",")
来源：http://hz.cqqwz.cn/gtrslchexc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtsoaxfprf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtehjsfkba.html

Ruby: s.split(",");  s.split
来源：http://hz.kuanghao11.cn/gtbgcduhpg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtvcffqymf.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtmlnjjbel.html

Py:   ",".join(items)
来源：http://hz.gogol.net.cn/gtcjtkoosu.html

PHP:  implode(",", $items);
来源：http://hz.andypj.xyz/gtdblbjtbp.html

JS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtygrkjzqe.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtbjvsdlts.html

Java: String.join(",", items)
来源：http://hz.hywenlv.cn/gttrgpxfcl.html

Go:   strings.Join(items, ",")
来源：http://hz.yj20258888.top/gtaiexqzil.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtcxqtoxqt.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gtkuesqdzt.html

[E09] 去除所有空白字符
来源：http://hz.yvedp.cn/gthpiggziu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtjypspqjr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guannengcc.top/gtxhxgtzxk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtliyycyfg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtzegwvvdb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yongpay.top/gtmcsrddev.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtqqsilgkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ybcxt.top/gtaipxdwed.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtvcmwukwb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gtulipqtel.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtujficrox.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtfznlrjdk.html

JS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtvinvidbh.html

TS:   "7".padStart(3, "0")
来源：http://hz.shanyushiyangkeji.top/gthmrrjutu.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtkqjhkncc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtvcvcyuke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ywan-chungtsiang.top/gtzagoxwop.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtqvrwyfxh.html

[E11] 反转字符串
来源：http://hz.hongshengwenyu.top/gtxsahaqnm.html

Py:   s[::-1]
来源：http://hz.gaohongyu789.top/gtyvqhmntx.html

PHP:  strrev($s);
来源：http://hz.9152youxi.cn/gtljqorife.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtkjaefyow.html

TS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gtryyivxsj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hysaishi.cn/gtaimwabgf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gtgqfreqji.html

Ruby: s.reverse
来源：http://hz.yuanzhike.top/gtgzsobunv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gtpmtetkie.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtpqhvstbk.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtrjmbkjsv.html

PHP:  substr_count($s, "a");
来源：http://hz.pycfn.com/gtjrqbabwa.html

JS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtpezrfwcg.html

TS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gthzhukuqg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtqldityev.html

Go:   strings.Count(s, "a")
来源：http://hz.daria6918.cn/gtbvyeztwo.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtfmahugco.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cucudq.cn/gtrjmracuq.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtscxoixfb.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtolcghesq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.mhx1999.top/gtpugqajpz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtzdmgnxbv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.smart0.xyz/gtdblqspis.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtfkzyqzxr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtvkkqqeqi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtqrrgjend.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigufen.top/gtxldqzvnd.html

[E14] URL 编码与 Base64
来源：http://hz.xuanzx.com/gtysydexot.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtzeovowgw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtotxixmpz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhixingplan.top/gtyiipwhgt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.9152youxi.cn/gtsrzpivpg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xylfe.cn/gtqixvcnxv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gtqyaiaivv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhijiandao.cn/gtqvehjsys.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtmivjvudy.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtwwndxffe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.snrcjt.cn/gtvdlvtslx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gtzfpytcvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gttwipiwcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.daxiang520.top/gtsnglleii.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gtdigcllva.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtscqrwkdq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ivvv.top/gttxwatmai.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.cdnleiting.top/gtcgygxrbp.html

[E16] 数字千分位
来源：http://hz.vqdsnc.cn/gtfvmtiohz.html

Py:   f"{1234567:,}"
来源：http://hz.xuetiantiany.cn/gttfzoaadz.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gttjjvkfry.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxuanxn.top/gtkcptnift.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtihcgnsvd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtsnwihpzr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtuvuvneim.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yuxming.cn/gtlsptzyrj.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gttjorxivt.html

[E17] 首字母大写
来源：http://hz.jinqigufen.top/gtakaurgsi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinyuanbaomall.cn/gtggzjitub.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ywan-chungtsiang.top/gtoahhotza.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtlokjbyzm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtaegaefmr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuanzhike.top/gtnglsbxsq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtgstsrxxa.html

Ruby: s.capitalize
来源：http://hz.xingfuxueyuan.xyz/gtsbzroosj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtmxqbugex.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtfhdcvvnh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtpzixqdns.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gtqsbxrgwr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gthouxxegu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtanfjwpav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gtxuqtpaph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hfpthk.cn/gtvajnrqja.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258.top/gtcdpgosjw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtobazwftt.html

[E19] 多行文本按行拆分
来源：http://hz.tanke756.top/gtnvzuczph.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtdsenawlp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtulokibjk.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtofkefarp.html

TS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gttamjmnnp.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtgqbarbfe.html

Go:   strings.Split(s, "\n")
来源：http://hz.hongshengwenyu.top/gtuzcpnuph.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtvrtluyqa.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gttmrprmst.html

[E20] 判断字符串是否为空
来源：http://hz.guowangkeji.top/gtbqojefqm.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtkramjzfu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gthgwkaonq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.dashuyun.cn/gtgdrppdaz.html

TS:   if (s === "") {}
来源：http://hz.chenlongwang.top/gtfjysjfeg.html

Java: if (s.isEmpty()) {}
来源：http://hz.svipenyu.cn/gthhjjswlo.html

Go:   if s == "" {}
来源：http://hz.chenlongwang.top/gtnprxhpxd.html

Ruby: if s.empty?
来源：http://hz.ppjwa.cn/gtqcxhquvq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gtqmgghipg.html

[E21] 超长截断加省略号
来源：http://hz.aibaodan.cn/gtmtcjgfmi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtsvqxnvoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shangyingyoupin.top/gtbesnubzh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtcfhordks.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtdsmjoqku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtudhumesp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hammf.cn/gtxtfgdtfn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtwonxpbpr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gteozgbagb.html

[E22] 字节长度与字符长度
来源：http://hz.dashuyun.cn/gthynpyjhw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtndgacfha.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtooiaywff.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtvfcuaexv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gthmrelxgg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtpymgganm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guannengcc.top/gtdojoyqpp.html

Ruby: s.bytesize;  s.length
来源：http://hz.dianchejie.cn/gtlaqovxkp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gotoacloud.top/gtfyfclzpm.html

================================================================================
来源：http://hz.fzhhl.top/gtkfhxslii.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtgrgmluva.html

================================================================================
来源：http://hz.yuxming.cn/gtmmmvuzxm.html

[F01] 读取整个文件
来源：http://hz.guowangkeji.top/gtjbprwoui.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtdlnfcepr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.52xcode.cn/gtyvmvyern.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtnnxmkrue.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtromhtixj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtnnxbhkbg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtmwpriovu.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtqbuckdis.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtojctjgth.html

[F02] 逐行读取文件
来源：http://hz.ppjwa.cn/gtnuytbahq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtbdjvghlw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtrfjqihbd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtggbqfjis.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258888.top/gtoghcyacb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.gzhubu.top/gtnfbxkoqc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtvkuvjlst.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtzisbnibi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tanke756.top/gtlheejmog.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gthnwhclqk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.9152youxi.cn/gtwnderjfb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtjrsmxeuk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtbywqhhjd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gtoprvgqmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.dianchejie.cn/gtpyuzpoil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhaomingkeji.xyz/gtofpdkeix.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gtfvymjuls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.wangdashe.top/gtipbtspjb.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtexdzbmwf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.meibo888.top/gthhhsfteq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ydzc1.top/gtjgpnuhbs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gttfaqfbqp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtyebvqyqz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigfzy.top/gtjstvshzc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenlongwang.top/gtjuampoot.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yanxiufei.cn/gtsqfjhvly.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tian-w.cn/gttyqibvqq.html

[F05] 判断文件或目录是否存在
来源：http://hz.tanke756.top/gttjiflujx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.feifeiyinyue.top/gtawrsfals.html

PHP:  file_exists("a.txt");
来源：http://hz.chenzaomai.com/gtleihpuzk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yueranfly.top/gtyfoteebd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yongpay.top/gtoueglclr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtdrxzakud.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yonumen.top/gtfeuujrub.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtbtektnmx.html

C#:   File.Exists("a.txt")
来源：http://hz.kuanghao11.cn/gtnxlkugua.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtxabphkaq.html

Py:   os.remove("a.txt")
来源：http://hz.yuxming.cn/gtnchayoio.html

PHP:  unlink("a.txt");
来源：http://hz.zhixingplan.top/gtnfrbiohu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yvedp.cn/gtmwaycrgv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.daxiang520.top/gtpzbkziyj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtrztysjft.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gttqbkuihi.html

Ruby: File.delete("a.txt")
来源：http://hz.xylfe.cn/gtdynwaees.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigufen.top/gtmfkohiqr.html

[F07] 创建目录（含多级）
来源：http://hz.tanke756.top/gtvjvhpxmg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.sweek.top/gtivxrfppw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj20258.top/gtrmjkynij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtffwbcbvt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtlsdmmmmn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shanyushiyangkeji.top/gtstbxiifv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtwxoabfgx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shangyingyoupin.top/gtkooyrewh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuxming.cn/gtwxukmoiy.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtskzkprin.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.birdmap.top/gtatcvsrfq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.kuanghao11.cn/gtgmnalews.html

JS:   fs.readdirSync("dir")
来源：http://hz.jiagoushi.top/gtcjzcfhjr.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnxiangtu.top/gtbnibqzsp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.guowangkeji.top/gtwwspdlfc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhixingplan.top/gtpivjzbvb.html

Ruby: Dir.children("dir")
来源：http://hz.0kj1m.cn/gtkaqoxilm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xziqi.cn/gtmsuskuds.html

[F09] 获取文件大小
来源：http://hz.zhixingplan.top/gtjsihejse.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtbwititec.html

PHP:  filesize("a.txt");
来源：http://hz.kuanghao11.cn/gtkmyxsqsy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtftqkcqmr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhaomingkeji.xyz/gtmxezeweb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtwxaihedl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtuogliagq.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gthbrbmril.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtxdeipicb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jinghuilouyu.cn/gtrfzljyeb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hfpthk.cn/gtsphdiebs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.jiagoushi.top/gtfvsuztdv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtktfbtujv.html

TS:   path.extname("a.txt")
来源：http://hz.yuanzhike.top/gtcexcobjn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtkmoihopj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shangyingyoupin.top/gtapwmgbsn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtllxxgpbd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.smart0.xyz/gtfgsnyqhx.html

[F11] 复制与移动文件
来源：http://hz.ywan-chungtsiang.top/gtnhxxdiis.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ydjk.org.cn/gtacfoneww.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hnqzz.top/gtngbufcki.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtaxfissgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gteczarcyg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.nwbrower.top/gtqloclfju.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cashguo.top/gtvzotnywc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtseulpiju.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xinyue.icu/gteadcbbfr.html

[F12] CSV 读写
来源：http://hz.haohaochexian.top/gtjmohrydl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.pengpengdd.cyou/gtifanchhr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.daria6918.cn/gtkqyhegnq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtgrkznkjn.html

TS:   // 同上
来源：http://hz.zycfv.cn/gtgnpzlrke.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtgftsmznu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuetiantiany.cn/gtwwfqgwxo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.vqdsnc.cn/gtsfbiatxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtqufigfvn.html

================================================================================
来源：http://hz.aibaodan.cn/gtikcfsnrm.html

G. 面向对象
来源：http://hz.xingfuxueyuan.xyz/gtrlfuzrqx.html

================================================================================
来源：http://hz.svipenyu.cn/gtmpfmhpwe.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtskcadwca.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtuezgzplf.html

PHP:  class User {}
来源：http://hz.nwbrower.top/gtxvbzdkkb.html

JS:   class User {}
来源：http://hz.pengpengdd.cyou/gthzoonjzx.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtsipjriiy.html

Java: class User {}
来源：http://hz.shanyushiyangkeji.top/gtmjmfsbot.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtjkrpoqfu.html

Ruby: class User; end
来源：http://hz.hysaishi.cn/gtfrjdjjqa.html

C#:   class User {}
来源：http://hz.sxryk.cn/gtzcqskkuh.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtsvhjqqoa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtjwraysts.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.ydjk.org.cn/gtjytbbdsg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gtnxaeqans.html

TS:   constructor(public name: string) {}
来源：http://hz.sysykeji.top/gtbnkdnjps.html

Java: User(String name) { this.name = name; }
来源：http://hz.aizwys.cn/gtqvwkuzrc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daxiang520.top/gtjgldafkp.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zdqjudy.top/gtcjtgktsl.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhiwuduotai.top/gtunjhfzza.html

[G03] 实例属性
来源：http://hz.jyoumei.cn/gtabinyzof.html

Py:   self.name = "x"
来源：http://hz.jinqigfzy.top/gtgibkowwp.html

PHP:  public string $name = "x";
来源：http://hz.yj20258888.top/gttgabhtdu.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gttxxaxwiz.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtginxogsr.html

Java: private String name;
来源：http://hz.aizwys.cn/gtquhjhjjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtbktpcakt.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtxeofphob.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gaohongyu789.top/gtqdjfklcv.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtavecoyjf.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtnuqhsnbn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yueranfly.top/gtjlypkfud.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtnmutcjwk.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangdashe.top/gtdzjllxdg.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtakldjpuh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtpyqbwllh.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtjhgeifei.html

C#:   public string Greet() => Name;
来源：http://hz.yuxming.cn/gtvqolwrcs.html

[G05] 继承
来源：http://hz.chenjidiqi.icu/gtfpbtuulm.html

Py:   class Admin(User): pass
来源：http://hz.ehwqpu.com/gtgcrsjbut.html

PHP:  class Admin extends User {}
来源：http://hz.svipenyu.cn/gtcrkbhznm.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtwdkyiqei.html

TS:   class Admin extends User {}
来源：http://hz.quarkkingdee.top/gtxzmlfsnx.html


<!-- 参考信息 -->