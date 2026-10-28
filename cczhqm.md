代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuanzx.com/gtbgbknypq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenzaomai.com/gtpzhyeeby.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxinkj.top/gtyaknocgt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gttapvhokn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtldhtooqz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.svipenyu.cn/gtkuajvgme.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gttiwicqfc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtjnwrrtic.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.birdmap.top/gthrnacblv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fzhhl.top/gtnlhljjiy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.kuanghao11.cn/gtyhewwikw.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtfrqbuedj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtyhrtqpxr.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtpijzuqvd.html

JS:   arr.join(", ")
来源：http://hz.yongpay.top/gtejdwvxpw.html

TS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtezlwfqic.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtlgjmbprn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daria6918.cn/gtkuloxdxb.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtidaoqbfp.html

C#:   string.Join(", ", list)
来源：http://hz.yuxming.cn/gtxxowosei.html

================================================================================
来源：http://hz.yuanzhike.top/gtrtposfmv.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtoddlnmku.html

================================================================================
来源：http://hz.cheryme.top/gttqsqekik.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtyrpabtoo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangtech.top/gtycaltwqu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhaomingkeji.xyz/gtceddlkug.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gteuacnnuz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtlgtoadae.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhixingplan.top/gtbmgzzbwt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yangfankeji.com/gtrbcmxzse.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.chenjidiqi.icu/gtqnjbpjxb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sweek.top/gturalxjnh.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtouxeiffj.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gtpabbpckj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ppjwa.cn/gtadaeople.html

JS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtswlenuyt.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtdrnsubtr.html

Java: "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtntrgnqfv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhengqikj.top/gtdikgcklc.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtbqnliszu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtnrniabuu.html

[E03] 截取子串
来源：http://hz.yanxiufei.cn/gtzoevcnht.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daxiang520.top/gtwexgycwz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtvkselclz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtazfpvtlj.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtovrsjqzu.html

Java: s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtyrpbfhhc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhongyouzk.top/gtvjaazfps.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gthwaromnn.html

C#:   s.Substring(1, 3)
来源：http://hz.sufxvd.cn/gtjzpwwkqm.html

[E04] 查找子串位置
来源：http://hz.hywenlv.cn/gtfigojwhr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtzxcztkau.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gtimutaxhg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.gaohongyu789.top/gtovglcwua.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtkylegdsk.html

Java: s.indexOf("x")
来源：http://hz.zycfv.cn/gtcsvpggno.html

Go:   strings.Index(s, "x")
来源：http://hz.snrcjt.cn/gtspuckhqi.html

Ruby: s.index("x")
来源：http://hz.zhongyouzk.top/gtkvitkghj.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtjprlkdzl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.0kj1m.cn/gthjvrcgqo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtuyrbcncw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gtcvpmmqkl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtciufwudi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.quarkkingdee.top/gtyzfbjfga.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hfpthk.cn/gtmvteumhj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sweek.top/gtpofzuelm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtwctvfvan.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydzc1.top/gtbvibyimq.html

[E06] 替换子串
来源：http://hz.wangshuangyany.cn/gteeuovuep.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hfpthk.cn/gtiarojjds.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.vqdsnc.cn/gtujmnegad.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtqpstfsdt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtfaolovqs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtaehdyajx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhixingplan.top/gtmcnrchhf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.guannengcc.top/gtfxpnjarp.html

C#:   s.Replace("a", "b")
来源：http://hz.hammf.cn/gtwfcjlrjf.html

[E07] 按分隔符拆分
来源：http://hz.xylfe.cn/gtkaiysmbd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jiagoushi.top/gtcuagtrix.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtsswlczhh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hfpthk.cn/gtxmvmuswu.html

TS:   s.split(",")
来源：http://hz.pycfn.com/gtcqgofhhf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zdqjudy.top/gtivletvrw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pycfn.com/gtggcedmgc.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtkpeqluhn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cashguo.top/gtdtinbcew.html

[E08] 数组按分隔符合并
来源：http://hz.gogol.net.cn/gtvhpvikib.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gtotjmyujz.html

PHP:  implode(",", $items);
来源：http://hz.xinyue.icu/gtvepezhrk.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtbwtwwonh.html

TS:   items.join(",")
来源：http://hz.gotoacloud.top/gtxrzrfcrt.html

Java: String.join(",", items)
来源：http://hz.svipenyu.cn/gtyssbwqoy.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtoxvnshkt.html

Ruby: items.join(",")
来源：http://hz.0kj1m.cn/gthpdzdrnk.html

C#:   string.Join(",", items)
来源：http://hz.chenjidiqi.icu/gtfusuheat.html

[E09] 去除所有空白字符
来源：http://hz.zhengqikj.top/gtkeuacfsp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigfzy.top/gthxidjqit.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.feifeiyinyue.top/gtqwtndxjc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxuanxn.top/gtgidduahr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtinevygpc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtcaskprur.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xziqi.cn/gtopxtnkzk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jianghu66.top/gtozrabibj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gthdnkrhsy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yanxiufei.cn/gtvtqoudyn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jyoumei.cn/gttzyxwdny.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtfjrybneo.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gthlhktvmz.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtubboqxit.html

Java: String.format("%03d", 7)
来源：http://hz.birdmap.top/gtcdncvpaf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtgyzfisya.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtebvdrxga.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinghuilouyu.cn/gtskuzxscs.html

[E11] 反转字符串
来源：http://hz.ehwqpu.com/gtvyykuuuf.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtdqcqauzq.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtctefjtqq.html

JS:   [...s].reverse().join("")
来源：http://hz.shuidangran.top/gtuoztvudd.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtuobizbsf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xziqi.cn/gtiofmsdxk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shanyushiyangkeji.top/gtjmqbsayh.html

Ruby: s.reverse
来源：http://hz.bjfxy.top/gtrehuwonc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gtumewxkce.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtwsgepbrw.html

Py:   s.count("a")
来源：http://hz.xinyue.icu/gtyrlbwney.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtmkfzygqd.html

JS:   s.split("a").length - 1
来源：http://hz.tian-w.cn/gtrwnthqyz.html

TS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtiivvmayh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtroxjbtkx.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtznmdmutb.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtbmpfutgj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.aibaodan.cn/gtwtgksobq.html

[E13] 逐字符遍历
来源：http://hz.wangshuangyany.cn/gtlpahpehk.html

Py:   for ch in s: print(ch)
来源：http://hz.xylfe.cn/gtqddnsdvv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ywan-chungtsiang.top/gtnlxziiqk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenlongwang.top/gtpdtnhktc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xylfe.cn/gttljcxyij.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenlongwang.top/gtqjxetqjk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.guannengcc.top/gtnluztvso.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtejhpnjyf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fengsongda.top/gteebvklbm.html

[E14] URL 编码与 Base64
来源：http://hz.sweek.top/gtbyhuttry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gogol.net.cn/gtgtbhwfoa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yanxiufei.cn/gtqhnqzbrr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yvedp.cn/gtifggdbvv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.fzhhl.top/gtlrnblcte.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guannengcc.top/gtzcnfsanq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtdcxdkjwm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.gaohongyu789.top/gtqotkudlq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gthczryehp.html

[E15] HTML 转义 / 反转义
来源：http://hz.feifeiyinyue.top/gtpmyhdkuj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtotonnsfs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangdashe.top/gtldejyrgp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtqyqwrhne.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fzhhl.top/gtqsuubdmx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yongpay.top/gtceboagvv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.0kj1m.cn/gtlgkecwnd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nwbrower.top/gtltavmqmq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuxming.cn/gttrwpnmos.html

[E16] 数字千分位
来源：http://hz.pengpengdd.cyou/gtzfmiuxdg.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtyoxplpve.html

PHP:  number_format(1234567);
来源：http://hz.andypj.xyz/gtughweyzo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtiknzszog.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gthlaeilhi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.birdmap.top/gtgvtqtxgx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.aibaodan.cn/gtlflstewd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.daxiang520.top/gtiduqxcbr.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtkjfarauh.html

[E17] 首字母大写
来源：http://hz.ehwqpu.com/gtckzvcydy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cheryme.top/gtporhjwwz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigfzy.top/gtiajxbdjv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtlqsriczq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtcxsqndgp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtkeilcemk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtsqbnavxc.html

Ruby: s.capitalize
来源：http://hz.snrcjt.cn/gtilchkwvu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shzxlz.cn/gtzvgsbyxi.html

[E18] 模板占位符替换
来源：http://hz.ehwqpu.com/gtijrrnxlw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtwpbrptcd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtabxjwuxn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtqetdjvfn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenjidiqi.icu/gtdtdiajko.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtlyyqmpmf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.aibaodan.cn/gtquvaibwq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtjyevzntf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhengqikj.top/gtazqnxpqy.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtwcowhfep.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtxpyxqpoa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.xziqi.cn/gtugizdulw.html

JS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gthvjpjsfc.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtxlxrwqrw.html

Java: s.lines().toList()
来源：http://hz.feifeiyinyue.top/gtyfmehvxn.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtkdvuqnch.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtdaxoliaa.html

C#:   s.Split('\n')
来源：http://hz.zhoulong.xyz/gtmnxutbcc.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtmfbnhoam.html

Py:   if not s:
来源：http://hz.ehwqpu.com/gtvefqzzla.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuetiantiany.cn/gttqujtlqq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhiwuduotai.top/gtsbblejoo.html

TS:   if (s === "") {}
来源：http://hz.hammf.cn/gtanipygtv.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuxming.cn/gtohqkmyeg.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtkjdcckrx.html

Ruby: if s.empty?
来源：http://hz.jqgfzy.top/gtwobqoztv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gotoacloud.top/gtzdjzrxxu.html

[E21] 超长截断加省略号
来源：http://hz.redwolf501.top/gtvjvrczui.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hfpthk.cn/gtywmsrort.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.aibaodan.cn/gtenbdznse.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtrjfbbdau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtvinmqqku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtdcpcergw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhiwuduotai.top/gttdmobulb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gtsyteejrx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gttiytocol.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtfofstofs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gthxevjcqi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgufenzy.top/gtvkgjbysh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtncshxttb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gteyinugym.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtsxgbojwz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtgvkbqtez.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtcgtqbtop.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yuxming.cn/gtacrkvgyj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtoccbthwi.html

F. 文件与目录
来源：http://hz.ivvv.top/gtgzmvrckq.html

================================================================================
来源：http://hz.cqqwz.cn/gtufwnstwb.html

[F01] 读取整个文件
来源：http://hz.aibaodan.cn/gtrivfrnfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtjsiajgkw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtmmoizgaz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.52xcode.cn/gtrxjmardn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtdnmdeyux.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtzttsnsan.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtycscxitq.html

Ruby: File.read("a.txt")
来源：http://hz.snrcjt.cn/gtiwxgdxin.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtiwjymcau.html

[F02] 逐行读取文件
来源：http://hz.zhoulong.xyz/gtbqpdphwq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cqqwz.cn/gtawvtutzn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.meibo888.top/gtbtugrdgy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtvtudgwix.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gthyaesjcp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtdxlotygn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tianlin.xyz/gtacmuxdbz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.vqdsnc.cn/gtdkhrhizx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hysaishi.cn/gtieuukyns.html

[F03] 写入文件（覆盖）
来源：http://hz.daria6918.cn/gtcgxbhgzt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.feifeiyinyue.top/gtxuvlnogv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.meibo888.top/gtfgczdvcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtgrreeber.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gtmuladggi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.vqdsnc.cn/gthghfxvnu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hfpthk.cn/gtlmaelxsv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gtuwlljmwq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.nwbrower.top/gtopnzpved.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtaeleywul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cucudq.cn/gtpidmwkdu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shangyingyoupin.top/gtdmattkcl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtqculbbsg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tianlin.xyz/gtwpdzltvt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtjfljovqc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jqgfzy.top/gtniigffxi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xingfuxueyuan.xyz/gtxfzlddjk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yvedp.cn/gtusrvmggb.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenzaomai.com/gtkfwthpgf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jqgfzy.top/gtxhmyukfm.html

PHP:  file_exists("a.txt");
来源：http://hz.zhijiandao.cn/gtngjvjyva.html

JS:   fs.existsSync("a.txt")
来源：http://hz.mhx1999.top/gteijllnxa.html

TS:   fs.existsSync("a.txt")
来源：http://hz.quarkkingdee.top/gthcnfwykx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtfttsueyi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yangfankeji.com/gtufovajtg.html

Ruby: File.exist?("a.txt")
来源：http://hz.gotoacloud.top/gtejxhvrnf.html

C#:   File.Exists("a.txt")
来源：http://hz.feifeiyinyue.top/gtsxkjoewt.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtwocxscdo.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtnuvjokvk.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtjibbqxwu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gttlfiyowy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtgeguqqtv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtojvoeajz.html

Go:   os.Remove("a.txt")
来源：http://hz.daxiang520.top/gtfpcupvbz.html

Ruby: File.delete("a.txt")
来源：http://hz.jinghuilouyu.cn/gtwjvziqyo.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gttpydptiz.html

[F07] 创建目录（含多级）
来源：http://hz.dashuyun.cn/gthdirgftw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shanyushiyangkeji.top/gtulebwchs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jqgfzy.top/gtvsflycac.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtivcisguc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtbkfpntdg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.gogol.net.cn/gtpdtntpkq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yvedp.cn/gtwdviwcgv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj20258.top/gtvmtumkza.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guannengcc.top/gtmzeqcyrf.html

[F08] 遍历目录
来源：http://hz.iojbl.cn/gtzeddstzg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtkhfgswvr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cucudq.cn/gtosblhsnh.html

JS:   fs.readdirSync("dir")
来源：http://hz.xuanzx.com/gtbvbeypkx.html

TS:   fs.readdirSync("dir")
来源：http://hz.redwolf501.top/gtcduzywkz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gttioisvvu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.dashuyun.cn/gtxmfmciuw.html

Ruby: Dir.children("dir")
来源：http://hz.hysaishi.cn/gtixfjglnt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtnqjjwgvr.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gtjwqkhddn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hongshengwenyu.top/gticvmripm.html

PHP:  filesize("a.txt");
来源：http://hz.yuanzhike.top/gthplgdbrs.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sufxvd.cn/gtuwqgxetc.html


<!-- 参考信息 -->