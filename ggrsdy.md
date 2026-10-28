代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.smart0.xyz/gtpogbiymv.html

[D24] 字典 / Map 基本操作
来源：http://hz.shuidangran.top/gtnzofwmee.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtarsqttde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtfdqyfbyi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gteqweikgm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtpqychpvh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtikedvjhj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtqmjjmixw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtsttyvnuu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gtazkztmqk.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtpilhiytk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtqkrnqnos.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtvvgfyaoa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtgxyhifez.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daria6918.cn/gtjafzpgwd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cheryme.top/gttvtwmqoj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtkmatcohl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cheryme.top/gtdmkfixhx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj202588.top/gtqgttngaj.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtncukgpuw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtlstvotvo.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtighhqqke.html

JS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtsbuqznth.html

TS:   arr.join(", ")
来源：http://hz.sweek.top/gtzlxmyrwu.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtngpkrpwn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtxhfabaou.html

Ruby: arr.join(", ")
来源：http://hz.ydjk.org.cn/gtwjdgjhxh.html

C#:   string.Join(", ", list)
来源：http://hz.yanxiufei.cn/gtxzdnkztr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtffvsrbar.html

E. 字符串处理
来源：http://hz.cqqwz.cn/gtvpcukjbv.html

================================================================================
来源：http://hz.havefunace.top/gtyyzfeqgl.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtskfwyhdi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuanzx.com/gtdolbdvmn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtxkmrtsnx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtycunxfvv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtdoiiqsfr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtzyxbkcaq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgfzy.top/gtawbaiqzp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shangyingyoupin.top/gtkavewwol.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtxsamyaks.html

[E02] 重复字符串
来源：http://hz.tianlin.xyz/gtgyfkbfsu.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtacrepbpg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtystfknxm.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtxofuhmxj.html

TS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtrynobvyd.html

Java: "ab".repeat(3)
来源：http://hz.andypj.xyz/gthsakchtx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yongpay.top/gtkkzwslqb.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtjrplknsm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yvedp.cn/gtrvidiaci.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtmqvhkmid.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigfzy.top/gtvtpjnwan.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tian-w.cn/gtcmzonloa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtvhqovqgv.html

TS:   s.slice(1, 4)
来源：http://hz.wangdashe.top/gtfirvncaz.html

Java: s.substring(1, 4)
来源：http://hz.nanxinkj.top/gthstpznnd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.gogol.net.cn/gtwlmiltzw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtjcgocrmt.html

C#:   s.Substring(1, 3)
来源：http://hz.yueranfly.top/gtvggrnyuo.html

[E04] 查找子串位置
来源：http://hz.iojbl.cn/gtaxqbeaed.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtyyyazufe.html

PHP:  strpos($s, "x");
来源：http://hz.snrcjt.cn/gtmujkwvax.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.quarkkingdee.top/gtiwdsslfg.html

TS:   s.indexOf("x")
来源：http://hz.yangfankeji.com/gtlkwamitf.html

Java: s.indexOf("x")
来源：http://hz.bjfxy.top/gtpyjuwyur.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtzfwrjgmf.html

Ruby: s.index("x")
来源：http://hz.havefunace.top/gtxfuubutt.html

C#:   s.IndexOf("x")
来源：http://hz.shuidangran.top/gtizxlnkqj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.52xcode.cn/gtnwxpikun.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.iojbl.cn/gtvhvidvcl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sysykeji.top/gtvitddudx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtadotrrra.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.bjfxy.top/gttsxlegnr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtchkjzvbv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtnzpkqiud.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuxming.cn/gtmrmzuanx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuanzhike.top/gtgfgziapi.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtkbsdeenw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtglmgxrib.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtccdhgfig.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gthxxlleey.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gttdabusbw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtlshotjzp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuanzx.com/gtylxdddgu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtdkcsadeh.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtpjtfpkhe.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gthflrzofo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gotoacloud.top/gtjqupvmud.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.chenjidiqi.icu/gtyhmlbjrt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cdnleiting.top/gtzjgyvzue.html

TS:   s.split(",")
来源：http://hz.yuxming.cn/gtjvnyxdpj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.andypj.xyz/gtbormpjki.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.smart0.xyz/gtrsuawnsc.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gthfwaagqs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtogicyqkf.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtugtxjjry.html

Py:   ",".join(items)
来源：http://hz.cheryme.top/gtuwonnuhp.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtlagcipjf.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtcwmqizqm.html

TS:   items.join(",")
来源：http://hz.ydzc1.top/gtsjzyvdkz.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtoljutxyz.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gteovlktie.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtydkzpskq.html

C#:   string.Join(",", items)
来源：http://hz.andypj.xyz/gtwovikfqd.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gtnanjopnp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtlpmlgqxz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gtpdxnystn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gtnabippzi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtukwlxzts.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sweek.top/gtghgmvmfw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtnkhutxnn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jianghu66.top/gtedllojoi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenzaomai.com/gtcdjpovxh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gtpwegpcfm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtzhrvvupz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daxiang520.top/gtjzodutgu.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtrabixnxv.html

TS:   "7".padStart(3, "0")
来源：http://hz.ppjwa.cn/gtcqeurjvt.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gtbhlwxcec.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hnqzz.top/gtgrhkdyzd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtshxnwzze.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gttguoghpn.html

[E11] 反转字符串
来源：http://hz.jinyuanbaomall.cn/gtikryvpbd.html

Py:   s[::-1]
来源：http://hz.dashuyun.cn/gtsnohckkl.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtrkvuuhhh.html

JS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtdkxwnrkn.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gttpugosxr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gogol.net.cn/gtslucyrrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jlsjyb.cn/gtuiwoyvye.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtxmzfjdzo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cdnleiting.top/gtdyynjkrs.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtdfyhfxrl.html

Py:   s.count("a")
来源：http://hz.ydzc1.top/gtzuslodye.html

PHP:  substr_count($s, "a");
来源：http://hz.snrcjt.cn/gtujedduqh.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtfsbnzirf.html

TS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtahngqiak.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtabxbxodj.html

Go:   strings.Count(s, "a")
来源：http://hz.smart0.xyz/gtcwouvlpi.html

Ruby: s.count("a")
来源：http://hz.jianghu66.top/gtztcddsbz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.bjfxy.top/gtwhaolsac.html

[E13] 逐字符遍历
来源：http://hz.xuetiantiany.cn/gtglrijifl.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtzueuadye.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.iojbl.cn/gtqjpncvqt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtsbvihuri.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtjzezosez.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gtzvkdybij.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hywenlv.cn/gtmznrvgmr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.andypj.xyz/gtsphkgnbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtxozskcni.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtbwrrrjuw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtygduywcn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhoulong.xyz/gtesfmisul.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.pycfn.com/gtzfjxujrw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ppjwa.cn/gtseiaomhl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtnoslsdgn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shangyingyoupin.top/gtlxaommxy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtrpproarg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sysykeji.top/gtswxspuxs.html

[E15] HTML 转义 / 反转义
来源：http://hz.xuetiantiany.cn/gtbncnknxw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.vqdsnc.cn/gtmemewqzy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cucudq.cn/gthqgxghmi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gtvfxvkcpl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gtxwsogutw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.meibo888.top/gttuvpxoin.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.fzhhl.top/gtxyfmwyiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.haohaochexian.top/gtuujteimv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinyuanbaomall.cn/gtvvtthhzs.html

[E16] 数字千分位
来源：http://hz.jyoumei.cn/gtxbjlwbgp.html

Py:   f"{1234567:,}"
来源：http://hz.gogol.net.cn/gtiimcxtra.html

PHP:  number_format(1234567);
来源：http://hz.yangfankeji.com/gtblnzanap.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtynnhrawt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtbyozbyzs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gaohongyu789.top/gtfugcpxta.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gthipanzlz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtbtjsvizr.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gthbcvccau.html

[E17] 首字母大写
来源：http://hz.zhixingplan.top/gtyivggjkb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtboxifdlj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zdqjudy.top/gtnmkemkia.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sufxvd.cn/gtcwzknfal.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtxsajdtmf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtautqfope.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hammf.cn/gtakfskfnh.html

Ruby: s.capitalize
来源：http://hz.yanxiufei.cn/gtbqfzspvc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hywenlv.cn/gtvovfppqe.html

[E18] 模板占位符替换
来源：http://hz.aibaodan.cn/gtdyfgsbdo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.wangshuangyany.cn/gtdzeuisqx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gttkunoxus.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtsgjfpgis.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtfizkgyel.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gtjewwsqdr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.redwolf501.top/gttqxkyovg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yangfankeji.com/gtibqoprpc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtqedzwvzw.html

[E19] 多行文本按行拆分
来源：http://hz.ydzc1.top/gtuwqeztrs.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtxjigvwcw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.quarkkingdee.top/gttomwjsju.html

JS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtnxvdhose.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gthaqewefe.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtkhzcvawh.html

Go:   strings.Split(s, "\n")
来源：http://hz.zdqjudy.top/gtwfzfetup.html

Ruby: s.lines
来源：http://hz.ehwqpu.com/gtckxpwbpn.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtobdabxtn.html

[E20] 判断字符串是否为空
来源：http://hz.jqgfzy.top/gtbwuykojc.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtzhcephlc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtxezhnrzp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sxryk.cn/gtgwqldoom.html

TS:   if (s === "") {}
来源：http://hz.ybcxt.top/gtiwrdoebv.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydzc1.top/gtaujgaloc.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gtrzoqbyda.html

Ruby: if s.empty?
来源：http://hz.xinyue.icu/gtrtmnkfrd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fengsongda.top/gtkgckcdds.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtutijercx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tianlin.xyz/gtyujhyjbz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.cucudq.cn/gtqozevjmp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtnzipyghb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtlzpwivpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtagmilhqi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtbpdcjiak.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtjeckyrfp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nanxinkj.top/gtjigqujgv.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gttxxbyvlw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhijiandao.cn/gtwkseczdt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtowefogyq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtpoygtsjy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtxknsoipp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.bjfxy.top/gtnirhymkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gtlmtcszep.html

Ruby: s.bytesize;  s.length
来源：http://hz.sysykeji.top/gtmeykabpv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cdnleiting.top/gtghcelzfc.html

================================================================================
来源：http://hz.yj202588.top/gtdwfwubpr.html

F. 文件与目录
来源：http://hz.zhongyouzk.top/gtecaxnbnx.html

================================================================================
来源：http://hz.havefunace.top/gtdxggpmaz.html

[F01] 读取整个文件
来源：http://hz.bjfxy.top/gttscenxtq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.feifeiyinyue.top/gtjrkjovxv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.kuanghao11.cn/gtcecoyrrm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jianghu66.top/gtoiauwfks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtzeuxpjzj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.mhx1999.top/gtyjutpdok.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.meibo888.top/gtldqigdpd.html

Ruby: File.read("a.txt")
来源：http://hz.wangdashe.top/gtvfjsysda.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtrwmjskhc.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtswqrsfsl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.316326.xyz/gtfgrdbzkb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ivvv.top/gtaqtfjsks.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtkosvtbtb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtpzlgavrk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtlissisvm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.cqqwz.cn/gtoqagbsyu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuetiantiany.cn/gtvkdgrint.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dianchejie.cn/gtwccbvrek.html

[F03] 写入文件（覆盖）
来源：http://hz.fengsongda.top/gttxiqjhfl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.kuanghao11.cn/gtopydrfli.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ydjk.org.cn/gtgpiwjhym.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtxcyfedaq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtxfljhbsz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zycfv.cn/gtidmylpya.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.birdmap.top/gtuszptaht.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.mhx1999.top/gtqwoktvpy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtljbfbjwt.html

[F04] 追加写入文件
来源：http://hz.hongshengwenyu.top/gtkxecfzjd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dianchejie.cn/gtnmpxrwjz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.c1oappe.top/gtlodrocrg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtqtsbchcj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtrklqoycf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj202588.top/gtrynahcpy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aibaodan.cn/gtynrwrjkn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj202588.top/gtnalklmag.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.birdmap.top/gtbxstvulr.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gtpysdtgjo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtgzaatdtb.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtgqlwekwv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtmbgbdisl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtacyfanty.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtgqiaehlh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.haohaochexian.top/gtyahulrps.html

Ruby: File.exist?("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtaoruyuen.html

C#:   File.Exists("a.txt")
来源：http://hz.nanxinkj.top/gtmmmgbgxk.html

[F06] 删除文件
来源：http://hz.hywenlv.cn/gttfzbmklf.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtpsollhok.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtxeoknobp.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtsegbrjkl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtyoroaxkq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gthjnkolqf.html

Go:   os.Remove("a.txt")
来源：http://hz.wangshuangyany.cn/gtnhihsjtc.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtsazggxpr.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtjmvlicch.html

[F07] 创建目录（含多级）
来源：http://hz.tianlin.xyz/gtitqucwoy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ydzc1.top/gtzeokwauw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.quarkkingdee.top/gtuatsfdsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtfsvvcjcy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtvudrnwvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.fzhhl.top/gtaiffizyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigufen.top/gtoapcfmbw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.tanke756.top/gtploelzzu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenjidiqi.icu/gtfatotzur.html

[F08] 遍历目录
来源：http://hz.meibo888.top/gtnbwpcwns.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zdqjudy.top/gtcdaavfxf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.ydzc1.top/gtshulrvzh.html

JS:   fs.readdirSync("dir")
来源：http://hz.xylfe.cn/gttadeafcc.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gthfggmkyn.html


<!-- 参考信息 -->