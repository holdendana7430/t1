代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtuqqwvqfw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtilfgbtvd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gthwowkcdk.html

Go:   // 手写循环累加
来源：http://hz.zhijiandao.cn/gtncycgiji.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtphalascf.html

C#:   list.Sum();  list.Average()
来源：http://hz.svipenyu.cn/gtmpwqhrul.html

[D17] 最大值与最小值
来源：http://hz.fzhhl.top/gtzfascnic.html

Py:   max(arr);  min(arr)
来源：http://hz.ydjk.org.cn/gtkltffnoq.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtfzghbrys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtsbulokyn.html

TS:   Math.max(...arr);
来源：http://hz.jyoumei.cn/gtaxlgwpjr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gthmcalxjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.c1oappe.top/gtmslazelw.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtoebmykut.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtysyqsrbm.html

[D18] 扁平化嵌套数组
来源：http://hz.52xcode.cn/gtqibqbyhz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.iojbl.cn/gttfiqrjag.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtklcehhvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.andypj.xyz/gtfzclujgs.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtuypxogmm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenzaomai.com/gtpnaeybbd.html

Go:   // 手写双层循环
来源：http://hz.chenzaomai.com/gtegzvwfba.html

Ruby: nested.flatten
来源：http://hz.xingfuxueyuan.xyz/gtxcjemele.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.c1oappe.top/gtisffcwkd.html

[D19] 按字段分组
来源：http://hz.xinyue.icu/gtcrialpfp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtohmgbyrn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258888.top/gtukeskxmz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.nanxinkj.top/gtvucfuwtd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cdnleiting.top/gtsclglaso.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtfahhqgra.html

Go:   // 手写 map[string][]T
来源：http://hz.hfpthk.cn/gtneihpxae.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cashguo.top/gtgbolarvs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gthtvubhgv.html

[D20] 统计每个元素出现次数
来源：http://hz.nwbrower.top/gtenuglfdu.html

Py:   Counter(arr)
来源：http://hz.chenlongwang.top/gtbsnheoas.html

PHP:  array_count_values($arr);
来源：http://hz.ywan-chungtsiang.top/gtmllpfkri.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gtfkbvefis.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtnkpfxhtt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydzc1.top/gtrobdopya.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtshizzvka.html

Ruby: arr.tally
来源：http://hz.cdnleiting.top/gtbunvlzrf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtxprcdeou.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtxkxzkcgr.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtebidgifz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj202588.top/gtqhekldvq.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtinwocejk.html

TS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtylaznxyf.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtwfumytex.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtxmequfmy.html

Ruby: arr.include?(x)
来源：http://hz.jinyuanbaomall.cn/gtfdvwlapq.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtvjazcotd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtmgrkelyg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtissyopyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gteziwwiyy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenjidiqi.icu/gtignhycls.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtqefgixbm.html

Java: new ArrayList<>(list);
来源：http://hz.yonumen.top/gtsefrpref.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guannengcc.top/gtkvvibdfg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.svipenyu.cn/gtqywplehj.html

C#:   new List<int>(list);
来源：http://hz.snrcjt.cn/gtmwlszniv.html

[D23] reduce 累积计算
来源：http://hz.cdnleiting.top/gtxbuoiywo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtwixsevnn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtruilvekp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtjbdyoyfy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtodfedwyn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.kuanghao11.cn/gttihjnnjn.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtazfqnvig.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnxiangtu.top/gtcyqywpeb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtnjaazlan.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtqswtyplq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtrwmdqibu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gogol.net.cn/gtvnymyxaj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.kuanghao11.cn/gtjtdsbrui.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jiagoushi.top/gtiuyinonu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhongyouzk.top/gtoqkpprwv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gthlksutzz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.feifeiyinyue.top/gtolhpksrd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgufenzy.top/gtzlzbdvvh.html

[D25] Set 集合去重与交并差
来源：http://hz.cashguo.top/gtephxgwru.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.redwolf501.top/gtmwfpdddo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj202588.top/gtzhgkhimh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cdnleiting.top/gttqepjudv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.svipenyu.cn/gtdlwbkrcs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtkkqpdfgg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xylfe.cn/gtbwqybysb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gthqkbyubk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtvxswnqlr.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtmcneyisw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtbpepdhsc.html

PHP:  implode(", ", $arr);
来源：http://hz.fzhhl.top/gtcqrbuisb.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtpmervjpv.html

TS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtllvczwve.html

Java: String.join(", ", list)
来源：http://hz.jinqigufen.top/gtcknvmkno.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtewkpogqa.html

Ruby: arr.join(", ")
来源：http://hz.zdqjudy.top/gtdsgehira.html

C#:   string.Join(", ", list)
来源：http://hz.zhoulong.xyz/gtairbtiga.html

================================================================================
来源：http://hz.sufxvd.cn/gtkeosxdql.html

E. 字符串处理
来源：http://hz.zhengqikj.top/gtvdvevuvc.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtadizzjjf.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtdoihrjpv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtzsrkwzii.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtotcnomld.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yvedp.cn/gtlckobmrp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtmzssbtkf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gthhcxjftg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.haohaochexian.top/gtovdggcnv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtnksiagzf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtgjcgiujs.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtdmennloo.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtvxkydpzz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenzaomai.com/gtpowlgtcs.html

JS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gtgbvmbeyk.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtygxgmfsx.html

Java: "ab".repeat(3)
来源：http://hz.hywenlv.cn/gtjcwtcbxy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtmjnfcarq.html

Ruby: "ab" * 3
来源：http://hz.yvedp.cn/gtqrocujqa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gtmusnfivp.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtupbffxdc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tanke756.top/gtumjtgaaf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daria6918.cn/gttyunggzp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gtmzftbvnw.html

TS:   s.slice(1, 4)
来源：http://hz.kuanghao11.cn/gtggbjtwpq.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtanygzoru.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtwusujjxb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guowangkeji.top/gthwdeseme.html

C#:   s.Substring(1, 3)
来源：http://hz.shzxlz.cn/gttzzmkmqw.html

[E04] 查找子串位置
来源：http://hz.ppjwa.cn/gtzgrvjfkg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtbkyethcx.html

PHP:  strpos($s, "x");
来源：http://hz.zdqjudy.top/gtmknkhhxf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.tanke756.top/gtkvusosrq.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gtvmvjtsxz.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtgqdknlca.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtaqyxoqzu.html

Ruby: s.index("x")
来源：http://hz.jinqigufen.top/gtbovokvvb.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtthmyzefa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtuaahgkes.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ywan-chungtsiang.top/gtwmoqhgqz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtlxahrnmk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtzryawnap.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yanxiufei.cn/gtszssvdnk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258.top/gthfezoqta.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jiagoushi.top/gtymzhyscv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gaohongyu789.top/gtztirvtyd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gteatccfsp.html

[E06] 替换子串
来源：http://hz.fzhhl.top/gtpaokcete.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.bjfxy.top/gtbzrqktsu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hammf.cn/gtktoiaqgc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ydjk.org.cn/gtiuunchuq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.52xcode.cn/gttzskbdfq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jianghu66.top/gtlaapnatx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jlsjyb.cn/gttevhlhsv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gttesqqtls.html

C#:   s.Replace("a", "b")
来源：http://hz.gogol.net.cn/gtqhgsyrrc.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtsbuatbjt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.c1oappe.top/gtovxkebcx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yvedp.cn/gtuzzhtnyn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gtznnojanq.html

TS:   s.split(",")
来源：http://hz.zhiwuduotai.top/gtdfjwcjia.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cqqwz.cn/gtovwotvey.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ivvv.top/gtcwtctdji.html

Ruby: s.split(",");  s.split
来源：http://hz.ydjk.org.cn/gtifgvkkiw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtvmfahbvf.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtmmfnikxg.html

Py:   ",".join(items)
来源：http://hz.zhiwuduotai.top/gtcnmfmepr.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gthpuxlbfn.html

JS:   items.join(",")
来源：http://hz.yongpay.top/gtyyqkbbzj.html

TS:   items.join(",")
来源：http://hz.cqqwz.cn/gtpddgfzyr.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtuozfofcj.html

Go:   strings.Join(items, ",")
来源：http://hz.zhoulong.xyz/gtpspzfvlh.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtuptltckg.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtratqyhay.html

[E09] 去除所有空白字符
来源：http://hz.gaohongyu789.top/gtkgpycfjo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenzaomai.com/gtjocaoqda.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtqadwqbqz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtabygvjbo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtahryegbt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtzctqcrql.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtqhdqqfar.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gtijplkzib.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhoulong.xyz/gtnjcmvufu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ehwqpu.com/gtmcxbqxcb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxinkj.top/gtpeasadik.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtxswatjob.html

JS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtyhusylcn.html

TS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtmoybxzsf.html

Java: String.format("%03d", 7)
来源：http://hz.zdqjudy.top/gtexlryowh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtbccieuon.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aizwys.cn/gtmuwpbiff.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xingfuxueyuan.xyz/gtqzfxoest.html

[E11] 反转字符串
来源：http://hz.zhoulong.xyz/gtmokvovex.html

Py:   s[::-1]
来源：http://hz.pycfn.com/gtgejgloik.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gtkjdprktv.html

JS:   [...s].reverse().join("")
来源：http://hz.ydzc1.top/gtffpxylnf.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtzdpzohxs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guowangkeji.top/gtaudqcisj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.andypj.xyz/gtvdnjvrua.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtbjatvkwd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hfpthk.cn/gtihwemsap.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtzqeoolbe.html

Py:   s.count("a")
来源：http://hz.316326.xyz/gtihhcejvi.html

PHP:  substr_count($s, "a");
来源：http://hz.c1oappe.top/gtradxizhb.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtrueqzlzs.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtsvsawdjn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zycfv.cn/gtzfwtgjes.html

Go:   strings.Count(s, "a")
来源：http://hz.dashuyun.cn/gtdbeletgp.html

Ruby: s.count("a")
来源：http://hz.cdnleiting.top/gtfuhkorxv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gtxubfxkob.html

[E13] 逐字符遍历
来源：http://hz.chenzaomai.com/gtdrtzacqp.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtgqvhmnmx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtmmvhkwpe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtkvrulbxy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gttpqlqytm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gogol.net.cn/gtpeyihjli.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ivvv.top/gttrveecnn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.mhx1999.top/gtqnjirvzu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhiwuduotai.top/gtnlbwhxjk.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gttivdlxaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtpnwyaatf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jyoumei.cn/gtxxpjoofv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gtoedmpqre.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtrlghtdxd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.bjfxy.top/gtlczbtwlq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guowangkeji.top/gtcwfjqivd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tian-w.cn/gtwzijvemx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtbhdaonvl.html

[E15] HTML 转义 / 反转义
来源：http://hz.cqqwz.cn/gthdfgymma.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tian-w.cn/gtgzaakhsq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtquwzuquf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.smart0.xyz/gtmggmhblk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ppjwa.cn/gtrijmsngx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fzhhl.top/gtwanofmlo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtvtzrogxq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dashuyun.cn/gtjjijldwt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtyfjqzyrt.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtjcqxbabl.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gthgcakpyk.html

PHP:  number_format(1234567);
来源：http://hz.cqqwz.cn/gtsevvredb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtaidyqsmx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtabfzorat.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.vqdsnc.cn/gtfhlssbxv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtopggqxfd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dashuyun.cn/gtxprnxgfg.html

C#:   1234567.ToString("N0")
来源：http://hz.svipenyu.cn/gteymnjbug.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gtpwfhojfa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtdyzxvyee.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtuevtzbgf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinyuanbaomall.cn/gtpqivcdpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gtxlkbmlnp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gthqwkwhgf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangdashe.top/gtaxisfykj.html

Ruby: s.capitalize
来源：http://hz.zhijiandao.cn/gtxuaoftwf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xziqi.cn/gtnteqhqlv.html

[E18] 模板占位符替换
来源：http://hz.meibo888.top/gtbvaqripv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.birdmap.top/gtvhdlhecg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yueranfly.top/gtqbevvdsr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtkocjvhjh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtnmylkmrd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtwdsadibn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hnqzz.top/gtazduchba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.feifeiyinyue.top/gtozdwqhlb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtjujsrlzp.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258.top/gtjvuanzvc.html

Py:   s.splitlines()
来源：http://hz.vqdsnc.cn/gtsqbfdxut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtvrfdjbmi.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gteoevnrmq.html

TS:   s.split(/\r?\n/)
来源：http://hz.cucudq.cn/gtxdnueszq.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtvfmkxjyf.html

Go:   strings.Split(s, "\n")
来源：http://hz.bjfxy.top/gtjusvjqgd.html

Ruby: s.lines
来源：http://hz.zhengqikj.top/gtbrwbcxqg.html

C#:   s.Split('\n')
来源：http://hz.ywan-chungtsiang.top/gtyzcnsnnl.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtvwlwkagc.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtelbubcyp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258.top/gtyhpwsixf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gtegmxbmpt.html

TS:   if (s === "") {}
来源：http://hz.snrcjt.cn/gtjfdtdrez.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gtxtwijgdp.html

Go:   if s == "" {}
来源：http://hz.nanxinkj.top/gtzcawilak.html

Ruby: if s.empty?
来源：http://hz.shuidangran.top/gtocvhrkmc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigfzy.top/gtjgxxyooa.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gtebtaqopp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.hammf.cn/gtfznhcusd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtjtiskrwk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtpjuxhpsv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.andypj.xyz/gtgnbpxjqu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtpsgboauu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yvedp.cn/gtciolhlzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtqsdeyetn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gaohongyu789.top/gtfuhftiye.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtmgafzmke.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guannengcc.top/gtmggvzvlb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtwkvxqknh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtmvzvbghn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuetiantiany.cn/gtaxnmxdui.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtdlhyyucy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtwtymwgdf.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtqzifadjc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ivvv.top/gtuzjeqbfw.html

================================================================================
来源：http://hz.meibo888.top/gtmvgltgtm.html

F. 文件与目录
来源：http://hz.andypj.xyz/gtlbmvxwvv.html

================================================================================
来源：http://hz.havefunace.top/gtyoywixzb.html


<!-- 参考信息 -->