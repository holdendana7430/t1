代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtisqithbz.html

Ruby: arr.max;  arr.min
来源：http://hz.zycfv.cn/gtburtcnlm.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gtprbmgsxm.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtokidkmat.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtecoekeyb.html

PHP:  array_merge(...$nested);
来源：http://hz.svipenyu.cn/gteesxcdad.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dashuyun.cn/gtwbvubehl.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gttkqvytbv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtqrourfrq.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gtyhxpsjao.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtwlmhrfvq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtctwbspco.html

[D19] 按字段分组
来源：http://hz.pengpengdd.cyou/gtvcvposnh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtcpovlsqi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtshhgyyfz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yuxming.cn/gtljyukcku.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtxmmjlelk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cashguo.top/gtwpjjdfez.html

Go:   // 手写 map[string][]T
来源：http://hz.xinyue.icu/gtudklhrvc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dianchejie.cn/gtzbugwczz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhoulong.xyz/gtsjqaabqf.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtewocpbid.html

Py:   Counter(arr)
来源：http://hz.jinyuanbaomall.cn/gtseaeabue.html

PHP:  array_count_values($arr);
来源：http://hz.yvedp.cn/gthfmtlcce.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ywan-chungtsiang.top/gtruoarnul.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shzxlz.cn/gtxtrfgkpn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tanke756.top/gtcubyuklw.html

Go:   // 手写 map[T]int
来源：http://hz.tianlin.xyz/gturlgyqvg.html

Ruby: arr.tally
来源：http://hz.gaohongyu789.top/gtbyhorcbl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtjcarnnxm.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtwhxhgdku.html

Py:   x in arr
来源：http://hz.redwolf501.top/gtwgvweous.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtdfbnnjpg.html

JS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtdfxdckqe.html

TS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gttpxzgwtv.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtqznzxgvy.html

Go:   slices.Contains(arr, x)
来源：http://hz.dashuyun.cn/gthvqwflxm.html

Ruby: arr.include?(x)
来源：http://hz.ybcxt.top/gtwqonoljp.html

C#:   list.Contains(x)
来源：http://hz.tianlin.xyz/gtphkhlwvs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtqxrrcsje.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cdnleiting.top/gtxkhxpfeu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xylfe.cn/gtobvbwrin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shzxlz.cn/gthpcelmwj.html

TS:   [...arr];
来源：http://hz.jlsjyb.cn/gtuefayzin.html

Java: new ArrayList<>(list);
来源：http://hz.yangfankeji.com/gtulgengbj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtutfntrtg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtocsweoyf.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtlhptieff.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtfkqdcogr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtbqvstygj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.haohaochexian.top/gtzqrdbhxg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gtysmajnty.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tanke756.top/gtoqnitylt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtoixdqfum.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gtcywbcrqr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aibaodan.cn/gtkmfhmwei.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtkydizgxu.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtbowurtga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhijiandao.cn/gtoskclybb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhiwuduotai.top/gtasioayte.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtxowerbrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtofwstqzs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtwljlfmin.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtredkaagq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtmnpdwokk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenzaomai.com/gtdbvbqvxf.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtprsqgvja.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ppjwa.cn/gtzqzfyftm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtifztxwaz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtifokrrzr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gtyoxdxcxk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hnxiangtu.top/gtyexsgxiz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sysykeji.top/gtasuupthm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtjipumhyn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtdjdmoshg.html

[D26] 数组转字符串
来源：http://hz.c1oappe.top/gtsfuxuysc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.daxiang520.top/gtjahjmers.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gttnegcfzr.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtboikeoxl.html

TS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gthughxxgp.html

Java: String.join(", ", list)
来源：http://hz.vqdsnc.cn/gtdvpjcrdf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtvzcbturz.html

Ruby: arr.join(", ")
来源：http://hz.aizwys.cn/gtrhunarom.html

C#:   string.Join(", ", list)
来源：http://hz.shuidangran.top/gtvpviwwpe.html

================================================================================
来源：http://hz.yueranfly.top/gthdznrqeb.html

E. 字符串处理
来源：http://hz.chenlongwang.top/gtuusnyuil.html

================================================================================
来源：http://hz.0kj1m.cn/gthghjxxyk.html

[E01] 拼接字符串
来源：http://hz.haohaochexian.top/gttaifsjat.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnxiangtu.top/gtrwglmszt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hongshengwenyu.top/gtfnjkabel.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.quarkkingdee.top/gtccjxgrcx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtgvwomlyd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fengsongda.top/gtmoyqgknc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gthqlcislv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtfmjlhxmq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.dashuyun.cn/gtthktrdto.html

[E02] 重复字符串
来源：http://hz.guannengcc.top/gtwtxryuoo.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtzbrdlbqi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gzhubu.top/gtkdavndyz.html

JS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gtlgunfmbj.html

TS:   "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtsgaykzep.html

Java: "ab".repeat(3)
来源：http://hz.ehwqpu.com/gthvekktul.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.iojbl.cn/gtsyfqbtsq.html

Ruby: "ab" * 3
来源：http://hz.yj202588.top/gtphjojzgw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gtcvyuhyek.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtjiooyobe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtqartqncp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shuidangran.top/gtgwvpohhh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cucudq.cn/gtgqpqwbha.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtvmqnbram.html

Java: s.substring(1, 4)
来源：http://hz.jlsjyb.cn/gtdaappgvl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cheryme.top/gtgtpajygp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aizwys.cn/gtxmmcqjwc.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtcajdntlu.html

[E04] 查找子串位置
来源：http://hz.yj202588.top/gtxwnpofja.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xziqi.cn/gtjnmxumle.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtafaacfce.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sweek.top/gttsngylpy.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gtvyauvsxl.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gtopvnyrvv.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtifgpojpl.html

Ruby: s.index("x")
来源：http://hz.guowangkeji.top/gtyecthlvb.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangtech.top/gtqvpdaakp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.andypj.xyz/gtrthkhfui.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtrawmoyhe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtnzxliwhf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtiivxpdeb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.tianlin.xyz/gthgpfiaiz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtnbzzcfxi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.iojbl.cn/gtbtgryxid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgfzy.top/gtxiyuugqi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cashguo.top/gtfgryhvxh.html

[E06] 替换子串
来源：http://hz.guowangkeji.top/gtiamptnnm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtvyqhbwmm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gtpqrfmmst.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gttginuqhx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtsxgsqmfh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtjskuajvz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtpeokuwpr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yueranfly.top/gtwzuudaky.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtcaeutdwc.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtaujwtile.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shanyushiyangkeji.top/gtlyjscadq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gthcbwfoyt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtirpnsaaj.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtshvpqwrw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gtfbfzqmyg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtisgucvwk.html

Ruby: s.split(",");  s.split
来源：http://hz.xuanzx.com/gtuwhfvden.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cucudq.cn/gtayhlsatd.html

[E08] 数组按分隔符合并
来源：http://hz.cashguo.top/gtkxjojxbl.html

Py:   ",".join(items)
来源：http://hz.chenjidiqi.icu/gtxziwgasz.html

PHP:  implode(",", $items);
来源：http://hz.yanxiufei.cn/gttihqdnrn.html

JS:   items.join(",")
来源：http://hz.smart0.xyz/gtcrwugteu.html

TS:   items.join(",")
来源：http://hz.yanxiufei.cn/gttjoilwko.html

Java: String.join(",", items)
来源：http://hz.yj20258.top/gtheskxchw.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gthqmxkvwm.html

Ruby: items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtpaxqxyxm.html

C#:   string.Join(",", items)
来源：http://hz.sysykeji.top/gtpzjscrrb.html

[E09] 去除所有空白字符
来源：http://hz.yongpay.top/gtbhqdhpjw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtywvsdmcz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.meibo888.top/gtprhhtish.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtcwfkbjqo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhengqikj.top/gtknovfioz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj202588.top/gtetbzttvi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yueranfly.top/gtnapmtmsi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.guannengcc.top/gtpecrjzda.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shzxlz.cn/gtflkgykya.html

[E10] 左侧补零 / 定长填充
来源：http://hz.meibo888.top/gtpeprzczi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtajnjgwcl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.daria6918.cn/gtuescruux.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gthifvcymr.html

TS:   "7".padStart(3, "0")
来源：http://hz.birdmap.top/gtqfbacgpi.html

Java: String.format("%03d", 7)
来源：http://hz.nanxuanxn.top/gtkdjmhtkh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cqqwz.cn/gteyhmwmxa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtvcwurofw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gtdncrkccl.html

[E11] 反转字符串
来源：http://hz.shanyushiyangkeji.top/gtidhfyhmm.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtcwcqoizd.html

PHP:  strrev($s);
来源：http://hz.hysaishi.cn/gteyxftumx.html

JS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtkkzqmozf.html

TS:   [...s].reverse().join("")
来源：http://hz.pycfn.com/gtlyixmjsh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhiwuduotai.top/gtnrpsmhvt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ywan-chungtsiang.top/gtbqftkdmv.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gtpchmusny.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtwvbbhdrs.html

[E12] 统计某字符出现次数
来源：http://hz.cucudq.cn/gtigtnfrwb.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtbvarjsfl.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtesogfxbu.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtewpoxhlc.html

TS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtbgzpyrmy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tian-w.cn/gtdwywdeqh.html

Go:   strings.Count(s, "a")
来源：http://hz.daxiang520.top/gtakggylcb.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtagnqlmlo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhoulong.xyz/gtsjsiseom.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtdjfkjpmd.html

Py:   for ch in s: print(ch)
来源：http://hz.quarkkingdee.top/gtzcrlrcbr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hammf.cn/gtcfiamdjv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtwdklihpw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtbowgodzf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yuanzhike.top/gtdsiwuqxp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nwbrower.top/gttyeepegv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtznabrbsm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nwbrower.top/gtgemxbmbg.html

[E14] URL 编码与 Base64
来源：http://hz.ehwqpu.com/gttohpvcbj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gtzhxinowv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jianghu66.top/gtxbqhvfmu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jiagoushi.top/gtqzjpwwtp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gtqdgkycks.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.svipenyu.cn/gtemjqiqvx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtfemiukrg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtqsyxotvy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xinyue.icu/gtzjsanggc.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtcwngivsa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.havefunace.top/gtrzozlfmx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuetiantiany.cn/gtfrjnbzus.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yj20258.top/gtillxlwjy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shuidangran.top/gtqjeakxqw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtdvqznyfm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.tanke756.top/gtwhmzecri.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtfiwtfihj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yonumen.top/gtrtfufsym.html

[E16] 数字千分位
来源：http://hz.yongpay.top/gtjirchbxk.html

Py:   f"{1234567:,}"
来源：http://hz.zdqjudy.top/gtngzafuex.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gthpimerzb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtgpcitrrj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtrfcnzbww.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pycfn.com/gtvcpjrsje.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jiagoushi.top/gtfojmrpdx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtenfjmvut.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtzizmitlt.html

[E17] 首字母大写
来源：http://hz.yj20258888.top/gtexkzxxqq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.cqqwz.cn/gtrghllmgl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtonqzkfhm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtbonmtyct.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtwdtqhooo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenjidiqi.icu/gtqozbdtdo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtrwgbesee.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtwubkjtgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guowangkeji.top/gtzqolqbbb.html

[E18] 模板占位符替换
来源：http://hz.jinyuanbaomall.cn/gtvligfcqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gotoacloud.top/gtoywizlie.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ywan-chungtsiang.top/gtkqiahfdh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtsvqtpldc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtffxkcvlk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.guannengcc.top/gtuyfkwiep.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtxpspksme.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtxdtdvidy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtjflykwhz.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtnernasuh.html

Py:   s.splitlines()
来源：http://hz.jlsjyb.cn/gtkxdfcwfa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.9152youxi.cn/gtdsgbhapo.html

JS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtgrulqkbb.html

TS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gthblcwuee.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gteojvhcos.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtfbeplvik.html

Ruby: s.lines
来源：http://hz.sweek.top/gtirkfmzqa.html

C#:   s.Split('\n')
来源：http://hz.cucudq.cn/gtftutebsc.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtbvcwrslm.html

Py:   if not s:
来源：http://hz.cqqwz.cn/gtjocqbxcg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtmhvwmtjh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.fzhhl.top/gtrbcbmqtb.html

TS:   if (s === "") {}
来源：http://hz.52xcode.cn/gtkruzhcgl.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gttwekvmqr.html

Go:   if s == "" {}
来源：http://hz.zhiwuduotai.top/gtzedqopgz.html

Ruby: if s.empty?
来源：http://hz.zhengqikj.top/gtddixhapn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtvngzdbix.html

[E21] 超长截断加省略号
来源：http://hz.jlsjyb.cn/gtqajlrowa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtfgqntksx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shuidangran.top/gtdydkizvv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gtwtnewkme.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtckhspifv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.316326.xyz/gtpjifsdpv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtcttntpbb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.0kj1m.cn/gtqtutrlqe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtnerimsiv.html

[E22] 字节长度与字符长度
来源：http://hz.cheryme.top/gtfwbzgtwd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zhoulong.xyz/gttnprzuzg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtqhmnhbwc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinghuilouyu.cn/gtroxcurdf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hysaishi.cn/gtctebzcnj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtznckiqpv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.aizwys.cn/gtdgsxzxpz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigfzy.top/gtocvthkjk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenjidiqi.icu/gtmqpbvghh.html

================================================================================
来源：http://hz.yueranfly.top/gtpmhcgnmd.html

F. 文件与目录
来源：http://hz.shangyingyoupin.top/gtkozuwgum.html

================================================================================
来源：http://hz.shuidangran.top/gtkdenhggh.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gtavxkhhvf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtxnsoomth.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yonumen.top/gtbvgcrnmo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.havefunace.top/gtcebrdkln.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtfxsqbmlj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtaiocbpql.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.haohaochexian.top/gtxbnrxrsg.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtyyxjewwg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.tianlin.xyz/gtpgpfpujs.html

[F02] 逐行读取文件
来源：http://hz.yonumen.top/gtysmqllip.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yanxiufei.cn/gtvshuizce.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shuidangran.top/gtbrqmzhra.html


<!-- 参考信息 -->