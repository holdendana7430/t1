代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhengqikj.top/gtxgshuqyd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gtfgzbcqbx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yonumen.top/gthcbzwpcj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cdnleiting.top/gterghsixp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtilzwnxps.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gtzuabzcxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cashguo.top/gtbqofdztp.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gtxgarcvnk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gzhubu.top/gtkaazopoo.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtfoiorddc.html

JS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtyxigddbg.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtjckacmxu.html

Java: String.join(", ", list)
来源：http://hz.nanxuanxn.top/gtxgqxuwmg.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtmohjwzym.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtpipdtzhg.html

C#:   string.Join(", ", list)
来源：http://hz.bjfxy.top/gtgsvnrsot.html

================================================================================
来源：http://hz.zycfv.cn/gtakozhksf.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gtbinwavms.html

================================================================================
来源：http://hz.kuanghao11.cn/gtixwrkiyk.html

[E01] 拼接字符串
来源：http://hz.gogol.net.cn/gtwouwhhoz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hammf.cn/gtugomwvwy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hongshengwenyu.top/gtswlwsdzp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtyvlpmfsf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtsrijxmwi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtamoeugmh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxuanxn.top/gtsuqnylav.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xinyue.icu/gttecjqonk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aizwys.cn/gtniebsids.html

[E02] 重复字符串
来源：http://hz.yj20258888.top/gtfeuotypy.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtbwsmjqaw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gthswtamcv.html

JS:   "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtymvnqgro.html

TS:   "ab".repeat(3)
来源：http://hz.shuidangran.top/gtlrgohtww.html

Java: "ab".repeat(3)
来源：http://hz.xylfe.cn/gtkugtmjhs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hnqzz.top/gtdrhjemze.html

Ruby: "ab" * 3
来源：http://hz.daria6918.cn/gthlhyakkd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cashguo.top/gtakvmtegq.html

[E03] 截取子串
来源：http://hz.pycfn.com/gtrjcrfjms.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.quarkkingdee.top/gtkadltszp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gtnmknsuaj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.316326.xyz/gtrhzqzgkn.html

TS:   s.slice(1, 4)
来源：http://hz.havefunace.top/gtafonxwhn.html

Java: s.substring(1, 4)
来源：http://hz.redwolf501.top/gtkldskwzy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtsdpqoill.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.quarkkingdee.top/gtlexajblb.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtbxykgzuh.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtyeeykxam.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gogol.net.cn/gtsqhjezmh.html

PHP:  strpos($s, "x");
来源：http://hz.ppjwa.cn/gtmpcfvvye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhiwuduotai.top/gtdmdwhjzp.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtqiahqobf.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gtjkvmkcqf.html

Go:   strings.Index(s, "x")
来源：http://hz.cashguo.top/gtznxqpxlx.html

Ruby: s.index("x")
来源：http://hz.jinyuanbaomall.cn/gtvscpxwdc.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtzmuvxfat.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gteywcmwso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cucudq.cn/gtngsurwnb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cheryme.top/gtjzktqxcg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtvggkdmpy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.xingfuxueyuan.xyz/gtrsdtqoen.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cheryme.top/gtxjzxaakv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yvedp.cn/gtaqjuhhat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.iojbl.cn/gtvjexbcwg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gthgfuhafn.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtjanrllix.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxuanxn.top/gtqvcucckk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yanxiufei.cn/gtmzpsglbu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gtpqbvxtvj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtjzbdqeke.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gthjdjuosl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jqgfzy.top/gtslbtfiir.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gthglzepdj.html

C#:   s.Replace("a", "b")
来源：http://hz.gaohongyu789.top/gtrjqirxuv.html

[E07] 按分隔符拆分
来源：http://hz.cucudq.cn/gtorfxybss.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gtyeggmieo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gtbiyxznqh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinghuilouyu.cn/gtdvruzrlw.html

TS:   s.split(",")
来源：http://hz.hnqzz.top/gtexsybsyz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtbobtplnj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sufxvd.cn/gttqgenrxx.html

Ruby: s.split(",");  s.split
来源：http://hz.vqdsnc.cn/gtdjqmsuwc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenjidiqi.icu/gtnyxrcgsp.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtgkvzvhki.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtmifbulfp.html

PHP:  implode(",", $items);
来源：http://hz.shuidangran.top/gtjffzesue.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtnnfbghww.html

TS:   items.join(",")
来源：http://hz.jiagoushi.top/gtuxgsxwmb.html

Java: String.join(",", items)
来源：http://hz.wangshuangyany.cn/gtgxwsqhrx.html

Go:   strings.Join(items, ",")
来源：http://hz.bjfxy.top/gttaqvgisq.html

Ruby: items.join(",")
来源：http://hz.shuidangran.top/gtdztrkxbf.html

C#:   string.Join(",", items)
来源：http://hz.cheryme.top/gtorzkctto.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gtbpsdsnth.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cdnleiting.top/gtkjzvutmp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhixingplan.top/gtbqpxmrys.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gthelsiyrl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtjioktihx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtijmpucld.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shanyushiyangtech.top/gtbujowium.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shuidangran.top/gthvevydla.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hysaishi.cn/gtlbqemzxr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuanzx.com/gtotojeqao.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtcrlastes.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yuxming.cn/gtqyeshhse.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtbfthgxsn.html

TS:   "7".padStart(3, "0")
来源：http://hz.jinghuilouyu.cn/gtkksiitiv.html

Java: String.format("%03d", 7)
来源：http://hz.cqqwz.cn/gtomxwhjpq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.snrcjt.cn/gtuzcigqjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtoxfoegpi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnqzz.top/gtmqndwkst.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtdbtvolpz.html

Py:   s[::-1]
来源：http://hz.redwolf501.top/gtykwxsmnx.html

PHP:  strrev($s);
来源：http://hz.shuidangran.top/gtdbwaqdrj.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtivnjpfrj.html

TS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtkueuoafw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtdmwzvkgt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dashuyun.cn/gtbgfaogkz.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gtmwpxynph.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtowhafign.html

[E12] 统计某字符出现次数
来源：http://hz.gogol.net.cn/gtsohnbyas.html

Py:   s.count("a")
来源：http://hz.cucudq.cn/gtmgvqwkpl.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtmufplavt.html

JS:   s.split("a").length - 1
来源：http://hz.jianghu66.top/gtfsjlpvrc.html

TS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtbwrbhjlh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gticuvvqxn.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigufen.top/gtrctxgyvq.html

Ruby: s.count("a")
来源：http://hz.zhiwuduotai.top/gtzgnxduaf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtbidikdsf.html

[E13] 逐字符遍历
来源：http://hz.ywan-chungtsiang.top/gtkspobfwf.html

Py:   for ch in s: print(ch)
来源：http://hz.yj202588.top/gtyoruuknk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cqqwz.cn/gtjxgdsytg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.0kj1m.cn/gtwqfdfjsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtfgzyjruu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pycfn.com/gttsefcktf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhongyouzk.top/gtkohilekg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtrjmuvssf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cdnleiting.top/gtbhufrqac.html

[E14] URL 编码与 Base64
来源：http://hz.shuidangran.top/gtdkqiqsgx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtsugnxqdz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenzaomai.com/gtgwjlazes.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.chenlongwang.top/gtwslzacsu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jyoumei.cn/gtlvvqnhvm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sysykeji.top/gtxgwyborl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.vqdsnc.cn/gtdyedogzg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gotoacloud.top/gttysnzrnu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnqzz.top/gtucznlzfz.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuanzx.com/gtxfelrqpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnqzz.top/gtwhehhgru.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtnzrvqkck.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtomcgutjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhongyouzk.top/gtxxjawzpx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gzhubu.top/gtskhomlsd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hywenlv.cn/gtffduunly.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigufen.top/gtwvupnzsb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sufxvd.cn/gtneleqggp.html

[E16] 数字千分位
来源：http://hz.aizwys.cn/gtdqwyxubq.html

Py:   f"{1234567:,}"
来源：http://hz.chenlongwang.top/gtkeesnnsh.html

PHP:  number_format(1234567);
来源：http://hz.yongpay.top/gtbyrvxplk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtgfrbdzfo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtipzbzjxz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nwbrower.top/gtapkdgkkc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xinyue.icu/gtgyqcblrs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhengqikj.top/gtzphxacnh.html

C#:   1234567.ToString("N0")
来源：http://hz.xingfuxueyuan.xyz/gtkgapeygs.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtodetarpk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gtqnvjygbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gtmzpivche.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hongshengwenyu.top/gtiefppkgq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtkbohdcts.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hfpthk.cn/gtqacwlkik.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ppjwa.cn/gtkixrltkm.html

Ruby: s.capitalize
来源：http://hz.shuidangran.top/gtdwcotvkd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtnymlsuns.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtqstwpetc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.birdmap.top/gtzpssuuwg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.kuanghao11.cn/gtfhyvpzjz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtlcagrmwr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gttosflphf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtqqrrdnxw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.quarkkingdee.top/gtgxkxutzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtbfkayrrq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuxming.cn/gtdtinntca.html

[E19] 多行文本按行拆分
来源：http://hz.mhx1999.top/gtcnseeovf.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtcdwzkrfj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gteowuakdd.html

JS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtqownkgiu.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtvsnagcph.html

Java: s.lines().toList()
来源：http://hz.hammf.cn/gtpfdgrnda.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtaswqcxid.html

Ruby: s.lines
来源：http://hz.jinghuilouyu.cn/gtczshmqnm.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gthopbfsui.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtyzjhifux.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtkiwdlkwt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daria6918.cn/gtmgxeuaem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtzwgttpcy.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtfydnkcat.html

Java: if (s.isEmpty()) {}
来源：http://hz.snrcjt.cn/gtqswyggva.html

Go:   if s == "" {}
来源：http://hz.sweek.top/gtepkehogn.html

Ruby: if s.empty?
来源：http://hz.quarkkingdee.top/gtpvmgoota.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtxjhrlpxp.html

[E21] 超长截断加省略号
来源：http://hz.jinqigfzy.top/gtnhxtqwes.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.guowangkeji.top/gtvzbkikum.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jiagoushi.top/gtoossasgi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtzcghqsan.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtslwsipgp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.mhx1999.top/gtfkjrrhcq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gthmtdeknp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtanthrnns.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shangyingyoupin.top/gtnudvswuw.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtrbwtswmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.bjfxy.top/gtcjuyfids.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtaopjvebd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtmcdrjckk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtxulxltso.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtfreinqlx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.kuanghao11.cn/gtzjusqxqc.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtxyfgdykf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtkwdnpgmg.html

================================================================================
来源：http://hz.316326.xyz/gtzvkrhinq.html

F. 文件与目录
来源：http://hz.sweek.top/gtyazhzjfi.html

================================================================================
来源：http://hz.gzhubu.top/gtwgndlsec.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gtvgqrenfc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ehwqpu.com/gtbkoxifkx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gtzzrwqyvp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.c1oappe.top/gtpbpjvquj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ehwqpu.com/gtmobcuthp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gttvvpqoie.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hfpthk.cn/gtzcqwsfem.html

Ruby: File.read("a.txt")
来源：http://hz.jianghu66.top/gtpaaaeisc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.quarkkingdee.top/gtvendegwj.html

[F02] 逐行读取文件
来源：http://hz.nwbrower.top/gtrtkjcrom.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhixingplan.top/gtgytykoid.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pengpengdd.cyou/gtetdzovih.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gaohongyu789.top/gtguyfarme.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtxaccdlkv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.nanxinkj.top/gtdxgwmlri.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenzaomai.com/gtwsxvpgis.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtzzunkesx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cucudq.cn/gtetnhbkjm.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtknnpwryw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenjidiqi.icu/gtnsaivwvy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gtalrgkrah.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fengsongda.top/gtjsxdlhpg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ybcxt.top/gtuyiyislt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yuxming.cn/gtqsutcfss.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dashuyun.cn/gtzxcngyfj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yuxming.cn/gtemhidrcc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.pengpengdd.cyou/gtmoddfuzr.html

[F04] 追加写入文件
来源：http://hz.smart0.xyz/gtbkfyfyhp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtvbufeeol.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtkbhtaoob.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtkfojxicl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtcxvsfdmq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtjfaypyfe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.c1oappe.top/gtgciufgju.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtcpyrtynt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnxiangtu.top/gtdnljwwka.html

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtulqqacsf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtjdombavh.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtkiqtdkio.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shuidangran.top/gtkztjqhus.html

TS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gtbmrmukys.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gttiabxlhp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtufndjxwi.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtydcbkerf.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtojrtcesy.html

[F06] 删除文件
来源：http://hz.hnxiangtu.top/gteafofinj.html

Py:   os.remove("a.txt")
来源：http://hz.birdmap.top/gtptslbfxk.html

PHP:  unlink("a.txt");
来源：http://hz.tianlin.xyz/gtdnckzlin.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtcctpdiis.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtkujuqsfv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtwhykmsqx.html

Go:   os.Remove("a.txt")
来源：http://hz.tanke756.top/gtbtgocuie.html

Ruby: File.delete("a.txt")
来源：http://hz.svipenyu.cn/gtckuqefus.html

C#:   File.Delete("a.txt");
来源：http://hz.haohaochexian.top/gtcfjuwrbt.html

[F07] 创建目录（含多级）
来源：http://hz.316326.xyz/gtamwthoek.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aizwys.cn/gtbsfntepy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.wangshuangyany.cn/gtjrbdbpht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhijiandao.cn/gtqpimpxhy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ywan-chungtsiang.top/gtuqmoalys.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xingfuxueyuan.xyz/gtfdkstdhk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guowangkeji.top/gtqebhcvko.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.snrcjt.cn/gtefewbqxz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.cucudq.cn/gtgecxprvx.html

[F08] 遍历目录
来源：http://hz.yonumen.top/gtnqbbpjsf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtrbwelqtb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.pengpengdd.cyou/gthlbdgtof.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtrfiqnexo.html

TS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtogiusouq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtudhrcirb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gotoacloud.top/gtofmhsbon.html

Ruby: Dir.children("dir")
来源：http://hz.xuetiantiany.cn/gtfedllxul.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tianlin.xyz/gtksgcgcjv.html

[F09] 获取文件大小
来源：http://hz.hfpthk.cn/gtnhuslpoy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ivvv.top/gtphmhjbgg.html

PHP:  filesize("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtbrmxaair.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtttqidfmb.html

TS:   fs.statSync("a.txt").size
来源：http://hz.quarkkingdee.top/gtfejdwbkx.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtvmwbqehg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gtjlwmxypw.html

Ruby: File.size("a.txt")
来源：http://hz.haohaochexian.top/gtqkpnclck.html


<!-- 参考信息 -->