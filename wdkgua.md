代发 wailian999

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtzutnzgfk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtjaifrewr.html

[D21] 判断是否包含某元素
来源：http://hz.aizwys.cn/gtegzsmzlm.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtxfjoekct.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtavlarhxl.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtqtyqplpr.html

TS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtzmzhwocb.html

Java: list.contains(x)
来源：http://hz.wangdashe.top/gtfmclefjn.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtxgohjckv.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gtvsqleimh.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtcntjfbnd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.svipenyu.cn/gtpsfyyfhu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aizwys.cn/gtignkzipe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnxiangtu.top/gtzgvpjqmd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gotoacloud.top/gtpvvwiasw.html

TS:   [...arr];
来源：http://hz.zhixingplan.top/gtecpjbrqq.html

Java: new ArrayList<>(list);
来源：http://hz.shanyushiyangkeji.top/gtiherebkv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gzhubu.top/gtavayqoum.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtqyqotstk.html

C#:   new List<int>(list);
来源：http://hz.jinqigufen.top/gtnwlaafcp.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gtlcgnqula.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guannengcc.top/gthkaxfoao.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnqzz.top/gtjrwujxhq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtgrkkpmpq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtfzpvaszx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dianchejie.cn/gtoifkupyn.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtswnfluhk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jyoumei.cn/gtzfceflmu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtlrctxqjh.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtelfmzcgq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gteyfwbniv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gtkxjnginl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtbucpphsh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shanyushiyangtech.top/gterrjkate.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhijiandao.cn/gtfobesujz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtyhchjpxe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtzekylnxi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtvrkaogiy.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gtsxwmckar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtryhblrxl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtsthodazq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gtqvdwrsip.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ivvv.top/gtlysoyobt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtxexhgont.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pengpengdd.cyou/gtonhcuuyx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258888.top/gtnaiyayrf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtzclqqfkl.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtarmfpctx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.mhx1999.top/gtyqtuzkop.html

PHP:  implode(", ", $arr);
来源：http://hz.pengpengdd.cyou/gtmbnhtcye.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtyswzubsv.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtjcchrvdg.html

Java: String.join(", ", list)
来源：http://hz.fengsongda.top/gtgrtofqkm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258888.top/gtnuaegiit.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtqhqnulqn.html

C#:   string.Join(", ", list)
来源：http://hz.fzhhl.top/gtuzfnmycq.html

================================================================================
来源：http://hz.cqqwz.cn/gtwpdthkub.html

E. 字符串处理
来源：http://hz.birdmap.top/gtfszxxsnl.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbxwmcmtz.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gthckaajsd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fzhhl.top/gtzaghzajv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tian-w.cn/gtveogvboi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtnnltlksc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtqqteleng.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jqgufenzy.top/gtvibvpowm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinqigufen.top/gtxdcwhiab.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jianghu66.top/gtgnvyuksk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtyizwphxo.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtmsfefoin.html

Py:   "ab" * 3
来源：http://hz.zhoulong.xyz/gtrlqhraqt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtogjzrrkq.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtkzsjcuio.html

TS:   "ab".repeat(3)
来源：http://hz.ybcxt.top/gthapdwmoz.html

Java: "ab".repeat(3)
来源：http://hz.birdmap.top/gteoqxqygo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gtlxvwpewx.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtyhffjaov.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zdqjudy.top/gtehtjhtla.html

[E03] 截取子串
来源：http://hz.svipenyu.cn/gtibpyedhc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xingfuxueyuan.xyz/gtpufdboqd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yonumen.top/gtmtfiifzp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtdyblwlgl.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtqxreswht.html

Java: s.substring(1, 4)
来源：http://hz.daria6918.cn/gtsfpjgkxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yongpay.top/gtygnqixmn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yj20258.top/gtrpgqbscv.html

C#:   s.Substring(1, 3)
来源：http://hz.jianghu66.top/gtkynrzvyn.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtqsaprcyj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aibaodan.cn/gtvqhmqvrn.html

PHP:  strpos($s, "x");
来源：http://hz.haohaochexian.top/gtdtywxnvv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hongshengwenyu.top/gtcehjpcvb.html

TS:   s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtkbpoxzqv.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gtxzgbnsls.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtsiesggtl.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtiphhwonw.html

C#:   s.IndexOf("x")
来源：http://hz.316326.xyz/gtjhqscfbk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gthpanhepr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtlipdzqvn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenzaomai.com/gtzdbmwqsx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtnrswepxc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.316326.xyz/gtjhamjidz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gtrpzzgivj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.guowangkeji.top/gtjuqrzicj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuxming.cn/gteeovqfeg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.quarkkingdee.top/gtdyprfguj.html

[E06] 替换子串
来源：http://hz.daxiang520.top/gtlfufzdku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gtygryjsje.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ywan-chungtsiang.top/gtuqntjqod.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtiovyygcl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtiameskps.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtjhlzxgel.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fzhhl.top/gtjoutgnso.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cheryme.top/gtgkhsdlbl.html

C#:   s.Replace("a", "b")
来源：http://hz.yangfankeji.com/gtwscjhiri.html

[E07] 按分隔符拆分
来源：http://hz.dashuyun.cn/gtptjneczl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.kuanghao11.cn/gtwsyezrrq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jyoumei.cn/gtugoxgtej.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtlohrgdjo.html

TS:   s.split(",")
来源：http://hz.kuanghao11.cn/gtdovjaplv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tianlin.xyz/gtsiopakyx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinghuilouyu.cn/gtcvuvjduc.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtryczwptg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gtxqzqpjdp.html

[E08] 数组按分隔符合并
来源：http://hz.aibaodan.cn/gtxjoqwyxm.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtatxwffip.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtxozenxrq.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtixlnazlf.html

TS:   items.join(",")
来源：http://hz.sysykeji.top/gtxbcjcukp.html

Java: String.join(",", items)
来源：http://hz.birdmap.top/gtahdrlgxg.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtebllyrwm.html

Ruby: items.join(",")
来源：http://hz.shangyingyoupin.top/gtabtbonym.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtpgjgmtdy.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gthjvzwlbt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtovyybfgk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sweek.top/gtekovlmhb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtoznfnkai.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuanzhike.top/gtfbchwrxa.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtdwskqpvg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtfznwxoph.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ppjwa.cn/gtkwgapvgl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hysaishi.cn/gtgelkyicd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtkyjapyuc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gtsflsfsaa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtaoglcxox.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinqigufen.top/gtvpatihsy.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtyyaqtcbf.html

Java: String.format("%03d", 7)
来源：http://hz.zhijiandao.cn/gtwqfblfqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hysaishi.cn/gtuudjgquo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuxming.cn/gtlaqgdyhr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtwmswivkg.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtgiunkeep.html

Py:   s[::-1]
来源：http://hz.52xcode.cn/gtzlvhlaxr.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtykffrdlo.html

JS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtscycbkss.html

TS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtljuvzxoq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jqgufenzy.top/gtkrsobwmf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtiwnpcthy.html

Ruby: s.reverse
来源：http://hz.cashguo.top/gtoumfftdv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gtheqjdiug.html

[E12] 统计某字符出现次数
来源：http://hz.cqqwz.cn/gtdnibavng.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtbgycsxgc.html

PHP:  substr_count($s, "a");
来源：http://hz.nanxinkj.top/gtotvnwxyr.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtxyjyqtbk.html

TS:   s.split("a").length - 1
来源：http://hz.nanxuanxn.top/gtvnowdnqg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhijiandao.cn/gtlzzoxxez.html

Go:   strings.Count(s, "a")
来源：http://hz.cqqwz.cn/gtdakiowzj.html

Ruby: s.count("a")
来源：http://hz.ehwqpu.com/gtuumcwzbd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ehwqpu.com/gtqygbwber.html

[E13] 逐字符遍历
来源：http://hz.zycfv.cn/gtscpzbnpq.html

Py:   for ch in s: print(ch)
来源：http://hz.hywenlv.cn/gtwjfelkzx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.9152youxi.cn/gtuqfztwkz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tanke756.top/gtcjbombtf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtugvkyypr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtjqpgcclh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yvedp.cn/gtzvqrauth.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangdashe.top/gtmgryppju.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtiunsrghq.html

[E14] URL 编码与 Base64
来源：http://hz.fengsongda.top/gthtegbksy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gtsvpzoxjf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yj20258888.top/gtyfblcaub.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtqgvewczb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtkqleomtv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yueranfly.top/gtjwuivbdc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhoulong.xyz/gtytuqzkcb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jyoumei.cn/gtzkurrqvb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtyenlfajq.html

[E15] HTML 转义 / 反转义
来源：http://hz.hongshengwenyu.top/gtatpmnuuq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zycfv.cn/gtvhprelne.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxuanxn.top/gtwiqvdxnw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtaaqlvqco.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtujplnncc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gthflpykhb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.pengpengdd.cyou/gtvbakqjud.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.svipenyu.cn/gtblodbfdk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.vqdsnc.cn/gtzavxpzxm.html

[E16] 数字千分位
来源：http://hz.snrcjt.cn/gtvbbupjrg.html

Py:   f"{1234567:,}"
来源：http://hz.quarkkingdee.top/gtktptslco.html

PHP:  number_format(1234567);
来源：http://hz.zhengqikj.top/gtddpdonjy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cheryme.top/gtznmdjwyl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtuofuhmci.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.smart0.xyz/gthsleegqp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtgtfpggci.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258888.top/gtmarxgliw.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxinkj.top/gtjaidmzor.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtyvixpqgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hywenlv.cn/gtmtpnaqnz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtrhpyfpec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtabeuhuuy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.316326.xyz/gtxjmxdyyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gtpdnnsnjl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtnbmxqawl.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtpyvafisf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yangfankeji.com/gtarinsfjb.html

[E18] 模板占位符替换
来源：http://hz.yangfankeji.com/gtrzirlltq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtwlrthotn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dianchejie.cn/gtfjwybqjd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtztzrglza.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.bjfxy.top/gtkyiblbdk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtllracoti.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtzjpopxll.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhoulong.xyz/gtspzwxfhd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtwtkmxgvv.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtwcimxmty.html

Py:   s.splitlines()
来源：http://hz.cucudq.cn/gtvbcpctzi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtwvsidisi.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnxiangtu.top/gtkhkyssgn.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gtojcocvjw.html

Java: s.lines().toList()
来源：http://hz.316326.xyz/gtvghxrsmx.html

Go:   strings.Split(s, "\n")
来源：http://hz.ybcxt.top/gtarlytovn.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtqtibjjpb.html

C#:   s.Split('\n')
来源：http://hz.guowangkeji.top/gtjmwnukxs.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtkntnqrxs.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtnrkpaloh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gttfchflrq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yanxiufei.cn/gtlehrlvvh.html

TS:   if (s === "") {}
来源：http://hz.guowangkeji.top/gtvdylpged.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtibfooksf.html

Go:   if s == "" {}
来源：http://hz.hysaishi.cn/gtxkligprm.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtsfmqbiwp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tanke756.top/gtbllsjurl.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtpyfudbsn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtvvqeeawj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtksaepega.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yongpay.top/gtcpwkhevb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ybcxt.top/gtlgxhybdi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtujuwoidh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.havefunace.top/gtownzgdkl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daxiang520.top/gtiqpjbthw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtormhejbm.html

[E22] 字节长度与字符长度
来源：http://hz.yanxiufei.cn/gttwrturud.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.kuanghao11.cn/gtwqitqneb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhoulong.xyz/gtfgzdlnyy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtnaeyfowk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtjimkrxun.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxinkj.top/gtwehbflym.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj20258888.top/gtmwxpzozr.html

Ruby: s.bytesize;  s.length
来源：http://hz.hfpthk.cn/gtudbnjhub.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtrmyhakew.html

================================================================================
来源：http://hz.dashuyun.cn/gtzdsjqwal.html

F. 文件与目录
来源：http://hz.dashuyun.cn/gtbdtqyrub.html

================================================================================
来源：http://hz.jinqigfzy.top/gtrcouxopc.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtdxkdrnkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cdnleiting.top/gttuidnjxb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtlbfbrjhx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.meibo888.top/gtevdsoccu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtxyjlvgjy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtccifmchl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jyoumei.cn/gtiafjricz.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gtlvrdeatw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxuanxn.top/gtupkpyvbe.html

[F02] 逐行读取文件
来源：http://hz.tian-w.cn/gtibtdffxw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtxqahisxl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hongshengwenyu.top/gtqirzkpza.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.havefunace.top/gtwsxiyubx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtlgabwlbu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cheryme.top/gtjbgvnnwh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hywenlv.cn/gtxgkchvvm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtyazoqtkz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sysykeji.top/gtourujsbq.html

[F03] 写入文件（覆盖）
来源：http://hz.fzhhl.top/gtrsyzmfjo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.birdmap.top/gthacioaot.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gtjlseoinh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gthyajietb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtjcjxuwgh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gtgucqlbxc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fengsongda.top/gtonubdrmd.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtjxuzltkz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtvpgjmzhz.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gteunmqlwx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinghuilouyu.cn/gtturzzulc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtdiphymyu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtkuqmfzeb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtyxllxsaa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cucudq.cn/gtbejphxrw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtctqsrflv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhoulong.xyz/gtzlyfdpni.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.haohaochexian.top/gtrgrwxciu.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtbdbpjhxa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.fengsongda.top/gtszukifxq.html

PHP:  file_exists("a.txt");
来源：http://hz.chenlongwang.top/gtdsvbfkzn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtltixdwgg.html


<!-- 参考信息 -->