代发 wailian999

[E02] 重复字符串
来源：http://hz.gzhubu.top/gtjbaaxszf.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtrfueezvq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtqsiqynye.html

JS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gtoohbeaei.html

TS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtizgjvqen.html

Java: "ab".repeat(3)
来源：http://hz.yj20258888.top/gttzridqvp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtifqgqcug.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtdznhkkbb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtajoshxuy.html

[E03] 截取子串
来源：http://hz.ybcxt.top/gtablodizd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtqeciwcyv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gtpxhxztvd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.52xcode.cn/gtqdngpffg.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtfjjtutrr.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtmeswrcsj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhongyouzk.top/gtymzmgjmd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ivvv.top/gtoyhksxpb.html

C#:   s.Substring(1, 3)
来源：http://hz.ppjwa.cn/gtpgvaedyc.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtahaklxll.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtuffxldvd.html

PHP:  strpos($s, "x");
来源：http://hz.yangfankeji.com/gtyefkfbes.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtexhfpstk.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gteexrfxog.html

Java: s.indexOf("x")
来源：http://hz.svipenyu.cn/gtpmhemlgh.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtcsycehbc.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtzhtqtouu.html

C#:   s.IndexOf("x")
来源：http://hz.iojbl.cn/gtengyiauk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shangyingyoupin.top/gttsrezcto.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtgkowcyps.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.meibo888.top/gtcrmqkcwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtdjxfkpjt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenlongwang.top/gtzfhbbkwb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtpbusqmis.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yanxiufei.cn/gtezqxbiyx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tian-w.cn/gtskqnezdx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258888.top/gtotllvpcj.html

[E06] 替换子串
来源：http://hz.pycfn.com/gtssxmtghr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.meibo888.top/gtkruymgea.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.snrcjt.cn/gtitgpfgpa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gthsagynis.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtfkggtbkm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtndqgswtd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtoeyzwocw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jiagoushi.top/gtpineydzh.html

C#:   s.Replace("a", "b")
来源：http://hz.zhongyouzk.top/gtfpnfuyms.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtslqcifii.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtdthsbbrh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtmdswhlnc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydzc1.top/gtbxbpfglu.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gthyglromi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangtech.top/gtnijmmaro.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hysaishi.cn/gtmvhzprit.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxuanxn.top/gtottymdjx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shuidangran.top/gtmcvspvvp.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtbabydxho.html

Py:   ",".join(items)
来源：http://hz.yvedp.cn/gtvhlmwyyq.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtejdlaxxt.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtrbdnqcmx.html

TS:   items.join(",")
来源：http://hz.zhixingplan.top/gthudqklor.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtinrgsevz.html

Go:   strings.Join(items, ",")
来源：http://hz.quarkkingdee.top/gtqrcvjxyz.html

Ruby: items.join(",")
来源：http://hz.tanke756.top/gtdvutifso.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtwugfxgky.html

[E09] 去除所有空白字符
来源：http://hz.hfpthk.cn/gtfadnocvq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cdnleiting.top/gteoavannp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtbhbrspxm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtlbtcrflc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtaoaqrind.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zycfv.cn/gtzjpqugsl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtmanqpscd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gogol.net.cn/gtvhffatoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtqczfmnln.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtcmaxkgrx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sysykeji.top/gtijqifjvn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtrtkexwby.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhoulong.xyz/gtovibnfwe.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenlongwang.top/gtxlawlvnb.html

Java: String.format("%03d", 7)
来源：http://hz.yangfankeji.com/gtttrdhgkd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yueranfly.top/gtnndvpcyh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.mhx1999.top/gtywgmfbat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cucudq.cn/gtghptyxjb.html

[E11] 反转字符串
来源：http://hz.kuanghao11.cn/gtnpjqtpmm.html

Py:   s[::-1]
来源：http://hz.svipenyu.cn/gtrniyfwra.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gtuxbmjzzc.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtqirppjdh.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtzmmywghe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigfzy.top/gtrqshrfes.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yuanzhike.top/gtfhnvgwhu.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtkzqwwjfw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jianghu66.top/gtmcsqjmzu.html

[E12] 统计某字符出现次数
来源：http://hz.c1oappe.top/gtsirotpne.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtmgfpmckw.html

PHP:  substr_count($s, "a");
来源：http://hz.snrcjt.cn/gtkhskflyp.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtclodpyvz.html

TS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtqjrdkbyh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtislchuab.html

Go:   strings.Count(s, "a")
来源：http://hz.tanke756.top/gtitbdvnww.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtgoymlprk.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cashguo.top/gtjmludjgt.html

[E13] 逐字符遍历
来源：http://hz.tanke756.top/gtjiociyii.html

Py:   for ch in s: print(ch)
来源：http://hz.xingfuxueyuan.xyz/gtwpndbsmp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jyoumei.cn/gtlwqrdfcy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtitegasxh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtcdowunhw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guannengcc.top/gtvfhcmcsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.smart0.xyz/gtaqaprujy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shuidangran.top/gtuwmdtnxg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtjtguswqg.html

[E14] URL 编码与 Base64
来源：http://hz.pycfn.com/gtwqamrvnp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtfhfibuaw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtmtwmkqgp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gteorkiukj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtulurnsti.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtbfoiguyx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnxiangtu.top/gtafjsqokq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtahzpepgw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.meibo888.top/gtjmqoqhya.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhixingplan.top/gthmglkzvd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gzhubu.top/gtkvzbagtv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gttazteczi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtbvhozkjd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gthrrpggcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtwzmpyhod.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258888.top/gtpvttrqvh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tanke756.top/gtiiuapllf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yvedp.cn/gtkfyxtdib.html

[E16] 数字千分位
来源：http://hz.zhengqikj.top/gtnrjhrpkx.html

Py:   f"{1234567:,}"
来源：http://hz.dianchejie.cn/gtvggdimkd.html

PHP:  number_format(1234567);
来源：http://hz.yangfankeji.com/gtykekhqdl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtliuyysfl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtinnywhip.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pycfn.com/gtzmaabuaa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shangyingyoupin.top/gtomogtaoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258.top/gtlbckwyom.html

C#:   1234567.ToString("N0")
来源：http://hz.yj20258.top/gtmztimjrw.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtrctgqxht.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtzqlhyekb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daxiang520.top/gtrqcxbkgk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtyfrvcnqh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtyufmyqam.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtarbchtuk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fengsongda.top/gtfmujltwx.html

Ruby: s.capitalize
来源：http://hz.mhx1999.top/gtnmjszrft.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtqqnoqcaq.html

[E18] 模板占位符替换
来源：http://hz.yanxiufei.cn/gtltmjxayp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xingfuxueyuan.xyz/gtoxsawcwd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hysaishi.cn/gtqcyduibr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.birdmap.top/gtnltmeyoz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtcggmzntl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigfzy.top/gtzrpznjgl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.havefunace.top/gtybwnnodx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cdnleiting.top/gtebrqulbl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.quarkkingdee.top/gtfoyfcvao.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gteodxzrgc.html

Py:   s.splitlines()
来源：http://hz.birdmap.top/gthvbsvsch.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtufypllpc.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtturvbzwo.html

TS:   s.split(/\r?\n/)
来源：http://hz.shangyingyoupin.top/gtofaaqdqu.html

Java: s.lines().toList()
来源：http://hz.yongpay.top/gtphlruuum.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtdtepuawo.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtyzgtktjy.html

C#:   s.Split('\n')
来源：http://hz.sysykeji.top/gteyusxlvr.html

[E20] 判断字符串是否为空
来源：http://hz.pycfn.com/gthxkrbukw.html

Py:   if not s:
来源：http://hz.haohaochexian.top/gtouwogiwk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.feifeiyinyue.top/gtgxfejeyf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shangyingyoupin.top/gtggznyahz.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtckxoukxc.html

Java: if (s.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gthlanvqaw.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gtowdquewd.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtgvuuinrm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gtrfoiaxuu.html

[E21] 超长截断加省略号
来源：http://hz.yanxiufei.cn/gtkqekrsyl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhiwuduotai.top/gtzgwrguce.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.bjfxy.top/gtyuhycmis.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtksskavzb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtwozuvkcp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtbwpztyor.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fzhhl.top/gtalduavrg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.bjfxy.top/gtjkrumchu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guannengcc.top/gtzkrgjswv.html

[E22] 字节长度与字符长度
来源：http://hz.yj202588.top/gtwuowwtly.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.feifeiyinyue.top/gtguyinycb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258.top/gtlnqydsen.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtinuuoctu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtdqnlghya.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gteawlelmg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigfzy.top/gtucyuguno.html

Ruby: s.bytesize;  s.length
来源：http://hz.fengsongda.top/gtfdisfqxd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gthqyswbdl.html

================================================================================
来源：http://hz.shzxlz.cn/gtbeadxyac.html

F. 文件与目录
来源：http://hz.havefunace.top/gttvrspvrd.html

================================================================================
来源：http://hz.sysykeji.top/gtcuydeiah.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gteishnvys.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cucudq.cn/gtaipzoftp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.haohaochexian.top/gteblkedtj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hnqzz.top/gtmjwauaki.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtjzyydhgk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtgdjcguhx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtcmcyxeeu.html

Ruby: File.read("a.txt")
来源：http://hz.iojbl.cn/gtanginyxw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gtyufrzflk.html

[F02] 逐行读取文件
来源：http://hz.0kj1m.cn/gtahlhllte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yongpay.top/gtxfmkjxek.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtemienrce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtnumjknjn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtsdapgjvm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtajytftpe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtydohaqeo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258.top/gtyropekat.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ehwqpu.com/gtowdlywmj.html

[F03] 写入文件（覆盖）
来源：http://hz.jyoumei.cn/gtjucvtjah.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtogceuxxk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtgdtcunzg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cdnleiting.top/gtwqkcscae.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtrdrzrvgh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtwnonwjyn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtptelzzjh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtplchupaf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtgahdjdfi.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtspikjbhf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.shanyushiyangkeji.top/gtaxhtrfdr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xinyue.icu/gtddqyfvmf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.mhx1999.top/gtaoqpshuz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtiexubotx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.fzhhl.top/gtlzwwyjac.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.sufxvd.cn/gtpqpuamdg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtcnqptbib.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pycfn.com/gtoktddhyo.html

[F05] 判断文件或目录是否存在
来源：http://hz.316326.xyz/gtfubsfkqu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pengpengdd.cyou/gtmtlypqos.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtjrkmfggz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gttvopqqtt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yanxiufei.cn/gtqwdjuely.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtlvowvcys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shuidangran.top/gthgrqipdq.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtbrwkqrjs.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gtdjdsvoew.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtwrvergxt.html

Py:   os.remove("a.txt")
来源：http://hz.yueranfly.top/gtdxhwswyq.html

PHP:  unlink("a.txt");
来源：http://hz.birdmap.top/gtpmvgjhbd.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtsgvjxiyw.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yangfankeji.com/gtyvqvizdf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtyicamdrq.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtouqurgow.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gtrrxgklvy.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtxvdmfzqu.html

[F07] 创建目录（含多级）
来源：http://hz.feifeiyinyue.top/gtlllxbtdz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yueranfly.top/gtfnkmsply.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.redwolf501.top/gtpswlbfke.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.mhx1999.top/gtzlexsuql.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtasfnjrxi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.chenzaomai.com/gtzxqwzujv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.316326.xyz/gtzoekvzcq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.smart0.xyz/gtbtoswmla.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.meibo888.top/gttiwxzjui.html

[F08] 遍历目录
来源：http://hz.sufxvd.cn/gtlggymftt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.meibo888.top/gtcdqksign.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tanke756.top/gtmfvvwodh.html

JS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtpybiwlsn.html

TS:   fs.readdirSync("dir")
来源：http://hz.zdqjudy.top/gtfgbjzher.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gttfgyzvxa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuanzhike.top/gthmwlyaaq.html

Ruby: Dir.children("dir")
来源：http://hz.jlsjyb.cn/gtpmkduwdo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhixingplan.top/gtjfwhvpip.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtygotsrck.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gttjrmedfv.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gtepteuwkt.html

JS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtfoqrrqjz.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yj20258888.top/gtydcpfkbq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtxytijauh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.snrcjt.cn/gtcwtiyrqe.html

Ruby: File.size("a.txt")
来源：http://hz.dashuyun.cn/gtsnhpdyqp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.smart0.xyz/gtotucijvl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hongshengwenyu.top/gteqreejyu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.ppjwa.cn/gtxbiggmex.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yvedp.cn/gtyjdnskhz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.iojbl.cn/gtvmilimut.html

TS:   path.extname("a.txt")
来源：http://hz.nwbrower.top/gtwogtkxpj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zdqjudy.top/gtlmwsndth.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ywan-chungtsiang.top/gtruxwbbzp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtquftpbjt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.ehwqpu.com/gtzqbvfgqw.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtofidpznt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtjtqltkva.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.meibo888.top/gtnltxbicy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtfrpbrnnq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtabssapzs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.bjfxy.top/gtahikfcca.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shanyushiyangtech.top/gtzrlpxmmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtrgqekgqj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.0kj1m.cn/gtdtbgipeo.html

[F12] CSV 读写
来源：http://hz.feifeiyinyue.top/gtmyysbils.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtypoewmoy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenjidiqi.icu/gthlbpdera.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.gaohongyu789.top/gteiyavvuc.html

TS:   // 同上
来源：http://hz.ydjk.org.cn/gtnawewqcr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gtsotdrudg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xinyue.icu/gttvtdrubp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.birdmap.top/gtyquuyzft.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yangfankeji.com/gttvsfnear.html


<!-- 参考信息 -->