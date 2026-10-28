代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hongshengwenyu.top/gtfilgqevq.html

[E03] 截取子串
来源：http://hz.gaohongyu789.top/gtuymlxbxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.316326.xyz/gtwtjbucif.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.haohaochexian.top/gttdbmxesd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtqxxszqvd.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtflzuwdmv.html

Java: s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtavzefwfd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ivvv.top/gtolbnrqgk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.kuanghao11.cn/gttefvdsix.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtbtccklkb.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gttrvueeer.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtbtozxisy.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangkeji.top/gtlbdcllbl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtzddjqngt.html

TS:   s.indexOf("x")
来源：http://hz.shzxlz.cn/gtjmqranqi.html

Java: s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtaivuafav.html

Go:   strings.Index(s, "x")
来源：http://hz.birdmap.top/gttotxvwkn.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtvrjbomms.html

C#:   s.IndexOf("x")
来源：http://hz.guowangkeji.top/gtnnwvnkno.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gtkwflgsdl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtoofoklzm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.pengpengdd.cyou/gtlmysubyh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtmydpcivf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.iojbl.cn/gteodrbbct.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtbaszbfsv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hywenlv.cn/gtlqxbtjwt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtosddtlxi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gtlezgwgxu.html

[E06] 替换子串
来源：http://hz.jinqigufen.top/gttjpzomzw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yueranfly.top/gtwvyxqlbg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hnxiangtu.top/gtcsdeaqhv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtunwemutu.html

TS:   s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtmsgidgpn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtaopbdqpz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtweyvyuri.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ydjk.org.cn/gtqmvkbqxj.html

C#:   s.Replace("a", "b")
来源：http://hz.ydjk.org.cn/gtmcnzaniq.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtsdflyrpo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gaohongyu789.top/gtmmbtcffm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gtbonlmilw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.kuanghao11.cn/gtmgajzrvp.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtjxbmwfog.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cdnleiting.top/gtccfkrgpj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtpcvzxvva.html

Ruby: s.split(",");  s.split
来源：http://hz.andypj.xyz/gtziwrfzqq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydzc1.top/gtqfaycafn.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtyaclomsq.html

Py:   ",".join(items)
来源：http://hz.kuanghao11.cn/gtuuspcdfm.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtgvuygpha.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gthpzvhfxu.html

TS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtnqkowwkq.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtdtoqyhai.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtxjgmmrty.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gtuwpbvtxk.html

C#:   string.Join(",", items)
来源：http://hz.fzhhl.top/gtehkocuju.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gtmhlrqdrj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yj202588.top/gtogwhibdp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydjk.org.cn/gtzxgpfnqh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtqeewjfyv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtcqcdegsy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.vqdsnc.cn/gtaxdjghjw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtbkbnqrrd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtklejobmg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fzhhl.top/gtypvliwft.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtjursxzbw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xinyue.icu/gtbrgvgowx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenlongwang.top/gtkobtwurm.html

JS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtffpfjtaq.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtcdmadzkn.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gtyltpccgx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtasavmajl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtfukvgzuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtnzzumeal.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtdctbxfkd.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtpkpizsxm.html

PHP:  strrev($s);
来源：http://hz.hywenlv.cn/gtarosnkoe.html

JS:   [...s].reverse().join("")
来源：http://hz.chenjidiqi.icu/gtwrtbqugk.html

TS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtdxrlqufa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtllikhdxd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtdbgkrfvm.html

Ruby: s.reverse
来源：http://hz.wangdashe.top/gtjlipbtbo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yonumen.top/gthmvnjesx.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtbieghdyf.html

Py:   s.count("a")
来源：http://hz.nanxuanxn.top/gtcyjbxveo.html

PHP:  substr_count($s, "a");
来源：http://hz.zhijiandao.cn/gtvmuldlrp.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtlmcifwuf.html

TS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gteiunfmta.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gotoacloud.top/gttrgtxwch.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtcwmbsony.html

Ruby: s.count("a")
来源：http://hz.tian-w.cn/gtshbakbmj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.dashuyun.cn/gthvrwvwac.html

[E13] 逐字符遍历
来源：http://hz.yj20258.top/gtvxuqtvjm.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtwidlbree.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gogol.net.cn/gtihtmvgue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtxmlpfkbs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtkwbxqmhj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtvfsxetjg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxuanxn.top/gtpnnmwpvh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.smart0.xyz/gtginlxxbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydjk.org.cn/gtcdyhxvhm.html

[E14] URL 编码与 Base64
来源：http://hz.quarkkingdee.top/gtixmlkagh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtfefnophb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.birdmap.top/gtccubqzqm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtrfyifgnr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shuidangran.top/gthgxlexuf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhixingplan.top/gtuliljiqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtiuprnauj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtljipdvoo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.mhx1999.top/gtoiahbzyg.html

[E15] HTML 转义 / 反转义
来源：http://hz.yongpay.top/gthhppzgan.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.smart0.xyz/gtrktrcgiu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gtjzbewsmx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhiwuduotai.top/gtvaehkkim.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtutcntjgu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtzpvzzghr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shanyushiyangtech.top/gtyjajpwez.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gttmjavjsn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hfpthk.cn/gttrohkmjz.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtlqcyxslc.html

Py:   f"{1234567:,}"
来源：http://hz.cqqwz.cn/gtaleajkcs.html

PHP:  number_format(1234567);
来源：http://hz.sufxvd.cn/gtgmckogtt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtmjqvbnjm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnqzz.top/gtkmmjyklc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hammf.cn/gtdxrohbog.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtebodimzy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daria6918.cn/gtvfofpfvn.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangkeji.top/gtdftwjlpg.html

[E17] 首字母大写
来源：http://hz.svipenyu.cn/gtvzwxwmka.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtqhqvlvxq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtetrviqwq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtoirlsiwy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gtpnibihnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yueranfly.top/gtwwdtzfvy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtkkidxwrt.html

Ruby: s.capitalize
来源：http://hz.fzhhl.top/gtzzdezbjt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ivvv.top/gtmddiikgd.html

[E18] 模板占位符替换
来源：http://hz.nanxuanxn.top/gtnokhcevi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zdqjudy.top/gttpeslrtj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.pycfn.com/gtwoetdlpp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtaxlmjbok.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtpuzwexeo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtiwauavpg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zdqjudy.top/gteicpbkoe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtyiimnicn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnxiangtu.top/gthynpuzmq.html

[E19] 多行文本按行拆分
来源：http://hz.gotoacloud.top/gtdoghcaec.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtnguplcws.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cdnleiting.top/gtvxfrieye.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtxcsxroqi.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtfeypxshp.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtqyeggvah.html

Go:   strings.Split(s, "\n")
来源：http://hz.yuxming.cn/gtycskzggu.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtrbzouunv.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtcmrttgdw.html

[E20] 判断字符串是否为空
来源：http://hz.52xcode.cn/gtrxkdwnnj.html

Py:   if not s:
来源：http://hz.yongpay.top/gtqmxesuif.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtslfhlkvu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gtrfvqnyyj.html

TS:   if (s === "") {}
来源：http://hz.gogol.net.cn/gtagkntseh.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtbmafwrcz.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtneoaqsyn.html

Ruby: if s.empty?
来源：http://hz.chenlongwang.top/gtkgspoczb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tian-w.cn/gtmncfatzq.html

[E21] 超长截断加省略号
来源：http://hz.hammf.cn/gtanqgiihj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.feifeiyinyue.top/gtoddphhej.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtplofbhhq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtjhuinyok.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtxvokfcyj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtwgqzgkhj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtjyrczhbs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhengqikj.top/gtsagjpauh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cucudq.cn/gtscnywnsg.html

[E22] 字节长度与字符长度
来源：http://hz.feifeiyinyue.top/gtkcedyhhf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gogol.net.cn/gtcigqklgb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtnwnygubk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtqogcbuux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gtxfpsbjzz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.redwolf501.top/gtcakpfsgh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.0kj1m.cn/gtutmzwxmd.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtwvcwmdmr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtwvmdvfow.html

================================================================================
来源：http://hz.pycfn.com/gtfuwraote.html

F. 文件与目录
来源：http://hz.tianlin.xyz/gthdhnonxq.html

================================================================================
来源：http://hz.cashguo.top/gtrzyawdjo.html

[F01] 读取整个文件
来源：http://hz.316326.xyz/gtdrelzwkd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhaomingkeji.xyz/gtaomnrrpz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gteginqgmi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xingfuxueyuan.xyz/gtmwkvahom.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenzaomai.com/gtasdfujpi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtrazqhqgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gtjwshwprl.html

Ruby: File.read("a.txt")
来源：http://hz.daria6918.cn/gtuupcqqxz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tanke756.top/gtidpydowa.html

[F02] 逐行读取文件
来源：http://hz.gzhubu.top/gtqazdhaoy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gzhubu.top/gtrvhokkfq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangtech.top/gtgxgqhkwz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xinyue.icu/gtayehetvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zycfv.cn/gtozemlqes.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtigkapfbd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtadglpndd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yvedp.cn/gtayagcjyx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtdbwdgkps.html

[F03] 写入文件（覆盖）
来源：http://hz.birdmap.top/gthwmdbyzl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtdbjfvlry.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.mhx1999.top/gtvmffdfkf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtosummrzj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gotoacloud.top/gthdcnfbev.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhengqikj.top/gtmnfatwnh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jianghu66.top/gtdzhioegw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cdnleiting.top/gtdyathexw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xziqi.cn/gtvflvpptg.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtskckpjoe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hammf.cn/gtpoyaqxam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtwhdjtuam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtmfgmzxyn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtjowvnjmg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.svipenyu.cn/gtyklfmoaw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hammf.cn/gtvconjqwf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydzc1.top/gtlyedtjqc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.shangyingyoupin.top/gtuprjkgdp.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtsztwddpk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtrdwekdgb.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtxjwatneu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtaaemfnvl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtlpdktovv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtjmvxeyuj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.tianlin.xyz/gtrvemlxiq.html

Ruby: File.exist?("a.txt")
来源：http://hz.mhx1999.top/gtmjawfffb.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtnbdvfbhs.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtazpqoiih.html

Py:   os.remove("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtxczuousc.html

PHP:  unlink("a.txt");
来源：http://hz.xylfe.cn/gterxpvjxp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtokwhiivw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yuxming.cn/gtvbfoixmu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtaejfuyjt.html

Go:   os.Remove("a.txt")
来源：http://hz.kuanghao11.cn/gtxljxfiyb.html

Ruby: File.delete("a.txt")
来源：http://hz.gzhubu.top/gtcmxpjvqy.html

C#:   File.Delete("a.txt");
来源：http://hz.smart0.xyz/gtujhnykbq.html

[F07] 创建目录（含多级）
来源：http://hz.aibaodan.cn/gtviowwobj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.9152youxi.cn/gtxwbjlhmi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtehvhagqp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jqgufenzy.top/gtexznuwec.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtepybwecc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jqgfzy.top/gtqfnleowg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtkwomefjz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guowangkeji.top/gtdztrvtqm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hysaishi.cn/gtjpmdgyij.html

[F08] 遍历目录
来源：http://hz.cheryme.top/gtguwxdodh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sysykeji.top/gtzqgjsjoy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yonumen.top/gthyclzypj.html

JS:   fs.readdirSync("dir")
来源：http://hz.aibaodan.cn/gtxayebsjp.html

TS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gthtbaomvu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtoeglfytk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtqxpilcic.html

Ruby: Dir.children("dir")
来源：http://hz.kuanghao11.cn/gtlfxgnoir.html

C#:   Directory.GetFiles("dir")
来源：http://hz.meibo888.top/gtbwovarxh.html

[F09] 获取文件大小
来源：http://hz.pycfn.com/gtkskrymvu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtkotaoyag.html

PHP:  filesize("a.txt");
来源：http://hz.hnxiangtu.top/gtnysvetxx.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtvuiycnuk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gttrcfykam.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtzruxawds.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtlqwfxelj.html

Ruby: File.size("a.txt")
来源：http://hz.dianchejie.cn/gtsqwkpmjh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xingfuxueyuan.xyz/gtfmowrhxk.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gtkrdnibon.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtbjiozdhg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.dianchejie.cn/gtakivvwfn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dianchejie.cn/gtvxixtbsf.html

TS:   path.extname("a.txt")
来源：http://hz.zhengqikj.top/gtskkfmmdp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.gzhubu.top/gthwahdsmb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yuxming.cn/gthbelmqql.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtewuiifrq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hammf.cn/gteqzddvyg.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gtynnoptvm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtzqrsftgi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.aizwys.cn/gtjaxbvinw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtuxphwquz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigfzy.top/gtppgywokv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yonumen.top/gtpwjnpzsb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.daria6918.cn/gtcghgkmhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtlvofwhkd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shangyingyoupin.top/gtstxoqumf.html

[F12] CSV 读写
来源：http://hz.yj202588.top/gtpqgdukwe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.0kj1m.cn/gtgpdkstbi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nanxuanxn.top/gtjyvdniqa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ppjwa.cn/gtrkgewnfs.html

TS:   // 同上
来源：http://hz.hfpthk.cn/gtwmcfozfi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ehwqpu.com/gtznwkjcvq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.haohaochexian.top/gtoupcpewz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gtrufkxjbh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yj20258888.top/gtbsywasun.html

================================================================================
来源：http://hz.hammf.cn/gtmbvpolao.html

G. 面向对象
来源：http://hz.ydzc1.top/gthhzfkbsy.html

================================================================================
来源：http://hz.yangfankeji.com/gtyqektuqb.html

[G01] 定义类
来源：http://hz.havefunace.top/gtrqwtudoa.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtfslnpqix.html

PHP:  class User {}
来源：http://hz.hnxiangtu.top/gthmhxbzdy.html

JS:   class User {}
来源：http://hz.shzxlz.cn/gtjoqrhdfp.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtfsabmoio.html


<!-- 参考信息 -->