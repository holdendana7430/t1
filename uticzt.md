代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hfpthk.cn/gtvdheonwq.html

Go:   // 手写双层循环
来源：http://hz.0kj1m.cn/gtixadcgmd.html

Ruby: nested.flatten
来源：http://hz.zhengqikj.top/gtaluqjoqo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtdxwvkiyb.html

[D19] 按字段分组
来源：http://hz.hnqzz.top/gtdrlcqwfx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtxweidesl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shuidangran.top/gtukbmqbql.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtydspftge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tanke756.top/gtumaevdsm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtveiigywq.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtephjgbyc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtiizpzqlp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xinyue.icu/gtczdrbpyl.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gtvzonvizi.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtygolfhlf.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtyqfanusz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxinkj.top/gtfemxjvkw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtdjzsksmj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxuanxn.top/gtsnyahnbj.html

Go:   // 手写 map[T]int
来源：http://hz.shangyingyoupin.top/gtysvrhmue.html

Ruby: arr.tally
来源：http://hz.sweek.top/gtdftxesxk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtrzaqkynp.html

[D21] 判断是否包含某元素
来源：http://hz.tian-w.cn/gtuhynejiq.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtbubbkxgq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gtwazrgfak.html

JS:   arr.includes(x)
来源：http://hz.pycfn.com/gtytaxuvnq.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtgainauhz.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtworbijfb.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxuanxn.top/gtpraqnjow.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtirqtloug.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtnkilisof.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gotoacloud.top/gtvdutnazv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ywan-chungtsiang.top/gtglbeewbh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtbgodyquu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtgobtkmoz.html

TS:   [...arr];
来源：http://hz.cheryme.top/gtgqnwzirs.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtodlfhzyw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtaderjdsh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtmhrvshlf.html

C#:   new List<int>(list);
来源：http://hz.smart0.xyz/gtpqrvalwt.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtwatdxisf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtsjidhexy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtucfrxhdq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gtgtbwhrlb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtizzwkfnh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtvgqlfusr.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtmmnujabx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gtdbslayqd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuanzx.com/gtklmowamo.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtlxtfwcvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.kuanghao11.cn/gtxsrptmjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gtypyynjda.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtuzsmitsa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtscpbufcb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigfzy.top/gttslbhvwk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.316326.xyz/gtcuzmjqnm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxuanxn.top/gtrbawjbeh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jyoumei.cn/gtgsihjxwi.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gtwutjovuh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cqqwz.cn/gtjzfayilk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtpfrvcuzu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhaomingkeji.xyz/gtnyevwtzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtenmadlsd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258.top/gtislqgyrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pengpengdd.cyou/gtippgwvye.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuetiantiany.cn/gtjmkgjmrd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yanxiufei.cn/gtdmkexwty.html

[D26] 数组转字符串
来源：http://hz.wangdashe.top/gtqstbkcgk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydjk.org.cn/gtuncaqguq.html

PHP:  implode(", ", $arr);
来源：http://hz.zhiwuduotai.top/gtfkszphut.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtnnvyjoef.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtfeepewpj.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtqecphxhj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gttmgmaqys.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtrirgujpb.html

C#:   string.Join(", ", list)
来源：http://hz.nwbrower.top/gtsmtanxdx.html

================================================================================
来源：http://hz.gogol.net.cn/gtjxajlslh.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gtoxvbadxl.html

================================================================================
来源：http://hz.sysykeji.top/gtuexrjgle.html

[E01] 拼接字符串
来源：http://hz.quarkkingdee.top/gtelqmviua.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtpudvwqvl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cashguo.top/gtsivhfrlm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtqrkharjs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtldsvpivr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gtrbyjhlvx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtjbstkcxr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cheryme.top/gtsydhhcpe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtzujzmigu.html

[E02] 重复字符串
来源：http://hz.yanxiufei.cn/gtgbxmzcih.html

Py:   "ab" * 3
来源：http://hz.andypj.xyz/gtwcnpylfx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtvnzdksvc.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtopxtqedl.html

TS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtqvlmrfme.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtesrrynrx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinghuilouyu.cn/gtpsjxalvm.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtthxpquzz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gtujysfpko.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtqcztxfkn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gthhntqqwp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gtckxungol.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtdbsyimoa.html

TS:   s.slice(1, 4)
来源：http://hz.yanxiufei.cn/gtqifwyzyg.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gttielwpav.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cashguo.top/gtyyyitmay.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dianchejie.cn/gtnfibwjim.html

C#:   s.Substring(1, 3)
来源：http://hz.fengsongda.top/gtntnqipae.html

[E04] 查找子串位置
来源：http://hz.fengsongda.top/gtphymufvj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxuanxn.top/gtqoonjhfp.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtwisekxja.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gtkgibithr.html

TS:   s.indexOf("x")
来源：http://hz.andypj.xyz/gtwgoiscpn.html

Java: s.indexOf("x")
来源：http://hz.jiagoushi.top/gtidflfpel.html

Go:   strings.Index(s, "x")
来源：http://hz.zhengqikj.top/gtedvjjobr.html

Ruby: s.index("x")
来源：http://hz.hnxiangtu.top/gtdnpwlnnw.html

C#:   s.IndexOf("x")
来源：http://hz.yj202588.top/gtlavaooag.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigufen.top/gtzpemxvij.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gzhubu.top/gtthmzinuk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtfddjigxc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pengpengdd.cyou/gteoxwsgov.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jlsjyb.cn/gtylnwbesh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtnkyuzcoi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cashguo.top/gtyknlihgf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.guowangkeji.top/gtwwwaxdow.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gogol.net.cn/gtnnuuxfze.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gttqaawwuh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtjsqcyoup.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.ehwqpu.com/gtvommglzu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtzodswemo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gttbswzykg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtdqmhodso.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gtlxqsoain.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtgmvdwiij.html

C#:   s.Replace("a", "b")
来源：http://hz.yj202588.top/gtqhwfiroc.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtuufxjkjb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jlsjyb.cn/gtpabrqzvg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtflimmavq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangkeji.top/gtowlawqyv.html

TS:   s.split(",")
来源：http://hz.zhoulong.xyz/gtsxkimwnq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtxgapxcmc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258888.top/gtveljvpwt.html

Ruby: s.split(",");  s.split
来源：http://hz.haohaochexian.top/gtccpiaeyv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nwbrower.top/gtrkpyujni.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtkuckxdor.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gttpgdagod.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtmfyobpgo.html

JS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtrhjbhwov.html

TS:   items.join(",")
来源：http://hz.dianchejie.cn/gtzmkfpmgp.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtbqkysmds.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtzbdjpaln.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtyiuxlxiu.html

C#:   string.Join(",", items)
来源：http://hz.shuidangran.top/gtyvqgytdu.html

[E09] 去除所有空白字符
来源：http://hz.birdmap.top/gtppsjbwov.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gzhubu.top/gtmjmboegt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gogol.net.cn/gtsjklzitd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtvntgnudb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtjgmzaoif.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtgnhutnxb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yj20258888.top/gtbmhltgwi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtdqpdgvap.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.andypj.xyz/gtevsizmgh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtpllzlixu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jianghu66.top/gtosqauhln.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtzdjjpekj.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtrmhyjsmk.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtvofbjmuq.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gtukpyiubi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhoulong.xyz/gtgtoyeljy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtplbauhed.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nwbrower.top/gtbzrelcpt.html

[E11] 反转字符串
来源：http://hz.sxryk.cn/gtcxrhfinm.html

Py:   s[::-1]
来源：http://hz.yuanzhike.top/gtglebfdot.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtxelcsffm.html

JS:   [...s].reverse().join("")
来源：http://hz.c1oappe.top/gttwitrzey.html

TS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtoapcrnkz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.svipenyu.cn/gtdoxkvpqs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtkddriyxh.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtpyskdxxp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtzvgtlvdq.html

[E12] 统计某字符出现次数
来源：http://hz.hfpthk.cn/gtgtdyavbo.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtrnqxmgsr.html

PHP:  substr_count($s, "a");
来源：http://hz.yueranfly.top/gtsiycwtdb.html

JS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gtswpaicme.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtylizxamu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuetiantiany.cn/gtpxnkwoqg.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtqjfpxdnc.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gtekiyjjfg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gtuadqcpsq.html

[E13] 逐字符遍历
来源：http://hz.ivvv.top/gtxmvyoapq.html

Py:   for ch in s: print(ch)
来源：http://hz.yonumen.top/gtypgjzjey.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yvedp.cn/gtrgmewsmj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtgkyckouc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gthxgtoyyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtjatbqsxo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gaohongyu789.top/gtnqakueag.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtybqhxrlm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sufxvd.cn/gtiiajemar.html

[E14] URL 编码与 Base64
来源：http://hz.vqdsnc.cn/gtbyigyjrq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hysaishi.cn/gtvshizhyd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shanyushiyangkeji.top/gtjxctegwa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.bjfxy.top/gtibtargtk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.tanke756.top/gtwqchhukx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sufxvd.cn/gtsymwfsmo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtpihfrzlp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtmufxguks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtbukhmhom.html

[E15] HTML 转义 / 反转义
来源：http://hz.gzhubu.top/gtpqxypwdo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aizwys.cn/gtzaksoyti.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtdethdwoi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gthjxmusne.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtxefqkcgp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtepprvftd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtqalkzvdb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shanyushiyangtech.top/gtslvmdkli.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtohvndlvv.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtzafodpas.html

Py:   f"{1234567:,}"
来源：http://hz.smart0.xyz/gtroarexlr.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtwqutplwq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.pycfn.com/gtpownytvr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtqjztqqlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtjrqruugj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gthghygdrh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nanxuanxn.top/gtlkglwmne.html

C#:   1234567.ToString("N0")
来源：http://hz.c1oappe.top/gthditxxqe.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtplrwkfep.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtiuddohtl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtoosmbsrc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtdscgeowr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtbbjlzzll.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xingfuxueyuan.xyz/gtkoeradvx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hnqzz.top/gtothypxrx.html

Ruby: s.capitalize
来源：http://hz.yangfankeji.com/gttnbofslx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hnxiangtu.top/gtesfhvwfz.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtjhaiwhra.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.nanxinkj.top/gtnhwovomg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtrrhhzpxi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnqzz.top/gtcpkmhgup.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ivvv.top/gtksxcescj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangdashe.top/gtodbquidi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtqgnlehxp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.guowangkeji.top/gtaeqsawwu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhixingplan.top/gtlgpogtsz.html

[E19] 多行文本按行拆分
来源：http://hz.bjfxy.top/gtnrifpqgg.html

Py:   s.splitlines()
来源：http://hz.kuanghao11.cn/gtjpscufzv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtmwtpuzvy.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj202588.top/gthainnmcc.html

TS:   s.split(/\r?\n/)
来源：http://hz.0kj1m.cn/gtlcofduhr.html

Java: s.lines().toList()
来源：http://hz.sufxvd.cn/gtqakxjdhn.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtteuissox.html

Ruby: s.lines
来源：http://hz.zycfv.cn/gtwmjpfetd.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtoorgtyjx.html

[E20] 判断字符串是否为空
来源：http://hz.zycfv.cn/gtpermqhis.html

Py:   if not s:
来源：http://hz.iojbl.cn/gtzwgbklmf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.smart0.xyz/gtirmqmcnp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtwlulovms.html

TS:   if (s === "") {}
来源：http://hz.fzhhl.top/gteuhjmxkr.html

Java: if (s.isEmpty()) {}
来源：http://hz.meibo888.top/gtpkwrfcyh.html

Go:   if s == "" {}
来源：http://hz.daria6918.cn/gtdsmyzmkk.html

Ruby: if s.empty?
来源：http://hz.ywan-chungtsiang.top/gtjixggssz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenjidiqi.icu/gtnkmayhir.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gtwiqfppop.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shuidangran.top/gtbthadayv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhaomingkeji.xyz/gtzjtpxbmd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtuvmgigaf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtdsaqxwkg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtbvwvkrmc.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xinyue.icu/gtimczixrf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenjidiqi.icu/gtaypcganj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.0kj1m.cn/gtkdtacvrc.html

[E22] 字节长度与字符长度
来源：http://hz.cheryme.top/gtcsdwximv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nanxinkj.top/gtbvaieoxm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtrrrnvxgn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtmhfvtnhr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xylfe.cn/gtbhyosabf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gtwrmjrdij.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.dianchejie.cn/gtniwvosjd.html

Ruby: s.bytesize;  s.length
来源：http://hz.yueranfly.top/gtwmfyhxwk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shzxlz.cn/gtuqjlcqhl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtkpoudakm.html

F. 文件与目录
来源：http://hz.yuxming.cn/gtjqijoseg.html

================================================================================
来源：http://hz.xuanzx.com/gtgujetsft.html

[F01] 读取整个文件
来源：http://hz.ybcxt.top/gtzwlfxnaj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtfbcfbahl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zdqjudy.top/gtpqimhlrp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gogol.net.cn/gtjmdjclnc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daxiang520.top/gtdxlipgye.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtlvpyspig.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guannengcc.top/gtlmicodgf.html

Ruby: File.read("a.txt")
来源：http://hz.chenlongwang.top/gtypawibfm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtuoydlqjd.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtfmhtvpsy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.xinyue.icu/gtadoojsmb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtzjijdgxw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtrbriqtvs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxinkj.top/gtwjqmnxsv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtneqndhch.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtahgygxju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtdgouojtc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtxxcsluzk.html

[F03] 写入文件（覆盖）
来源：http://hz.xylfe.cn/gtusxatfsi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gtephiewtf.html


<!-- 参考信息 -->