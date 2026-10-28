代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.c1oappe.top/gtwyuuvlal.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gthkqtjpsm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtcrmbgscq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gttxrtzwdh.html

[D15] 去重
来源：http://hz.smart0.xyz/gtghyqgoiu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtwequhell.html

PHP:  array_unique($arr);
来源：http://hz.tianlin.xyz/gtjnykygke.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtfowpiftf.html

TS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtoebjrazm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hongshengwenyu.top/gtnskaqxuy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtiltolcqs.html

Ruby: arr.uniq
来源：http://hz.sufxvd.cn/gttqcnozeq.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtbnwgtbxi.html

[D16] 求和与平均值
来源：http://hz.pycfn.com/gtqkhiglnq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtsjjngflw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtamhguskf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtrrkdlrib.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gterlnklyz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yangfankeji.com/gtsbxgncbo.html

Go:   // 手写循环累加
来源：http://hz.ydjk.org.cn/gtmgsvycfx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gttgbqxngb.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtoafguzax.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gtbhruiyql.html

Py:   max(arr);  min(arr)
来源：http://hz.ivvv.top/gtosejjgmm.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhengqikj.top/gtpisgrdel.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenlongwang.top/gtwuzirmek.html

TS:   Math.max(...arr);
来源：http://hz.fzhhl.top/gtguahzxmx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yongpay.top/gtclltjdfu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangshuangyany.cn/gtnadegohd.html

Ruby: arr.max;  arr.min
来源：http://hz.zhijiandao.cn/gtjbkxdajk.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtglcysorw.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gtnwgtorpv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gthzrxdeun.html

PHP:  array_merge(...$nested);
来源：http://hz.dianchejie.cn/gtphveofbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinyuanbaomall.cn/gtmgcbcuwl.html

TS:   nested.flat();
来源：http://hz.hywenlv.cn/gtfhuhsavt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.bjfxy.top/gtmrhetigz.html

Go:   // 手写双层循环
来源：http://hz.sxryk.cn/gtaabmuaou.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gtufywfkfc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhoulong.xyz/gtvowfcxkc.html

[D19] 按字段分组
来源：http://hz.cqqwz.cn/gtbalbzjdo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hywenlv.cn/gtxxhntleo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yvedp.cn/gtjjgcvkre.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gtxvhfofoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gzhubu.top/gtkelrksbf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cheryme.top/gtzelznlih.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gtsmsxajol.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gtsvpsbarc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ivvv.top/gtrhdqukxg.html

[D20] 统计每个元素出现次数
来源：http://hz.xinyue.icu/gtyfqxmsgj.html

Py:   Counter(arr)
来源：http://hz.gogol.net.cn/gtsmyypdpp.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtfqzvdpkf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhixingplan.top/gtrbmxurvc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtgfwoltzl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.quarkkingdee.top/gtgkxqogtn.html

Go:   // 手写 map[T]int
来源：http://hz.zdqjudy.top/gtjsuxnuwg.html

Ruby: arr.tally
来源：http://hz.feifeiyinyue.top/gtisvwdxtt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xziqi.cn/gtvcnqiqqn.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258888.top/gttpzwprhe.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtajtmuerp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daria6918.cn/gtcnzddhxx.html

JS:   arr.includes(x)
来源：http://hz.ydzc1.top/gtntypeppf.html

TS:   arr.includes(x)
来源：http://hz.aizwys.cn/gtnmswopwy.html

Java: list.contains(x)
来源：http://hz.fengsongda.top/gtwzwdfnis.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhijiandao.cn/gtgiyesust.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtweexwosx.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtgnummhfh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gttrkafase.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sysykeji.top/gthpnfxqyw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtuuvzhlbg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtlfcijhuk.html

TS:   [...arr];
来源：http://hz.gaohongyu789.top/gtrsfphkfw.html

Java: new ArrayList<>(list);
来源：http://hz.xziqi.cn/gttlnfredg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.fzhhl.top/gtvgkagcbx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.fengsongda.top/gtjmfudrnw.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gtvgwqwlqt.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gttuepcqdr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.smart0.xyz/gtpvslstjd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtbtygovhh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gthoncnqnm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtytytyriw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtakzhbazl.html

Go:   // 手写循环
来源：http://hz.zhixingplan.top/gtnmaegual.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cdnleiting.top/gtznkymlgl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtghiagflo.html

[D24] 字典 / Map 基本操作
来源：http://hz.cashguo.top/gtlzalfuae.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtyqhpkhpb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.redwolf501.top/gtgmtvshmo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtoixgqcaw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ppjwa.cn/gtpxojlvor.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hammf.cn/gtyibvgxmi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yonumen.top/gtsgcbemfk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangkeji.top/gtpxoezrmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.iojbl.cn/gtclqzuwgx.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigufen.top/gtfowhlfqx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gzhubu.top/gtrzisakbz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.fengsongda.top/gtxaucrgvv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sweek.top/gtwdwwizcp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgufenzy.top/gtodpyfhfp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sysykeji.top/gtzvioldrh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gtyjvbkpco.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenzaomai.com/gtjniouasv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtlzcyynzh.html

[D26] 数组转字符串
来源：http://hz.jqgufenzy.top/gtkazfppdq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fzhhl.top/gtrglrelhu.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtozfbjtdf.html

JS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtsntiefwg.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtgfzoqxxq.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtvutinwnp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgufenzy.top/gtchzcuica.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtkbactvow.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtiuwxfjil.html

================================================================================
来源：http://hz.hnqzz.top/gtdzgwwudb.html

E. 字符串处理
来源：http://hz.pycfn.com/gthcsucjyb.html

================================================================================
来源：http://hz.svipenyu.cn/gtqagkjyvy.html

[E01] 拼接字符串
来源：http://hz.dashuyun.cn/gtqlcwjlvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhoulong.xyz/gtogkpywva.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gtjufeqmoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtbdbvrvdc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtbrropzuy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ehwqpu.com/gttwkdpbxy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtvyqqbojo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.quarkkingdee.top/gticycbsrp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtpqpfgtmf.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gttlhqiyoz.html

Py:   "ab" * 3
来源：http://hz.hammf.cn/gtzoianddk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tian-w.cn/gtehwvitwb.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtvroqwcle.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtbphspozz.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtydiaheef.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.0kj1m.cn/gtlptsuugu.html

Ruby: "ab" * 3
来源：http://hz.hysaishi.cn/gtatyrgldd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtgtiyefhe.html

[E03] 截取子串
来源：http://hz.daxiang520.top/gtsnxrdcpk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aibaodan.cn/gtpgiyfpdz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.daxiang520.top/gtsxqvylwi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtspcpyhih.html

TS:   s.slice(1, 4)
来源：http://hz.ydzc1.top/gtqqifljpx.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtjdvuizam.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sweek.top/gtnhdtmdkv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.svipenyu.cn/gtlpshlnno.html

C#:   s.Substring(1, 3)
来源：http://hz.kuanghao11.cn/gtdvmrrklz.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtakumahez.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtwvceccce.html

PHP:  strpos($s, "x");
来源：http://hz.ehwqpu.com/gtogymrxpk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shuidangran.top/gttsxgecpp.html

TS:   s.indexOf("x")
来源：http://hz.sweek.top/gtcryjgsho.html

Java: s.indexOf("x")
来源：http://hz.52xcode.cn/gtdwrngroe.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gtddgzfcvx.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtsxmquuoc.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtxuzfdzqf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gaohongyu789.top/gtzfolfcew.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenlongwang.top/gtlelsfjbx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cheryme.top/gtzxguijot.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtrfkhvutl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtgsnfgljf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtcpiltrpx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fzhhl.top/gtpfwqhtei.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gogol.net.cn/gtvnfphzjd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pycfn.com/gttkpogidv.html

[E06] 替换子串
来源：http://hz.wangdashe.top/gtmddmlybs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtxlescoci.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gtwmqplpip.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtatklukma.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtblgrhqdc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtjmrknhqd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yonumen.top/gtvvxsqfbo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zdqjudy.top/gtmhlhzuzv.html

C#:   s.Replace("a", "b")
来源：http://hz.xylfe.cn/gtjjtfufvm.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtumsvowtt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtlebvewfz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gttegcafai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hysaishi.cn/gtioilvglb.html

TS:   s.split(",")
来源：http://hz.smart0.xyz/gtbuedqpjs.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.snrcjt.cn/gtpsvlsfox.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhijiandao.cn/gtqgulhhtw.html

Ruby: s.split(",");  s.split
来源：http://hz.vqdsnc.cn/gttsbhhnri.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shuidangran.top/gtndtuaogb.html

[E08] 数组按分隔符合并
来源：http://hz.yuxming.cn/gtvzbynzrk.html

Py:   ",".join(items)
来源：http://hz.cheryme.top/gtpnivojsx.html

PHP:  implode(",", $items);
来源：http://hz.hammf.cn/gtcnrsbhfq.html

JS:   items.join(",")
来源：http://hz.ywan-chungtsiang.top/gtlsvggbpw.html

TS:   items.join(",")
来源：http://hz.jqgfzy.top/gtxqmhenjx.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtessyefxq.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtyhnsiseo.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtedbnktub.html

C#:   string.Join(",", items)
来源：http://hz.hysaishi.cn/gtisjwgleo.html

[E09] 去除所有空白字符
来源：http://hz.ywan-chungtsiang.top/gtjcvytxyg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xinyue.icu/gtjgotphse.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ywan-chungtsiang.top/gtccnwnyrd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hnxiangtu.top/gtbhtkxtxr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sweek.top/gtlusmvnre.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gticqjuuog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtkuqcjjxd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pycfn.com/gtpksumyea.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.iojbl.cn/gtmhbjonzz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj202588.top/gtzjjxyqfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pycfn.com/gtkflxnebj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gtfboqgjda.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258.top/gtbrztupdk.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtyapykixh.html

Java: String.format("%03d", 7)
来源：http://hz.hongshengwenyu.top/gtbitflpaq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daxiang520.top/gterapklqg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtojrufdka.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtaiscerja.html

[E11] 反转字符串
来源：http://hz.ywan-chungtsiang.top/gtbujohaqh.html

Py:   s[::-1]
来源：http://hz.xinyue.icu/gtksypfoow.html

PHP:  strrev($s);
来源：http://hz.zhiwuduotai.top/gtlfimsztu.html

JS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtfrpgitpg.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtmvsuiync.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangtech.top/gtkszeugmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydjk.org.cn/gtaswmrcrw.html

Ruby: s.reverse
来源：http://hz.zhongyouzk.top/gtkkxvgqcp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtmpudtsrx.html

[E12] 统计某字符出现次数
来源：http://hz.yj202588.top/gtbmopbgvk.html

Py:   s.count("a")
来源：http://hz.cucudq.cn/gtbscdlocw.html

PHP:  substr_count($s, "a");
来源：http://hz.xuetiantiany.cn/gtlshstyjb.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtfasladmc.html

TS:   s.split("a").length - 1
来源：http://hz.sxryk.cn/gtszpgfxoj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gtskaggsaf.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtjiqutwhk.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtmhydwsnl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhoulong.xyz/gtgwasvdve.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtplfxyzfd.html

Py:   for ch in s: print(ch)
来源：http://hz.hnxiangtu.top/gtxibmgwpk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj202588.top/gtzuswmeky.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtrtmvughi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtwnaunuyn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtticwwycy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.9152youxi.cn/gtaqucpnvo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtnvysksol.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gthzzmaame.html

[E14] URL 编码与 Base64
来源：http://hz.dianchejie.cn/gtwmhorbvx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.quarkkingdee.top/gttqmwqtjv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gaohongyu789.top/gttkoosdvd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gtzgvjlmfi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhongyouzk.top/gtpfywzwdd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtsrishqmf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hnqzz.top/gthoqjwpcc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xingfuxueyuan.xyz/gtxsjopacx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuanzx.com/gtestjpolb.html

[E15] HTML 转义 / 反转义
来源：http://hz.fengsongda.top/gtirlhmjya.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yueranfly.top/gtatehrlka.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ppjwa.cn/gtqnledegx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gtmgnxojuy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtbhlevnwq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.fengsongda.top/gtiaghqxhn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuanzhike.top/gtamgedjii.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.shuidangran.top/gtaprrfzef.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtpwhgrebz.html

[E16] 数字千分位
来源：http://hz.zhiwuduotai.top/gtxzdldoqa.html

Py:   f"{1234567:,}"
来源：http://hz.daxiang520.top/gtypcgeemf.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtejnzywla.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtypglotnh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtghziblim.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gttywzfoyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtpoamtvve.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sweek.top/gtmpesgrpc.html

C#:   1234567.ToString("N0")
来源：http://hz.nanxuanxn.top/gtqmgsrzla.html

[E17] 首字母大写
来源：http://hz.cheryme.top/gtemuvzxyw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.quarkkingdee.top/gtyjinujva.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.quarkkingdee.top/gtwcaykwqu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtiaaxwjuk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtpoatahju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jyoumei.cn/gtgsrbobhr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtavofjieo.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtykspgvwg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dianchejie.cn/gtsmcxplwe.html

[E18] 模板占位符替换
来源：http://hz.jiagoushi.top/gtgtxvhdxq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtazuzjase.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gaohongyu789.top/gtcmocglzh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtgynuxrnw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.snrcjt.cn/gtpgpujjpp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cdnleiting.top/gtmfvsvuad.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinyuanbaomall.cn/gthmrunflw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.dashuyun.cn/gtcxslgxkm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.vqdsnc.cn/gtnehlgkik.html

[E19] 多行文本按行拆分
来源：http://hz.meibo888.top/gtxilgbwwk.html

Py:   s.splitlines()
来源：http://hz.nwbrower.top/gtqpgsvxxn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gttjafjshh.html

JS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gtjeeendkg.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gtkgykkevc.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtrghmejqk.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtluzrsvos.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtqrdkihjo.html

C#:   s.Split('\n')
来源：http://hz.tianlin.xyz/gtnatimtxv.html

[E20] 判断字符串是否为空
来源：http://hz.jlsjyb.cn/gtzxuvzzvy.html

Py:   if not s:
来源：http://hz.andypj.xyz/gtzanwfevg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xingfuxueyuan.xyz/gtgselhnpr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gtzvlfaxnk.html

TS:   if (s === "") {}
来源：http://hz.yj202588.top/gtsgqjjbpj.html

Java: if (s.isEmpty()) {}
来源：http://hz.jianghu66.top/gtsvhajqoj.html

Go:   if s == "" {}
来源：http://hz.pycfn.com/gtzkasrorv.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtzntljksk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gthcabypll.html

[E21] 超长截断加省略号
来源：http://hz.nwbrower.top/gtzinmjrmm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xylfe.cn/gtcdamsnqo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.c1oappe.top/gtwisojdee.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtybepicqr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtrneoxanq.html


<!-- 参考信息 -->