代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtliuaxiin.html

[D20] 统计每个元素出现次数
来源：http://hz.gotoacloud.top/gtzsglshuy.html

Py:   Counter(arr)
来源：http://hz.ywan-chungtsiang.top/gttkhlpyci.html

PHP:  array_count_values($arr);
来源：http://hz.yonumen.top/gtjalzbmhf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtpcknpiuc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtfhzgbtgj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhijiandao.cn/gtxqinfkai.html

Go:   // 手写 map[T]int
来源：http://hz.gaohongyu789.top/gtzwplbybr.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtriasrhli.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cashguo.top/gtqizllocm.html

[D21] 判断是否包含某元素
来源：http://hz.yuxming.cn/gtnfzfdtjg.html

Py:   x in arr
来源：http://hz.sufxvd.cn/gtfmlrzaep.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtckxixigz.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtccbelbtg.html

TS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtklgoubry.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtjigsibmp.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydjk.org.cn/gtwuyijxfu.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gtddknlojk.html

C#:   list.Contains(x)
来源：http://hz.hfpthk.cn/gtqskqbysk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.bjfxy.top/gteabnfgkc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ehwqpu.com/gtbjfmdukz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtrhfvvcdm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.52xcode.cn/gtoodjjxeh.html

TS:   [...arr];
来源：http://hz.zhongyouzk.top/gtuyfpbdyy.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtkczpdixd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.vqdsnc.cn/gtkrwetrte.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gtjajjrlxu.html

C#:   new List<int>(list);
来源：http://hz.gaohongyu789.top/gtcvlllvuf.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtygxkpsbw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.gzhubu.top/gtmuivavhl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.vqdsnc.cn/gtclqxmbqg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtipriywux.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtujudwwig.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnqzz.top/gtypsiiefi.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtaplmfuby.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigfzy.top/gtekwlhtop.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtdrpgkblp.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtydmfbgnb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuetiantiany.cn/gtflxthjxo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhixingplan.top/gtjqodviva.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pycfn.com/gtavcpxgql.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gogol.net.cn/gtoacfwkam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jiagoushi.top/gtyahkjpsd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sufxvd.cn/gtjcwhnpin.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gthjxcqxzh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.birdmap.top/gtzyqijmtl.html

[D25] Set 集合去重与交并差
来源：http://hz.ivvv.top/gtflsvfzvp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pengpengdd.cyou/gtomikyrfl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtygeuyals.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtkvpuajpj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtabxmuwav.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hnxiangtu.top/gtxhubbeld.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gteivgbycm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.fzhhl.top/gtdrvophlm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.pengpengdd.cyou/gtakdceruz.html

[D26] 数组转字符串
来源：http://hz.havefunace.top/gtmfidlkph.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenzaomai.com/gtujtywncv.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtzsfmwbks.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtqljimphg.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtlloowaij.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gttnpzhszn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtxkglajzn.html

Ruby: arr.join(", ")
来源：http://hz.yvedp.cn/gtunfgssvk.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtwwqinysi.html

================================================================================
来源：http://hz.jinqigufen.top/gtywmanpps.html

E. 字符串处理
来源：http://hz.ppjwa.cn/gtfzdrylmj.html

================================================================================
来源：http://hz.xuanzx.com/gtxteeriqb.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtlhomspks.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.316326.xyz/gtbslgszii.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgfzy.top/gtrsllvdlq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtucbmjvul.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtxbyfxvrl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtkvgriutt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gtrfghnjzg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.9152youxi.cn/gtpmvyfvdu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sufxvd.cn/gtuseowksq.html

[E02] 重复字符串
来源：http://hz.yongpay.top/gtbedocwyz.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtwdynvrqa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtrgqnkwir.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtldrdkjxj.html

TS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtmcnqrrfo.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtpfermfrk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtilesqfyb.html

Ruby: "ab" * 3
来源：http://hz.hnqzz.top/gttntglngq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtmvxpcxgh.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gttutrnkpz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hfpthk.cn/gttnfcabsp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258888.top/gtfgabcqoh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtdwggtgxq.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtviyaunwu.html

Java: s.substring(1, 4)
来源：http://hz.hongshengwenyu.top/gtbwummujl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pengpengdd.cyou/gtlxiprolp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtyjwitoyj.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtbqoiecxe.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtxusztcjv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtkksewokg.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigfzy.top/gtlweduddu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.guannengcc.top/gtuytrsuvo.html

TS:   s.indexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtachiiczu.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtxplpfpcn.html

Go:   strings.Index(s, "x")
来源：http://hz.yj202588.top/gtdklhhxuo.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gtvcpswcuc.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtantktjzi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yongpay.top/gtzlvonjgb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gttzauxrom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtzxwtpugl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtccjsmegc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtnoeoujot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenzaomai.com/gtxsoofgfb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtpgodmkfl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtygeafgdk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtoecbxhgj.html

[E06] 替换子串
来源：http://hz.birdmap.top/gthatbrjmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gttuvupilz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtgnncskwi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtuuwzuuxh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtgomxiwvz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gthifzcncq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhongyouzk.top/gtihkphjpt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gttxotyeoo.html

C#:   s.Replace("a", "b")
来源：http://hz.nwbrower.top/gtuwnhkwkd.html

[E07] 按分隔符拆分
来源：http://hz.yongpay.top/gtaiahybru.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhongyouzk.top/gtbywlfnil.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gtbocjfdho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.tianlin.xyz/gtmgawkeuk.html

TS:   s.split(",")
来源：http://hz.cdnleiting.top/gteqifgqyb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yongpay.top/gtuogrezcu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhijiandao.cn/gtlxyrhcvx.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtfgfrnptr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ppjwa.cn/gtstfeyzcy.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258888.top/gtarzuwuyi.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtuzxpmswk.html

PHP:  implode(",", $items);
来源：http://hz.shanyushiyangtech.top/gtszwgirrj.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtwctcjbpn.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtkzojwpex.html

Java: String.join(",", items)
来源：http://hz.shuidangran.top/gtvvisqare.html

Go:   strings.Join(items, ",")
来源：http://hz.snrcjt.cn/gtvzyzezee.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gtcyrspakt.html

C#:   string.Join(",", items)
来源：http://hz.hongshengwenyu.top/gthxgdotvs.html

[E09] 去除所有空白字符
来源：http://hz.gotoacloud.top/gtzlquepdn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gthxwuhqkq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtvlknasyc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtbtuxzghn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtksidaiii.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jinyuanbaomall.cn/gttcyfudnh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtddaqarxi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtougznajy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gtywyapcmz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xuetiantiany.cn/gtoatslosb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangtech.top/gtsnbmendz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ppjwa.cn/gtisrhljco.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtukmyxhko.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gteufegbkf.html

Java: String.format("%03d", 7)
来源：http://hz.hfpthk.cn/gtrotwvaee.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nwbrower.top/gtolrldpkv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.mhx1999.top/gtqffqshuy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtpauutiam.html

[E11] 反转字符串
来源：http://hz.jqgfzy.top/gthhmlxqla.html

Py:   s[::-1]
来源：http://hz.c1oappe.top/gtovsyfbga.html

PHP:  strrev($s);
来源：http://hz.gotoacloud.top/gtoaggtnes.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtdkulketv.html

TS:   [...s].reverse().join("")
来源：http://hz.9152youxi.cn/gtlpjwomlp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtzpnvscgv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.andypj.xyz/gtqdnmycig.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtwjmzoheb.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtfzmwfgou.html

[E12] 统计某字符出现次数
来源：http://hz.yuxming.cn/gtnldlirjm.html

Py:   s.count("a")
来源：http://hz.meibo888.top/gtshvpfqea.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtldnjhwgw.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtqstlyxht.html

TS:   s.split("a").length - 1
来源：http://hz.ivvv.top/gtzgggxjsb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.pengpengdd.cyou/gtvonbjyxq.html

Go:   strings.Count(s, "a")
来源：http://hz.hammf.cn/gtzhyaajgo.html

Ruby: s.count("a")
来源：http://hz.yonumen.top/gtyjjnvsfw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuanzx.com/gtlwoahvwv.html

[E13] 逐字符遍历
来源：http://hz.svipenyu.cn/gtnvgrgqnp.html

Py:   for ch in s: print(ch)
来源：http://hz.vqdsnc.cn/gtahtujxdc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gtoqqqsipd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtypnrfimx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gtzqdgjtyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hongshengwenyu.top/gttwhyedac.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.vqdsnc.cn/gtcafmrkyz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gttaydumdd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtgjqtpauj.html

[E14] URL 编码与 Base64
来源：http://hz.wangdashe.top/gtyhexdygv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangtech.top/gtezgsnzqi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yvedp.cn/gtcnggmzfl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtfwlwmmsn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gogol.net.cn/gtwcfzomwa.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtmywxsynr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.fengsongda.top/gterxldkvx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aizwys.cn/gtgyfwgxbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtfhcrndxz.html

[E15] HTML 转义 / 反转义
来源：http://hz.jiagoushi.top/gtxxdttafc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.iojbl.cn/gtjxfjkhfs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guowangkeji.top/gtecxhkbmh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hfpthk.cn/gtknwcqfwk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtupshrcko.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangkeji.top/gtmlvzqlba.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtkozutnit.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.c1oappe.top/gtrphetqkq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.nwbrower.top/gtczzqnomi.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtycmdmimp.html

Py:   f"{1234567:,}"
来源：http://hz.hfpthk.cn/gtrfwdexna.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtbwjubarx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtjspbessg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtnzqwagxp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hywenlv.cn/gthhxiaerg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhiwuduotai.top/gtybplircy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.quarkkingdee.top/gtydwsenyf.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtwjauhsba.html

[E17] 首字母大写
来源：http://hz.zhoulong.xyz/gtcuwzamfk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtwiidtjps.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.xinyue.icu/gtbcgzqfmc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gttnfzxfeo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhixingplan.top/gtrfewxdff.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yuxming.cn/gtqbluszsj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtsyjmwqqa.html

Ruby: s.capitalize
来源：http://hz.mhx1999.top/gtojartcgb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtrvuwrxqd.html

[E18] 模板占位符替换
来源：http://hz.chenzaomai.com/gtddxtcakk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtifcvmkpk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yangfankeji.com/gtmepwdjlf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtvrebjweb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtisydroug.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gthcoeopoc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.smart0.xyz/gtlhftvagf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtjqgdysni.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jianghu66.top/gtjkfemyta.html

[E19] 多行文本按行拆分
来源：http://hz.nanxuanxn.top/gtzhvmcopp.html

Py:   s.splitlines()
来源：http://hz.zhijiandao.cn/gtnqbibhrh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hywenlv.cn/gtddmmytvv.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtnrvjlzsd.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gthekjmyyf.html

Java: s.lines().toList()
来源：http://hz.haohaochexian.top/gtgjwgahth.html

Go:   strings.Split(s, "\n")
来源：http://hz.9152youxi.cn/gtkhfdkqyq.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtxiiustek.html

C#:   s.Split('\n')
来源：http://hz.hfpthk.cn/gtxjcfhxzd.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtsvnsactd.html

Py:   if not s:
来源：http://hz.daxiang520.top/gtqdxmgqjh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtmgjqfjcw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.9152youxi.cn/gtvxokvaph.html

TS:   if (s === "") {}
来源：http://hz.guowangkeji.top/gtiycksvnz.html

Java: if (s.isEmpty()) {}
来源：http://hz.quarkkingdee.top/gtydsnuvnz.html

Go:   if s == "" {}
来源：http://hz.birdmap.top/gtvkgpuqii.html

Ruby: if s.empty?
来源：http://hz.hammf.cn/gtpjdisshw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtqingzcwn.html

[E21] 超长截断加省略号
来源：http://hz.jinyuanbaomall.cn/gtqivhblni.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sysykeji.top/gtlxpuonvb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jlsjyb.cn/gtquctymdz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtivngrifi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtxjlpcwki.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gtmlpukrwn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xylfe.cn/gtmpsbjaht.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dashuyun.cn/gtkkrzuwue.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jianghu66.top/gtpequauug.html

[E22] 字节长度与字符长度
来源：http://hz.sweek.top/gtbthvsxaw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shanyushiyangkeji.top/gtzecpcehd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.nanxuanxn.top/gtahilflaa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gtisnhhykd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtmmijloky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dianchejie.cn/gtzesuzygr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jyoumei.cn/gtughivivv.html

Ruby: s.bytesize;  s.length
来源：http://hz.tianlin.xyz/gtxwbqfqql.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.52xcode.cn/gtoenzhrus.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsjnqxjju.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtntbdwqdj.html

================================================================================
来源：http://hz.tanke756.top/gtuejjbkdd.html

[F01] 读取整个文件
来源：http://hz.havefunace.top/gtqtzkzrbo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gogol.net.cn/gtcrkfxexj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtztlqxooh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhaomingkeji.xyz/gtelehjevs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgufenzy.top/gtwpygqhom.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtglzpwvxp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuetiantiany.cn/gtuoypwaql.html

Ruby: File.read("a.txt")
来源：http://hz.ybcxt.top/gtzdderzuo.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ivvv.top/gtlrvomewu.html

[F02] 逐行读取文件
来源：http://hz.jianghu66.top/gtnniwannv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtrkeeblts.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cdnleiting.top/gtlzbsladq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtecqpxlac.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtzmclofbi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gtyhlmmdqc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhoulong.xyz/gtspmcevar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hammf.cn/gtgalrrpia.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.feifeiyinyue.top/gtyahjeoun.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtwjajdisp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtelyivjdu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xinyue.icu/gtmxziiezj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtuwyehsny.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daxiang520.top/gtnpsavqsj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.9152youxi.cn/gtsdadkbkt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.nanxuanxn.top/gtbmnvvxat.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj202588.top/gtkfiafahe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtkesdwtlu.html

[F04] 追加写入文件
来源：http://hz.chenlongwang.top/gtkniooblv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jiagoushi.top/gtetjqqufo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuanzx.com/gterpmdurq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtstsiinkk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuxming.cn/gtvdzpctkg.html


<!-- 参考信息 -->