代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtntwicrwg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtpdczdnqx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cqqwz.cn/gtuqlyekfl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtabwzkiao.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhijiandao.cn/gtbwbsktoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtkzavuyxr.html

[D25] Set 集合去重与交并差
来源：http://hz.zhiwuduotai.top/gtaqugywhc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yanxiufei.cn/gtopkbknuy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtpefbbzkt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hywenlv.cn/gtexejthol.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gttuhtxcll.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sweek.top/gtitjjgjjo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhaomingkeji.xyz/gtqfoxxxht.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtovfodrnp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yueranfly.top/gtbzedkfwu.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtlixjcpet.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gteapzuqjf.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtbnysaycd.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gthpceszox.html

TS:   arr.join(", ")
来源：http://hz.daxiang520.top/gtmnrhxoex.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtrwehvvmb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gthylcwbys.html

Ruby: arr.join(", ")
来源：http://hz.316326.xyz/gtmducnroj.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtwukacbcn.html

================================================================================
来源：http://hz.yvedp.cn/gtlemozzdm.html

E. 字符串处理
来源：http://hz.xuanzx.com/gturnstpjo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtikmubsti.html

[E01] 拼接字符串
来源：http://hz.xziqi.cn/gtvjnhyepu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtzbspuwof.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.daxiang520.top/gtaxismyjp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gtiykopfei.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtwljsyoyq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xuanzx.com/gtoteqyjjm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigfzy.top/gtmaeyifjj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.vqdsnc.cn/gtcfypytze.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jqgfzy.top/gtmfptvdqu.html

[E02] 重复字符串
来源：http://hz.andypj.xyz/gtcjnmvvih.html

Py:   "ab" * 3
来源：http://hz.yanxiufei.cn/gtjrlmcjwi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtcsepsrkw.html

JS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gttqulfupj.html

TS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtfmssmeoq.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gtnpidnwcb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gtqmnjdtzf.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtxzfjpkai.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtuwfdkphe.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtovtjezdm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtqszgvgww.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ehwqpu.com/gtivnlwuvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtxvadagee.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtmwadevvt.html

Java: s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtteljwbfa.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinghuilouyu.cn/gtjkcuxwkp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenzaomai.com/gtopouvlcb.html

C#:   s.Substring(1, 3)
来源：http://hz.sweek.top/gtvbbqvpgi.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtczxqzerl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtyphbuyie.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtmsnuyjij.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtgbdcnhqg.html

TS:   s.indexOf("x")
来源：http://hz.aizwys.cn/gtgskuigoj.html

Java: s.indexOf("x")
来源：http://hz.shuidangran.top/gtbvhqretf.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtfstysshk.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtgwkskxjq.html

C#:   s.IndexOf("x")
来源：http://hz.zhongyouzk.top/gtdfsheqmq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenjidiqi.icu/gttjbrqola.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zdqjudy.top/gtmrdeggao.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.svipenyu.cn/gtbiwvguvg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtusarehrw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.feifeiyinyue.top/gtmskytwfe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gtcvyupdwu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtimsmxqai.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.quarkkingdee.top/gtbwhuhjqn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xuetiantiany.cn/gtvblkdofv.html

[E06] 替换子串
来源：http://hz.yongpay.top/gtnavuzrjh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.nanxinkj.top/gtwnbgqhxe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gtcicmzpiz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtxsqldona.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtkmbdkqlc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtkqbzscxw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ydzc1.top/gtgktodolx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.haohaochexian.top/gtedwvnmlt.html

C#:   s.Replace("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtlzhefwko.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtlnfqeutu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtxygkmwgb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sysykeji.top/gtohairhyk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.52xcode.cn/gtzkodrohc.html

TS:   s.split(",")
来源：http://hz.yanxiufei.cn/gtausapgfx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtfspuqkpa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gogol.net.cn/gtcvaxsqcx.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtyexsuryo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtbrvomfmp.html

[E08] 数组按分隔符合并
来源：http://hz.pengpengdd.cyou/gtvuurcgjx.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtyuyytmsr.html

PHP:  implode(",", $items);
来源：http://hz.yongpay.top/gtweeyngyc.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gteddalwqv.html

TS:   items.join(",")
来源：http://hz.hammf.cn/gtqhcbbntj.html

Java: String.join(",", items)
来源：http://hz.cdnleiting.top/gthfbjhbhk.html

Go:   strings.Join(items, ",")
来源：http://hz.ivvv.top/gtnikvymwy.html

Ruby: items.join(",")
来源：http://hz.yonumen.top/gthllpyese.html

C#:   string.Join(",", items)
来源：http://hz.svipenyu.cn/gtaajyffkg.html

[E09] 去除所有空白字符
来源：http://hz.jlsjyb.cn/gtnakojlwb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jyoumei.cn/gtqkxkqtlj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtltflorpq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.c1oappe.top/gtqtlpejzl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtmgreiojp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinghuilouyu.cn/gtnwkybrov.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuanzhike.top/gtghrwreai.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gtdesvdujq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xylfe.cn/gtekqmylig.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtachcfyoh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gthfgubeis.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shuidangran.top/gtsxerbbok.html

JS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gttqggtzfw.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtajiyohhp.html

Java: String.format("%03d", 7)
来源：http://hz.yueranfly.top/gtmscjepoj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtqkqkczfu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gttudsapuz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtqefgqvks.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtivyjzklw.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtasjjioxv.html

PHP:  strrev($s);
来源：http://hz.tian-w.cn/gtjrkanpqe.html

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtkjqtolbl.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gteoqwoxtl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gtyhthxndv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tanke756.top/gtuqcybedy.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtclbeigvf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtjyyisbcn.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtmjwslart.html

Py:   s.count("a")
来源：http://hz.hnxiangtu.top/gtommybitb.html

PHP:  substr_count($s, "a");
来源：http://hz.ydzc1.top/gtxtbjyzhh.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtdkmvthkb.html

TS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtguiqnemm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gaohongyu789.top/gtfrkbbiji.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtwxxqqovl.html

Ruby: s.count("a")
来源：http://hz.sysykeji.top/gtpzrvmnus.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jiagoushi.top/gtghprzqch.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtptmavicd.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtodsqvewa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtrqgpoaai.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gttelzguqg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtfeuuocgh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.vqdsnc.cn/gtmdmyrcio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtzwbdevlk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sxryk.cn/gtpnuljanr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtffylqzpa.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtrkageujw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxuanxn.top/gtyudelxdm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangshuangyany.cn/gtwbtqwmoq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhiwuduotai.top/gtjbtllkyj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtitmxwmqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guannengcc.top/gtyteksgev.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gotoacloud.top/gtzxxxbnsi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tanke756.top/gtcivzknkv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinqigfzy.top/gtlrigaivw.html

[E15] HTML 转义 / 反转义
来源：http://hz.tanke756.top/gtohuadfzs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aizwys.cn/gtvvkhyjpo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.feifeiyinyue.top/gtmliubhqa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hammf.cn/gtxzmhwnij.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtdiqmgeqb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jiagoushi.top/gtemhqubvg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jlsjyb.cn/gtydltokbr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.andypj.xyz/gtczbdlgbg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtayewkcmf.html

[E16] 数字千分位
来源：http://hz.iojbl.cn/gtokmytxih.html

Py:   f"{1234567:,}"
来源：http://hz.hywenlv.cn/gtszzcahtu.html

PHP:  number_format(1234567);
来源：http://hz.svipenyu.cn/gtcdhimsel.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtlcxnvsol.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtrcoxcrjt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tanke756.top/gtxolvozdt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xuanzx.com/gtnhtxfvrn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.bjfxy.top/gtadgjrour.html

C#:   1234567.ToString("N0")
来源：http://hz.dianchejie.cn/gtjizlluyh.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtpxqawlcn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.havefunace.top/gtnjzoymyh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtthymsjfu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenlongwang.top/gtkxqswjkf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fengsongda.top/gtxbljaaro.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtvbjuzvyj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xuetiantiany.cn/gtezpkxkyv.html

Ruby: s.capitalize
来源：http://hz.nanxuanxn.top/gtahngokci.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtpptmeqtj.html

[E18] 模板占位符替换
来源：http://hz.yueranfly.top/gtahfuvbdl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xinyue.icu/gtmtfmkrwv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.quarkkingdee.top/gtqqrygwmi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtrwgarbzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtwkbvvems.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gttjucwxjk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.mhx1999.top/gtyxomcjxr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gtvqqvcdmx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dashuyun.cn/gtrjyobxte.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtctztimlj.html

Py:   s.splitlines()
来源：http://hz.shuidangran.top/gtzhzlqlru.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtotltldiu.html

JS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtwujemfdv.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtaxctxnkw.html

Java: s.lines().toList()
来源：http://hz.yueranfly.top/gtjlippnvv.html

Go:   strings.Split(s, "\n")
来源：http://hz.hammf.cn/gtujoutcnw.html

Ruby: s.lines
来源：http://hz.yj20258.top/gtsamzmcfd.html

C#:   s.Split('\n')
来源：http://hz.aizwys.cn/gtaiwtqfzs.html

[E20] 判断字符串是否为空
来源：http://hz.zhongyouzk.top/gtncjlfkvd.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtatrlcqtq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hnqzz.top/gtuxnyxofk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtmhbphyus.html

TS:   if (s === "") {}
来源：http://hz.yuxming.cn/gtvgubtrtz.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtsddtzotw.html

Go:   if s == "" {}
来源：http://hz.52xcode.cn/gthlzaewie.html

Ruby: if s.empty?
来源：http://hz.vqdsnc.cn/gtqerlpllo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jlsjyb.cn/gttjtqrkzp.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtidahqwxz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xuanzx.com/gtbkuwcapa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtzpuhpojg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtpauoqcrf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtuvxqhhqb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sxryk.cn/gtcqwizfer.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gzhubu.top/gtjnvjvdkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gtexbvotun.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtcxskbglz.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gthpuncrmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aibaodan.cn/gtgaowhpfx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.vqdsnc.cn/gtujnhsxut.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gtzqtnaxdj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtxaqassjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhijiandao.cn/gtlczgkmlc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yangfankeji.com/gtqumfwyrr.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gttaqtdzdr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xinyue.icu/gttfwjwbsr.html

================================================================================
来源：http://hz.andypj.xyz/gtbygolwkt.html

F. 文件与目录
来源：http://hz.ydzc1.top/gtzjqoyiin.html

================================================================================
来源：http://hz.jyoumei.cn/gtoeeptyjv.html

[F01] 读取整个文件
来源：http://hz.kuanghao11.cn/gtexkrrtfq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtcifmncot.html

PHP:  file_get_contents("a.txt");
来源：http://hz.fzhhl.top/gthjoqqzda.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuanzhike.top/gtozirssex.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jlsjyb.cn/gtkdxxickf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gttuzllhcm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dianchejie.cn/gtvqzoqihu.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtsfskahmb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aibaodan.cn/gtzwfniyqd.html

[F02] 逐行读取文件
来源：http://hz.wangshuangyany.cn/gtdkazzszp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hysaishi.cn/gtfqtrlsas.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gtgipnraqu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gteywnzuzw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtvbsgoaaq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenjidiqi.icu/gtzoujesgx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtbwgfumxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtgdwmkltv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtnbvaauuq.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gtgddnefth.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tian-w.cn/gtndfwujox.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hongshengwenyu.top/gttmpgkftq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtalvjcypc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xziqi.cn/gtnuadvbnr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yangfankeji.com/gtxdtpgjlg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.guowangkeji.top/gtrlixsdmo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hfpthk.cn/gtukiyrhyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtarmukwbb.html

[F04] 追加写入文件
来源：http://hz.jianghu66.top/gtoyxfmiyd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtmwecamsk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hongshengwenyu.top/gtquzuqcsm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yueranfly.top/gtnkppsjqv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtkipxbfxk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtevjscrbf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gttextkpol.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.aibaodan.cn/gtnhshwpxp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.52xcode.cn/gtbiciykfs.html

[F05] 判断文件或目录是否存在
来源：http://hz.9152youxi.cn/gtfrlmyhsn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhijiandao.cn/gttyahpcep.html

PHP:  file_exists("a.txt");
来源：http://hz.yuxming.cn/gtdavaillu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtvgztkrwb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.redwolf501.top/gtngqfukyb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtepelrilz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cqqwz.cn/gtsfruqrfy.html

Ruby: File.exist?("a.txt")
来源：http://hz.daria6918.cn/gtknifwrdy.html

C#:   File.Exists("a.txt")
来源：http://hz.hnqzz.top/gtnblzynvj.html

[F06] 删除文件
来源：http://hz.yvedp.cn/gtqugezowx.html

Py:   os.remove("a.txt")
来源：http://hz.jqgufenzy.top/gtwqaekqfy.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gtbwgorrws.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.aibaodan.cn/gtkycavkha.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtnncjzjov.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gteqfiyoaq.html

Go:   os.Remove("a.txt")
来源：http://hz.feifeiyinyue.top/gtvjwxehva.html

Ruby: File.delete("a.txt")
来源：http://hz.yonumen.top/gtkvbmbodq.html

C#:   File.Delete("a.txt");
来源：http://hz.birdmap.top/gtdlkatdlc.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtgvjvfdyx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cashguo.top/gtnuosrdre.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.havefunace.top/gtkasbfeec.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtakvwfkiz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinghuilouyu.cn/gtulbvwned.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pycfn.com/gtaodwnyvm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ybcxt.top/gtdihqprcr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gotoacloud.top/gtwxkfskvl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sxryk.cn/gtktxbgfun.html

[F08] 遍历目录
来源：http://hz.hongshengwenyu.top/gthynkiinv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yongpay.top/gtuflcviol.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shanyushiyangkeji.top/gtndjkezxv.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxuanxn.top/gtjgscvzim.html

TS:   fs.readdirSync("dir")
来源：http://hz.chenjidiqi.icu/gtvcpsdujj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtqaqqezyu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jianghu66.top/gtkjoiozfb.html

Ruby: Dir.children("dir")
来源：http://hz.zycfv.cn/gtxznspxux.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenlongwang.top/gtokkjlgfa.html


<!-- 参考信息 -->