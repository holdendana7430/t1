代发 wailian999

Ruby: s.split(",");  s.split
来源：http://hz.vqdsnc.cn/gtinugeqgk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtscxmfvad.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtxpafcgwe.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtwzgzhnat.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtwtdlenjz.html

JS:   items.join(",")
来源：http://hz.ehwqpu.com/gtgmvpyztk.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtavelwumn.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtprrayrjr.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtcuhpklth.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtqsmktfxs.html

C#:   string.Join(",", items)
来源：http://hz.tian-w.cn/gtlktojhpl.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtcaliuthu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pengpengdd.cyou/gtewwsctfm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258888.top/gtngbcwffr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtjbmitjfl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ywan-chungtsiang.top/gtbfrdtrsi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtegppiecj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.vqdsnc.cn/gtgmgaqudm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.quarkkingdee.top/gtrgcqtiri.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgufenzy.top/gtnwcllpcw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.svipenyu.cn/gtuwhiukrm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yongpay.top/gtvvmroguq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtnifsejaz.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtuqogewem.html

TS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtmgkopfed.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gttsrzmgih.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtekujszgn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydjk.org.cn/gtiriulrlf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jyoumei.cn/gtoswuaocn.html

[E11] 反转字符串
来源：http://hz.cashguo.top/gtikbdyxfa.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtsojffrpn.html

PHP:  strrev($s);
来源：http://hz.sweek.top/gtxhullvzl.html

JS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtnhpafqqz.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtzomxunjp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtnyycrchq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtpgrvpjik.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gthjgowbjj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtqrguesjg.html

[E12] 统计某字符出现次数
来源：http://hz.guowangkeji.top/gttwhsshtr.html

Py:   s.count("a")
来源：http://hz.mhx1999.top/gtojnbssci.html

PHP:  substr_count($s, "a");
来源：http://hz.zhiwuduotai.top/gtwsfwudla.html

JS:   s.split("a").length - 1
来源：http://hz.zhixingplan.top/gthzohalib.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gteonszwva.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yueranfly.top/gtkqhpthln.html

Go:   strings.Count(s, "a")
来源：http://hz.yongpay.top/gtghppnqnt.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtooukazwe.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hammf.cn/gtstqwvjif.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtvwaplwtr.html

Py:   for ch in s: print(ch)
来源：http://hz.zhaomingkeji.xyz/gtgzkeonxb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtcsjzzonm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtdycqbanr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtnzwpikjr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gtbmzvtbku.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtqcnbcpag.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtgecfywad.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xinyue.icu/gtkhnvpqso.html

[E14] URL 编码与 Base64
来源：http://hz.ywan-chungtsiang.top/gthinjxjzh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtuujwakcs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtxgwhlrxv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtjopgllrs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtlydbyoja.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gttlzaysts.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinghuilouyu.cn/gtkxctvajb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guannengcc.top/gtykawtomf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenlongwang.top/gttjkqfjph.html

[E15] HTML 转义 / 反转义
来源：http://hz.zdqjudy.top/gtuczybbqm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhongyouzk.top/gtwntwbesw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.bjfxy.top/gtdoneowsk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.havefunace.top/gtbdahqwoq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aibaodan.cn/gtzamkpeni.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtccppgdyp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cashguo.top/gtnfrclcxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pengpengdd.cyou/gtucsbpirt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtrszqkahk.html

[E16] 数字千分位
来源：http://hz.nanxuanxn.top/gtqeuhiggm.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigufen.top/gtccjupoyn.html

PHP:  number_format(1234567);
来源：http://hz.jinyuanbaomall.cn/gtwrexcokm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtmferzcui.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtudennklb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zhiwuduotai.top/gtypiduftp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuetiantiany.cn/gtkybdqwyg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.kuanghao11.cn/gtefefztma.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtopwwcmos.html

[E17] 首字母大写
来源：http://hz.kuanghao11.cn/gtptvwgpio.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cheryme.top/gtdaebphqt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtsaficbmb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtyodszjjx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yangfankeji.com/gtiyiqurhu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgufenzy.top/gtwosioxzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.redwolf501.top/gtvfacdrpy.html

Ruby: s.capitalize
来源：http://hz.yj20258.top/gteyftjnkd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.52xcode.cn/gtzoldqdfh.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtckodhzrk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.bjfxy.top/gtbeecpfrb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.svipenyu.cn/gtfqzjcllh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtrborknkl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtsojufcqc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gtikfowqdv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hammf.cn/gtmdvsuvnm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtzwmdeanj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtixnskoqe.html

[E19] 多行文本按行拆分
来源：http://hz.jyoumei.cn/gtlscwzwjj.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gttoeihukc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gtlqemoizc.html

JS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtqnmjcrlv.html

TS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtrauwqonf.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtluyagntp.html

Go:   strings.Split(s, "\n")
来源：http://hz.daria6918.cn/gtuuuaisah.html

Ruby: s.lines
来源：http://hz.zhaomingkeji.xyz/gtypybiaay.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtkijowvit.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtvgbmqyou.html

Py:   if not s:
来源：http://hz.hammf.cn/gtrfyfakuq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gthdazrazj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtcgvglpnr.html

TS:   if (s === "") {}
来源：http://hz.dianchejie.cn/gtvrrhbdla.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtgbsaegrv.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtlnysudsp.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtabdvxdfa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hywenlv.cn/gtrmpzkgry.html

[E21] 超长截断加省略号
来源：http://hz.andypj.xyz/gtgpdgfavc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtyiasvzin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigfzy.top/gtfyloccdc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtizdaqfmz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtanocojxm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtyqaiutrg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.kuanghao11.cn/gtufhtdfbf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gtessrlpex.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gthqezweae.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtytgqveai.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hywenlv.cn/gttrrmuydy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtuvzkhxjb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtmxqpqgla.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtfdzyahki.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtethfzyue.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.mhx1999.top/gtrpdgwlnn.html

Ruby: s.bytesize;  s.length
来源：http://hz.ybcxt.top/gtpbaghngg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xuanzx.com/gtbhwsiqac.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcnzmmceq.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gtnigogqdl.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtctvqwepf.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtybxmeoal.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtxlfjdbvw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hysaishi.cn/gtnmapzdxx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtusmdqpet.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zycfv.cn/gteliiqahv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtztjvtobz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ywan-chungtsiang.top/gtytrjnatq.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtcpwyvjre.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtlwtqfxna.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtidujmzkr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtjnyqkwix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.svipenyu.cn/gtmaznhnkv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.iojbl.cn/gtowuusmax.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtciwhdgrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhongyouzk.top/gtyvpvfdxu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtnfvpdush.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.52xcode.cn/gtyzvcykca.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtqtelzfqw.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gttyqfetut.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtyygivtao.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jlsjyb.cn/gtdwbueskb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtophamgyu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtxbedhnqf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtkyricqup.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtuigbsrir.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.snrcjt.cn/gtflkhjtvy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtfhofhndf.html

[F04] 追加写入文件
来源：http://hz.yangfankeji.com/gtyvprxnnj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yonumen.top/gtfyfthlqn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhongyouzk.top/gtcvyqiarc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtuxmrlxll.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtnwbbjdpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cashguo.top/gtmzjuwbvv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtazfuikxc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.feifeiyinyue.top/gtjtihldur.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtsxlxlapy.html

[F05] 判断文件或目录是否存在
来源：http://hz.guowangkeji.top/gtuzemyzej.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtlppmwqem.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtejzkxzio.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtgkhciord.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtlvdiklgg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtvqyyebfo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xingfuxueyuan.xyz/gtvyrbrzub.html

Ruby: File.exist?("a.txt")
来源：http://hz.vqdsnc.cn/gtjkbyrbeh.html

C#:   File.Exists("a.txt")
来源：http://hz.iojbl.cn/gtfynphdmc.html

[F06] 删除文件
来源：http://hz.zdqjudy.top/gtgbyabhcf.html

Py:   os.remove("a.txt")
来源：http://hz.gogol.net.cn/gtsekqjlct.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtllzlrlxl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtjtlextbc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtzqvodqwd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtfnzzdter.html

Go:   os.Remove("a.txt")
来源：http://hz.cdnleiting.top/gtxtflyvnw.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtldydsqnx.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gthjtjpakm.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtxantmjrm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtgmgqfxvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj202588.top/gtknpigvvj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtyxldwqza.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtdezbmekl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.redwolf501.top/gtkfhzjnva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yongpay.top/gtywkikadc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gaohongyu789.top/gtxxwlbcdb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cheryme.top/gtpgjpmysp.html

[F08] 遍历目录
来源：http://hz.xuanzx.com/gtvyuwtivt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.0kj1m.cn/gtwnblzynj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yuanzhike.top/gtltunhoyx.html

JS:   fs.readdirSync("dir")
来源：http://hz.316326.xyz/gtcclcgfsw.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtjyvvkckd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jianghu66.top/gtwltpxqsh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hongshengwenyu.top/gtltuiilti.html

Ruby: Dir.children("dir")
来源：http://hz.svipenyu.cn/gtmygttgbt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gthbcppcat.html

[F09] 获取文件大小
来源：http://hz.ydzc1.top/gtegzyguke.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj202588.top/gtuzkamjfn.html

PHP:  filesize("a.txt");
来源：http://hz.shangyingyoupin.top/gtsvrqnxoy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.shuidangran.top/gtutduhcix.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhiwuduotai.top/gtcllwwxpp.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtlnyzhaea.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cqqwz.cn/gtcdgsuqgp.html

Ruby: File.size("a.txt")
来源：http://hz.shangyingyoupin.top/gtjiezxaby.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.wangdashe.top/gtojeoypwj.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnxiangtu.top/gthmcxuygu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jlsjyb.cn/gtgduuggpq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aizwys.cn/gtsspmpasd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtaprckmcu.html

TS:   path.extname("a.txt")
来源：http://hz.zhongyouzk.top/gtnujitxmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yangfankeji.com/gthoxhfitz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jqgfzy.top/gtpmmxxuus.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zdqjudy.top/gtnigweebo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gogol.net.cn/gtmjxaflsy.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtzlcdazos.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtvqutrtog.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cashguo.top/gtvjhvnbhs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtekybdsts.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtwjzyfmnx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ppjwa.cn/gtfrlwrrdq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.9152youxi.cn/gtisecihjk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gthvvlprnn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shuidangran.top/gtnfdzrzye.html

[F12] CSV 读写
来源：http://hz.shanyushiyangkeji.top/gtpjkefsdz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenjidiqi.icu/gtbdblgqbt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ivvv.top/gtyreazoce.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shanyushiyangkeji.top/gtclzlwrtz.html

TS:   // 同上
来源：http://hz.cqqwz.cn/gtguitewcd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yueranfly.top/gtzrpsmvqd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhengqikj.top/gtdwshshld.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtwliikbiz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtlrkmtatn.html

================================================================================
来源：http://hz.hfpthk.cn/gtaiyucifg.html

G. 面向对象
来源：http://hz.sweek.top/gtrblgzulv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtadnvypmn.html

[G01] 定义类
来源：http://hz.pycfn.com/gtusdonapq.html

Py:   class User: pass
来源：http://hz.jlsjyb.cn/gtulfaprhf.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtmtlhnyme.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtvkpidhdp.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtlgbgipil.html

Java: class User {}
来源：http://hz.mhx1999.top/gtrchmoapd.html

Go:   type User struct { Name string }
来源：http://hz.nanxuanxn.top/gtcueabagl.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtalzrnvze.html

C#:   class User {}
来源：http://hz.xylfe.cn/gtzzfloygo.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtegpdxezb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.redwolf501.top/gtupzxloqp.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.birdmap.top/gtdghhlost.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shangyingyoupin.top/gtjrpmvbcn.html

TS:   constructor(public name: string) {}
来源：http://hz.cdnleiting.top/gtrzankrzc.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtwjmuzaql.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.guowangkeji.top/gtlthtyxzs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gttjctxcom.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gtcyvytezi.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtdgxwitun.html

Py:   self.name = "x"
来源：http://hz.xylfe.cn/gtfwfdvmcn.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtnwhhrtbz.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtzungcygn.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gtrhpilwuj.html

Java: private String name;
来源：http://hz.aizwys.cn/gtvezukfuq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cucudq.cn/gtsvzadxyt.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtlkjnajkh.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj20258.top/gttysbgnul.html

[G04] 定义方法
来源：http://hz.yueranfly.top/gtyskwlcnl.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtixsyjloi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtwaqxkizq.html

JS:   greet() { return this.name; }
来源：http://hz.cqqwz.cn/gtujzrojdx.html

TS:   greet(): string { return this.name; }
来源：http://hz.tian-w.cn/gtjziygnrk.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtnxgznfrh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yuxming.cn/gtyapmfnnh.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtvjzxpfzt.html

C#:   public string Greet() => Name;
来源：http://hz.xylfe.cn/gtamfopuqg.html

[G05] 继承
来源：http://hz.yvedp.cn/gtwlhkljil.html

Py:   class Admin(User): pass
来源：http://hz.quarkkingdee.top/gttgdbwtbm.html

PHP:  class Admin extends User {}
来源：http://hz.jyoumei.cn/gthrndhtiz.html

JS:   class Admin extends User {}
来源：http://hz.havefunace.top/gtoedvudmp.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtmbmglmho.html

Java: class Admin extends User {}
来源：http://hz.0kj1m.cn/gtstywshej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtxoangljk.html

Ruby: class Admin < User; end
来源：http://hz.gogol.net.cn/gtbdbcmcam.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtqwnympmj.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtkkxgklqp.html

Py:   def greet(self): return "admin"
来源：http://hz.52xcode.cn/gtxhmgtpvz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtaqbdmcyu.html

JS:   greet() { return "admin"; }
来源：http://hz.tian-w.cn/gtalngaztu.html


<!-- 参考信息 -->