代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtwozosaka.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtelyyltiu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.daxiang520.top/gthexjdscx.html

Go:   // 手写循环累加
来源：http://hz.hongshengwenyu.top/gtvtmojlmo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sweek.top/gtimgzxxfm.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinyuanbaomall.cn/gtzuqpqocr.html

[D17] 最大值与最小值
来源：http://hz.yanxiufei.cn/gtbymfxzch.html

Py:   max(arr);  min(arr)
来源：http://hz.cucudq.cn/gtimdzachj.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtqnftggpn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtlexrszot.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gtmhhumatx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xylfe.cn/gtfivpgqtb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenlongwang.top/gtbzblpgeu.html

Ruby: arr.max;  arr.min
来源：http://hz.aizwys.cn/gtdaldjzeu.html

C#:   list.Max();  list.Min()
来源：http://hz.daxiang520.top/gtlsfaacop.html

[D18] 扁平化嵌套数组
来源：http://hz.sxryk.cn/gtifxtlwod.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aizwys.cn/gtufgmzqmw.html

PHP:  array_merge(...$nested);
来源：http://hz.ywan-chungtsiang.top/gtdbjhnloh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtiiatyfbi.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtbptqewsh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhijiandao.cn/gtsjfnwllk.html

Go:   // 手写双层循环
来源：http://hz.jinghuilouyu.cn/gtvsrnvxne.html

Ruby: nested.flatten
来源：http://hz.yj202588.top/gtctysusvw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtvstecrya.html

[D19] 按字段分组
来源：http://hz.ywan-chungtsiang.top/gtoxsuhaqe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtaivyrgln.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhijiandao.cn/gtmkcozrid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtqemzflzz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.andypj.xyz/gtfpemduem.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.vqdsnc.cn/gtsdjgjthm.html

Go:   // 手写 map[string][]T
来源：http://hz.birdmap.top/gtyrcrhqbu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yanxiufei.cn/gtmjiykrgz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.redwolf501.top/gtqsvjuolq.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtycxxaafx.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtllvhpcyn.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtoompsyfs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yonumen.top/gtmzgckwnm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gtzypldpti.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtcciscglo.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtjhbmcvrg.html

Ruby: arr.tally
来源：http://hz.chenzaomai.com/gtpfiobbrj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cqqwz.cn/gtlncryvzk.html

[D21] 判断是否包含某元素
来源：http://hz.daxiang520.top/gtvvuobnlh.html

Py:   x in arr
来源：http://hz.xuetiantiany.cn/gtygeyotpp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ppjwa.cn/gttihwnocp.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtxftpbzmg.html

TS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtvvmlqfkt.html

Java: list.contains(x)
来源：http://hz.jiagoushi.top/gtemzwlthm.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtklfjmqjs.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtztsbszxr.html

C#:   list.Contains(x)
来源：http://hz.jlsjyb.cn/gtvrobalmt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnqzz.top/gtftqzuyia.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.daria6918.cn/gtsbvjfzcs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.quarkkingdee.top/gtfkylmqpu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yangfankeji.com/gtiwazkeqc.html

TS:   [...arr];
来源：http://hz.bjfxy.top/gtfvnyugev.html

Java: new ArrayList<>(list);
来源：http://hz.ivvv.top/gtdtutahjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.vqdsnc.cn/gtbvkmsehp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtgjxkuqlc.html

C#:   new List<int>(list);
来源：http://hz.andypj.xyz/gtfqfzjxfv.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtsogbfpqk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtnhpzehaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.bjfxy.top/gtyddwrvki.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtncwmmevj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtmftfhndz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hongshengwenyu.top/gttjlontba.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtixtauzqp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yvedp.cn/gtfepcmgnh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenjidiqi.icu/gtvexvkdbd.html

[D24] 字典 / Map 基本操作
来源：http://hz.gzhubu.top/gtsyanvcqv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jiagoushi.top/gtqieetdko.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gthymwwyvq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.vqdsnc.cn/gtmxbofvno.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aibaodan.cn/gthodwqouy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258888.top/gtdozyhajd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.wangshuangyany.cn/gtiahbibop.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ivvv.top/gttalhyejn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.9152youxi.cn/gtvkqcpzcz.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtdlzdzytn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtiojoormu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zycfv.cn/gtvmpmxhrp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhaomingkeji.xyz/gtbrcosrtn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydzc1.top/gthezjbbjp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtqohusdvl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtzyfjnbqd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtbjkozqfn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.vqdsnc.cn/gtmiwxifwa.html

[D26] 数组转字符串
来源：http://hz.chenjidiqi.icu/gtcvzrhxmh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtmlwijcdu.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtscawdlzc.html

JS:   arr.join(", ")
来源：http://hz.shuidangran.top/gthhsccari.html

TS:   arr.join(", ")
来源：http://hz.ivvv.top/gtfviswqgz.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtnumtmqxa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aibaodan.cn/gtollxfvjx.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtauvwujsi.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gteicseqdb.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtravqiqgl.html

E. 字符串处理
来源：http://hz.haohaochexian.top/gtukzfqdzl.html

================================================================================
来源：http://hz.316326.xyz/gtuyakkssh.html

[E01] 拼接字符串
来源：http://hz.ydjk.org.cn/gtsmglkxxp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yvedp.cn/gttrkeyadp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtbemrvbfg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtmepllhie.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtqnhqgtax.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtoywgwoyd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.birdmap.top/gtyjquidht.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gtlvpugmyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.dashuyun.cn/gtxjpefjsa.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtugbainwa.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtnbucthke.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtmlmgwjgv.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtoicrgsxa.html

TS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtagkfukhn.html

Java: "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtqvztcase.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gtwljrtzaj.html

Ruby: "ab" * 3
来源：http://hz.zhixingplan.top/gtnqshxcsv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gtijjannan.html

[E03] 截取子串
来源：http://hz.ivvv.top/gtkezpcgzg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtoulbpvvw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtucmfvhwy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.fzhhl.top/gttzzieori.html

TS:   s.slice(1, 4)
来源：http://hz.ppjwa.cn/gtwuswvvap.html

Java: s.substring(1, 4)
来源：http://hz.yj20258888.top/gtwptidbvg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.iojbl.cn/gtekgjduei.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hongshengwenyu.top/gtonbwnzna.html

C#:   s.Substring(1, 3)
来源：http://hz.tian-w.cn/gttbqjzkdd.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtzfzthjwv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ybcxt.top/gtsmrchqyu.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtlwidmbzb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhixingplan.top/gtyrddpetd.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtrtyhgycz.html

Java: s.indexOf("x")
来源：http://hz.yvedp.cn/gtomebjgrj.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtmmadqyuu.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtdhcuygbm.html

C#:   s.IndexOf("x")
来源：http://hz.ivvv.top/gtgsxouvwh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.havefunace.top/gtjvxwtldv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtbxfzgacz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinyuanbaomall.cn/gtuuyihcun.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sysykeji.top/gtgwumrfes.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gthusiwsyf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtejpeojcj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nanxinkj.top/gtfjosduwk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daxiang520.top/gtobbzchzw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtqckgdlnp.html

[E06] 替换子串
来源：http://hz.xylfe.cn/gtepydpgvn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtxfqcbabe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gotoacloud.top/gtcnndytvw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtxqremuca.html

TS:   s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtrdwckzeb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gttccvaerw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gotoacloud.top/gtozzowvot.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xylfe.cn/gtkeohdsox.html

C#:   s.Replace("a", "b")
来源：http://hz.ppjwa.cn/gtjhxkbfwg.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtnxsxfohz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gtxyuhwmer.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gtmsucenkr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtizuxeubi.html

TS:   s.split(",")
来源：http://hz.sweek.top/gtywyfzhel.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jlsjyb.cn/gthlkihgal.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gttlhrzmhr.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtuuwobqil.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtplbudknn.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtaydcbwzz.html

Py:   ",".join(items)
来源：http://hz.jinqigufen.top/gttzgenkqj.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtcxeqjstq.html

JS:   items.join(",")
来源：http://hz.yanxiufei.cn/gtmczvfxpt.html

TS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtbopvmxmp.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtzaoppzxu.html

Go:   strings.Join(items, ",")
来源：http://hz.guannengcc.top/gtofhrwtzw.html

Ruby: items.join(",")
来源：http://hz.chenjidiqi.icu/gtbalauwbe.html

C#:   string.Join(",", items)
来源：http://hz.hnqzz.top/gtxlvyeyob.html

[E09] 去除所有空白字符
来源：http://hz.shuidangran.top/gtcxkheogx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.mhx1999.top/gtxnlsvzsi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258888.top/gtykkzcbit.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtgajxshvj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gteetvxrtb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtdgtndbln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dianchejie.cn/gtwfpkhria.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtxirodcxb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangtech.top/gtdocbhnlh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yangfankeji.com/gtsuwflnjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtydinfsfj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtvctpzyfg.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gttlgiguql.html

TS:   "7".padStart(3, "0")
来源：http://hz.pycfn.com/gtafmdwezp.html

Java: String.format("%03d", 7)
来源：http://hz.ivvv.top/gtyqsmjkre.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtsbjpqslw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gotoacloud.top/gtuaikiinw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pycfn.com/gtvxgqguek.html

[E11] 反转字符串
来源：http://hz.yvedp.cn/gtjaprrriz.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtywkkcmng.html

PHP:  strrev($s);
来源：http://hz.smart0.xyz/gtowcvsruc.html

JS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtnkemrdgu.html

TS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtliiznzwb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gttfiknemk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtxzuklvdk.html

Ruby: s.reverse
来源：http://hz.yanxiufei.cn/gtubzxigqj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gttoqaudfb.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtavlrrsvf.html

Py:   s.count("a")
来源：http://hz.xziqi.cn/gtsdgkfadr.html

PHP:  substr_count($s, "a");
来源：http://hz.ivvv.top/gtwstudusl.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gtfirlyfkq.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtdqrmueqq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtvhxxcxfv.html

Go:   strings.Count(s, "a")
来源：http://hz.shangyingyoupin.top/gtlzwukdmx.html

Ruby: s.count("a")
来源：http://hz.ydzc1.top/gtqaontyuz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnxiangtu.top/gtisbjjtod.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtrvmzhmum.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtzjizwlhv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gttvggvfpg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yongpay.top/gtveeruzyv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtudynizbl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnqzz.top/gtebwglkjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gttrhwmwny.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtpgywskhp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.iojbl.cn/gtienlelvx.html

[E14] URL 编码与 Base64
来源：http://hz.nanxuanxn.top/gtczuwkmog.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yanxiufei.cn/gtgxitybwd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenlongwang.top/gtblsjzxrj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nanxinkj.top/gtpxxrqksn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hongshengwenyu.top/gtqqrdhfvy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtmgltgbox.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.haohaochexian.top/gttxwpattx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtkywaztql.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuxming.cn/gtoskpgoyy.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gthmpvqkfb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gaohongyu789.top/gtisfcjfya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ywan-chungtsiang.top/gtdxdocnjz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtlwziipeo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtijvxibxo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jqgfzy.top/gtrlvhvfku.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.aizwys.cn/gteoocbvbf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yangfankeji.com/gtsfmlrogi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gaohongyu789.top/gtzituurfv.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtweoffunk.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtmkeokdhf.html

PHP:  number_format(1234567);
来源：http://hz.cdnleiting.top/gtnywrmqqy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yueranfly.top/gtqqzyjuqw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtdqolnioy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hnqzz.top/gtfmpsmyhk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dashuyun.cn/gtnnhlcxfo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtvwojzhqz.html

C#:   1234567.ToString("N0")
来源：http://hz.zhaomingkeji.xyz/gtiltjaqhr.html

[E17] 首字母大写
来源：http://hz.chenzaomai.com/gtlycmnsgt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yueranfly.top/gtvpfrimfy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtnrmlaykm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gthcruiokj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhongyouzk.top/gtiuqbtbbb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtzgdcfjns.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhongyouzk.top/gtzkplbive.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtxzosmcch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangdashe.top/gtcpnfpupy.html

[E18] 模板占位符替换
来源：http://hz.9152youxi.cn/gtldvewqok.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xziqi.cn/gtluzydhno.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangshuangyany.cn/gthbkeqkfd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.mhx1999.top/gtzhmrupqr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtljduahkk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtqfbqsyyb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtbzlsaapr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.nanxuanxn.top/gtlpqjnocy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtcsvmxizz.html

[E19] 多行文本按行拆分
来源：http://hz.gogol.net.cn/gtdulqmalw.html

Py:   s.splitlines()
来源：http://hz.ppjwa.cn/gtsauwojrf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gotoacloud.top/gtfvmzhgws.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtvayzdoji.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtooytnolo.html

Java: s.lines().toList()
来源：http://hz.havefunace.top/gtaonyruil.html

Go:   strings.Split(s, "\n")
来源：http://hz.cashguo.top/gtkgsidljk.html

Ruby: s.lines
来源：http://hz.wangshuangyany.cn/gtmaxwpcmy.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangkeji.top/gtuasxsluf.html

[E20] 判断字符串是否为空
来源：http://hz.meibo888.top/gtqpmzcrvp.html

Py:   if not s:
来源：http://hz.snrcjt.cn/gtaxccylgp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtzzrxctyp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tanke756.top/gtncztyfll.html

TS:   if (s === "") {}
来源：http://hz.jiagoushi.top/gtxlbwvhiu.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtjgyxipkw.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtbimhtuau.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtqwhugwdh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtomwiqaqb.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtanacwmqi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jqgufenzy.top/gtzywadtks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gttzothilc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtwtdcdppt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtoclerlon.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtmniackov.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dianchejie.cn/gtiwduxgmw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj202588.top/gtbxompdtu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xinyue.icu/gtpfpgwfhe.html

[E22] 字节长度与字符长度
来源：http://hz.chenjidiqi.icu/gtgowcmvhn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gthplekpub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cheryme.top/gthnvekzcr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgfzy.top/gtkntohxyq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.snrcjt.cn/gtuyqkikbe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtgkyfkood.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.gotoacloud.top/gtvgbnmach.html

Ruby: s.bytesize;  s.length
来源：http://hz.daria6918.cn/gtpdhzrmii.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.vqdsnc.cn/gtwrzoeopm.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvozmpvud.html

F. 文件与目录
来源：http://hz.birdmap.top/gtxwbmyvjp.html

================================================================================
来源：http://hz.gogol.net.cn/gtnagwkyqk.html


<!-- 参考信息 -->