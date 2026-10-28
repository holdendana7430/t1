代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtyahmfplp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hfpthk.cn/gtausqpxmd.html

Go:   // 手写循环
来源：http://hz.jqgfzy.top/gtotddlyok.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtypxoahaq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuanzhike.top/gtytpccsej.html

[D24] 字典 / Map 基本操作
来源：http://hz.shanyushiyangtech.top/gtulphqqin.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yongpay.top/gtrhezrrgx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtynytvjiw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtxxnukfzq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.wangshuangyany.cn/gtrvffahxu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.svipenyu.cn/gtolopwcun.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cheryme.top/gtlurhmxjr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtymedjhwt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtlraupklu.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtfwxrrety.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtvrqdzjjw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtpdlhibve.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtglpokkep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtblwbwdoo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dianchejie.cn/gtdgaferiv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtrpmjavnw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtreryitra.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daxiang520.top/gtskxhpyrl.html

[D26] 数组转字符串
来源：http://hz.yanxiufei.cn/gtjhuyedpg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtmdbdjatg.html

PHP:  implode(", ", $arr);
来源：http://hz.yuanzhike.top/gtsbvqeaok.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtqahmjirf.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtyqpmodqc.html

Java: String.join(", ", list)
来源：http://hz.bjfxy.top/gtlczfjbei.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cucudq.cn/gtmqwagfss.html

Ruby: arr.join(", ")
来源：http://hz.yvedp.cn/gtgdwwvwsw.html

C#:   string.Join(", ", list)
来源：http://hz.sysykeji.top/gtnwxwxldy.html

================================================================================
来源：http://hz.gogol.net.cn/gtmmajkufu.html

E. 字符串处理
来源：http://hz.jinghuilouyu.cn/gtdlljxwjo.html

================================================================================
来源：http://hz.smart0.xyz/gtbrlqlhmw.html

[E01] 拼接字符串
来源：http://hz.fzhhl.top/gtmxshxlsl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cheryme.top/gtgukyrxut.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gthbpoctyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtvnlfhzcf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.c1oappe.top/gtobtkhpoa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.quarkkingdee.top/gthpgwarri.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yvedp.cn/gtstrnrhia.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangdashe.top/gtieqcyttv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shuidangran.top/gttbzrxcqc.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtlyrpxghx.html

Py:   "ab" * 3
来源：http://hz.jqgufenzy.top/gtnjsiuhfp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.wangdashe.top/gtcjgjhcqw.html

JS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtmxpuaitg.html

TS:   "ab".repeat(3)
来源：http://hz.yuxming.cn/gtxqpdefjz.html

Java: "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtoramppsy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtmxkhoffg.html

Ruby: "ab" * 3
来源：http://hz.jinqigufen.top/gtbgdqszxk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gthjqwmjyt.html

[E03] 截取子串
来源：http://hz.hnqzz.top/gtphpxeuxk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtknintskl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gtdefocodh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtnlptltwb.html

TS:   s.slice(1, 4)
来源：http://hz.guowangkeji.top/gtpkweglvx.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtbnpmfinb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gthgmhdpyi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jiagoushi.top/gtltnjdnln.html

C#:   s.Substring(1, 3)
来源：http://hz.kuanghao11.cn/gtjzngfbkf.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gthvpkdmba.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtbreaifmh.html

PHP:  strpos($s, "x");
来源：http://hz.yuxming.cn/gthjblibow.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxinkj.top/gtzsocxxyd.html

TS:   s.indexOf("x")
来源：http://hz.snrcjt.cn/gtvgddnfef.html

Java: s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtnwlspcye.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtadcxaazq.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtjzorslbk.html

C#:   s.IndexOf("x")
来源：http://hz.jqgufenzy.top/gtitdgqins.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtbveohvxv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtcxtyetux.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xuetiantiany.cn/gttaraxziy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gtaqoisdge.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jqgfzy.top/gtmajpelas.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtzjfspocv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtmlzxubsl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.wangshuangyany.cn/gtdooablmf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hywenlv.cn/gtswxudwdm.html

[E06] 替换子串
来源：http://hz.dianchejie.cn/gthdkhomvl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtaqhmqetr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tanke756.top/gtmxpbrads.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtvohdzebm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hywenlv.cn/gtmgzadagk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtrbwqspbi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtxxdphrfp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yonumen.top/gtubkxcnxt.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigfzy.top/gtiflnourt.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtumjyotfd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gtfzcldagv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.snrcjt.cn/gtqmgonals.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.snrcjt.cn/gtevrxhrgv.html

TS:   s.split(",")
来源：http://hz.fzhhl.top/gtseohidon.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtwinhdzhp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.havefunace.top/gthabiokcy.html

Ruby: s.split(",");  s.split
来源：http://hz.nanxinkj.top/gtnkqdlztx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.daria6918.cn/gtzitknkic.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtmpgmdsdq.html

Py:   ",".join(items)
来源：http://hz.zdqjudy.top/gtrhvxvxln.html

PHP:  implode(",", $items);
来源：http://hz.pengpengdd.cyou/gtkkzdtqmx.html

JS:   items.join(",")
来源：http://hz.fzhhl.top/gtrxycqghg.html

TS:   items.join(",")
来源：http://hz.daxiang520.top/gtruhmnqmo.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gtvbzdmirh.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgufenzy.top/gtmosraxfy.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gttbmyxwig.html

C#:   string.Join(",", items)
来源：http://hz.zhengqikj.top/gtnbxgomsn.html

[E09] 去除所有空白字符
来源：http://hz.zdqjudy.top/gtbnwrfohd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigufen.top/gtdkydiqyi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gotoacloud.top/gtikxgqpds.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gthcasjvzw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zycfv.cn/gtxdmqnwlx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtzfhtalfo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258888.top/gtaasbbhqw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gthouxidlv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shzxlz.cn/gtvuayvqyo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gturgpeahb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydjk.org.cn/gthcraxpah.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.quarkkingdee.top/gtxvqwtota.html

JS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtrixknejt.html

TS:   "7".padStart(3, "0")
来源：http://hz.gotoacloud.top/gtmthlvfqh.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtjenwskpb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gttuzejcvz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtvtsyoyov.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.aibaodan.cn/gtcmgkbapr.html

[E11] 反转字符串
来源：http://hz.xuetiantiany.cn/gtzxzkaqiy.html

Py:   s[::-1]
来源：http://hz.jiagoushi.top/gtoispfhef.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gtfrueqjol.html

JS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gtiufcqwuw.html

TS:   [...s].reverse().join("")
来源：http://hz.52xcode.cn/gttduictve.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.smart0.xyz/gtcyjrkzgq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gzhubu.top/gtxlnahdrz.html

Ruby: s.reverse
来源：http://hz.fengsongda.top/gtldnyaorg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtxmztcmlf.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtnbnzufak.html

Py:   s.count("a")
来源：http://hz.gzhubu.top/gtznfcwjhy.html

PHP:  substr_count($s, "a");
来源：http://hz.cdnleiting.top/gtnvndhmgi.html

JS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gttgcsesaq.html

TS:   s.split("a").length - 1
来源：http://hz.pengpengdd.cyou/gtdfnpwhqe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gthdgubrra.html

Go:   strings.Count(s, "a")
来源：http://hz.jiagoushi.top/gtwoaxdasc.html

Ruby: s.count("a")
来源：http://hz.9152youxi.cn/gtylfzdasj.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtmetxtuic.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtzmkagiyz.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtzbzmdumx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sufxvd.cn/gtnhwylgdq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gotoacloud.top/gtytnulxhn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtrpzpuhdu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtkiuxbusv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtfbsmfjra.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtimpiisvq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jlsjyb.cn/gtopaajzho.html

[E14] URL 编码与 Base64
来源：http://hz.wangdashe.top/gtiqkvxrup.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gthwhweylc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fzhhl.top/gtygikksve.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.andypj.xyz/gtjxypljhx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hfpthk.cn/gtbibarxgf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnxiangtu.top/gtcjdmbban.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangdashe.top/gtdylmqsnk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.9152youxi.cn/gtdnvcdgks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gtrrubghtd.html

[E15] HTML 转义 / 反转义
来源：http://hz.52xcode.cn/gteavjepms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.guannengcc.top/gteaxypmub.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj202588.top/gtphpepait.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgufenzy.top/gtdwlsbplq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtmwwspxdm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhoulong.xyz/gtwtlkhnqx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.redwolf501.top/gtrihsskvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gthqwxyeef.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhengqikj.top/gtcopwmqdp.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtejflgbau.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtnyjdbzkm.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtllxmuael.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhixingplan.top/gtkexntami.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtaimwxtlu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gtibmhoawd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.nwbrower.top/gtluolxogb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cucudq.cn/gtdxlmijtl.html

C#:   1234567.ToString("N0")
来源：http://hz.snrcjt.cn/gtarredprg.html

[E17] 首字母大写
来源：http://hz.snrcjt.cn/gtfzcygtfp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtzdadvslv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtmjyblqoe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtqwiqdeuw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtmwchmsiu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.smart0.xyz/gtuoiokruj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.52xcode.cn/gtkkifmfno.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtpxtmkddo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtikffrrgw.html

[E18] 模板占位符替换
来源：http://hz.pycfn.com/gtgewqxdjp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gaohongyu789.top/gtnaeppllf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtabvzases.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gttmllyygs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtvysbafhr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gtvajczwgg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj20258.top/gtfozwwazo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yongpay.top/gtttlykmjf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gtdfdsfeut.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtqsdzuijn.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtpbpnanea.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gtxswnfpsb.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtjkievgqw.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gtxeetweta.html

Java: s.lines().toList()
来源：http://hz.redwolf501.top/gthextzglt.html

Go:   strings.Split(s, "\n")
来源：http://hz.c1oappe.top/gtdqwhoitf.html

Ruby: s.lines
来源：http://hz.jinqigufen.top/gtqmpjzsqn.html

C#:   s.Split('\n')
来源：http://hz.xinyue.icu/gtzmpryvlf.html

[E20] 判断字符串是否为空
来源：http://hz.aizwys.cn/gtdeezklwe.html

Py:   if not s:
来源：http://hz.pycfn.com/gtsqtdylbz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xuanzx.com/gtyvkshwgl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtzkdufwhf.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtqnsfhmgz.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtdyxhuyry.html

Go:   if s == "" {}
来源：http://hz.0kj1m.cn/gtlhiwxizk.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtkxlwaxnv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgfzy.top/gtymvrjilf.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtyqgsgqzm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtnqhxaiwg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jyoumei.cn/gtvuopcsyn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zdqjudy.top/gtaazadaun.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.c1oappe.top/gtmpnhccuf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hywenlv.cn/gtjgrjxbqw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jyoumei.cn/gtvefpivjx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtwkbgqffo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnxiangtu.top/gtizunqhlb.html

[E22] 字节长度与字符长度
来源：http://hz.fengsongda.top/gtieepjxbx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gtcxffnlxc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.aizwys.cn/gtgzbiyssg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.mhx1999.top/gterihwfez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtvkdjylrh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtgnretyok.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgufenzy.top/gtkplmuynx.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtdjwvajdw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.tianlin.xyz/gtzbgygefz.html

================================================================================
来源：http://hz.xziqi.cn/gttgevwjub.html

F. 文件与目录
来源：http://hz.birdmap.top/gtwsnrmexv.html

================================================================================
来源：http://hz.havefunace.top/gtdfnbtyae.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtdteuqqye.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gtwrbihgnr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtjryeshvm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gzhubu.top/gtuwwybdbo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj202588.top/gtahjdxiur.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtquvqtxeh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.aizwys.cn/gttvpgnkmu.html

Ruby: File.read("a.txt")
来源：http://hz.chenlongwang.top/gtnzviyguz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gzhubu.top/gtxyntqacg.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtylxasmct.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtfmcfqcdt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuetiantiany.cn/gtbqbmscqe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangtech.top/gtwkuvjscj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yonumen.top/gtpmxrxrae.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtnttisgof.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhiwuduotai.top/gtpqxxdevu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cheryme.top/gtovyeuxjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yongpay.top/gtakcpqvsg.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtgovmfchz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.bjfxy.top/gtyprdhnfg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtusflfcxg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtxsibizrw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yuanzhike.top/gtsdsukbyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gtbjnamxyd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gttblqawrh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.meibo888.top/gtqedbebjn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtovqpfoch.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtvxmxmtui.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtxhxnjkuf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.guannengcc.top/gtvcysvsac.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtstejhgms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gterbkxgxf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.snrcjt.cn/gtdipiezfv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtqpaxjmuh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gttvgrulda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtqdrcwaol.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangtech.top/gtfefagtvh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtepqtejsi.html

PHP:  file_exists("a.txt");
来源：http://hz.yangfankeji.com/gtpntnippe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jianghu66.top/gtoamymapt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtilcfvwpz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtwtkbjwaa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtemlekqds.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gtbbyfeqdp.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gttcbumufs.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtnjufoxkc.html

Py:   os.remove("a.txt")
来源：http://hz.jinghuilouyu.cn/gtxpltvxgq.html

PHP:  unlink("a.txt");
来源：http://hz.chenjidiqi.icu/gtvnentfqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtekzdncuu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jiagoushi.top/gtzcjucfmn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gthspdnuqk.html

Go:   os.Remove("a.txt")
来源：http://hz.zdqjudy.top/gthapsbwzn.html

Ruby: File.delete("a.txt")
来源：http://hz.havefunace.top/gtigxfwmxp.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtecdsobhx.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigufen.top/gtzvcvywlj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.svipenyu.cn/gtsyocdmhs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.feifeiyinyue.top/gtahppvjyl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.9152youxi.cn/gtofvdfbyo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtzopnyywg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.52xcode.cn/gtavhoqxwh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.aizwys.cn/gtrgvusnif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.fzhhl.top/gtdxebojiq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xziqi.cn/gtvzvondmt.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gtxckdzpkr.html


<!-- 参考信息 -->