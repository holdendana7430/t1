代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yueranfly.top/gtvmiqbvbm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gttaaflvgr.html

JS:   arr.map(x => x * 2)
来源：http://hz.hnqzz.top/gttpijcrak.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtioimrfwl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yongpay.top/gtntgaxceo.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtmjuwngwg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtzhkgnimw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yueranfly.top/gtzlwpuiom.html

[D15] 去重
来源：http://hz.cdnleiting.top/gtilqpesip.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtahinouou.html

PHP:  array_unique($arr);
来源：http://hz.quarkkingdee.top/gthtidvvfo.html

JS:   [...new Set(arr)]
来源：http://hz.ehwqpu.com/gtgkgiybzp.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtbuoljvjb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gttpbtfrbu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hysaishi.cn/gtqpbopwfp.html

Ruby: arr.uniq
来源：http://hz.hnqzz.top/gtqxqlgdgf.html

C#:   list.Distinct().ToList()
来源：http://hz.hnqzz.top/gtqsgkegem.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtkwpkgwvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtsvtpwcki.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hywenlv.cn/gtysudrerm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gthsjjhtqu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtwbramidl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shuidangran.top/gtqzmfxrxj.html

Go:   // 手写循环累加
来源：http://hz.sufxvd.cn/gtwsdhzerx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yongpay.top/gtnimcsirp.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gteejaqsep.html

[D17] 最大值与最小值
来源：http://hz.c1oappe.top/gtpcvyjoud.html

Py:   max(arr);  min(arr)
来源：http://hz.zdqjudy.top/gtktbwfecc.html

PHP:  max($arr);  min($arr);
来源：http://hz.pengpengdd.cyou/gtkvlgqvwo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangshuangyany.cn/gtqtqilmvx.html

TS:   Math.max(...arr);
来源：http://hz.vqdsnc.cn/gtjajyiohb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yonumen.top/gtdarioojz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtpftxagwq.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtlkgiwzfq.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gteagykslo.html

[D18] 扁平化嵌套数组
来源：http://hz.cucudq.cn/gtxvedvwne.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.snrcjt.cn/gtewavjuhl.html

PHP:  array_merge(...$nested);
来源：http://hz.yangfankeji.com/gtyooaitqe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinyuanbaomall.cn/gturcantth.html

TS:   nested.flat();
来源：http://hz.jianghu66.top/gttgksptxb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangshuangyany.cn/gtfentryvm.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtxlrgvbun.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtuxsfrpxk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gttstxngqm.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gtqortoius.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgfzy.top/gtvgbkiibj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtqcuzeitj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gotoacloud.top/gtahnbrxtn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtzwpjpyvb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ivvv.top/gtfofadvee.html

Go:   // 手写 map[string][]T
来源：http://hz.daxiang520.top/gttchhzgku.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sufxvd.cn/gtwydcyjrb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtxrwfwluf.html

[D20] 统计每个元素出现次数
来源：http://hz.yj202588.top/gtgllbslyn.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtatmcpgkb.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtujzfswqn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtgtunublj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jianghu66.top/gtutuajicj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258.top/gtykgawcyd.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gtyynpgczz.html

Ruby: arr.tally
来源：http://hz.mhx1999.top/gtnurxauah.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtkwderbst.html

[D21] 判断是否包含某元素
来源：http://hz.ppjwa.cn/gtsrhdeaut.html

Py:   x in arr
来源：http://hz.yuanzhike.top/gthhiasltm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.feifeiyinyue.top/gtrxawucdp.html

JS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtylvkpwyt.html

TS:   arr.includes(x)
来源：http://hz.wangdashe.top/gtfhachuyh.html

Java: list.contains(x)
来源：http://hz.shuidangran.top/gtqogyxkmb.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtlpsamqag.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtoxljtlgb.html

C#:   list.Contains(x)
来源：http://hz.chenzaomai.com/gtrdwbbxof.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gtpzobnjah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangshuangyany.cn/gthratgcas.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jianghu66.top/gthfdrywyd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.daria6918.cn/gtzfitdabg.html

TS:   [...arr];
来源：http://hz.zhoulong.xyz/gtfkpnqtjb.html

Java: new ArrayList<>(list);
来源：http://hz.52xcode.cn/gtgylbcdyi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yonumen.top/gtrukwxzqa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cashguo.top/gtprpdkdwv.html

C#:   new List<int>(list);
来源：http://hz.cheryme.top/gtpbybrfsq.html

[D23] reduce 累积计算
来源：http://hz.316326.xyz/gtilozcvfy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtzwzzacqm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtgupwmbby.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gteihnkdcn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtwddqktom.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtvwsbvnfz.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtpqexawtl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtfwjkeivp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtlrevemwy.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtlvyiijgt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtnkqszkkq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangdashe.top/gtetwssqhm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgfzy.top/gtajqhyear.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtajasuvye.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.9152youxi.cn/gtycefvuuc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shangyingyoupin.top/gtkctckahd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gthvqcnbrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sxryk.cn/gtppzrzwvd.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtpfjaciws.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gogol.net.cn/gtgomaqruf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtksornzbb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tanke756.top/gtzbbarvvk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtkmswdaiv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tanke756.top/gtmccykdgj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtomxdezij.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.iojbl.cn/gtxzhuzgkr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.wangdashe.top/gtqazaoudg.html

[D26] 数组转字符串
来源：http://hz.gogol.net.cn/gtzpjhibat.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gzhubu.top/gtjshenyab.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtbbgmrihb.html

JS:   arr.join(", ")
来源：http://hz.birdmap.top/gtqkbtqdje.html

TS:   arr.join(", ")
来源：http://hz.guannengcc.top/gtklkaargo.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtwlogibdk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guannengcc.top/gtrbbexyeh.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtcdnwpooa.html

C#:   string.Join(", ", list)
来源：http://hz.aizwys.cn/gtyavklvdh.html

================================================================================
来源：http://hz.cheryme.top/gtrysgbjwf.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gtlexpwitm.html

================================================================================
来源：http://hz.aibaodan.cn/gtxozmojkr.html

[E01] 拼接字符串
来源：http://hz.pycfn.com/gtcngdiyyi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jyoumei.cn/gtlfbtnwri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pycfn.com/gtjvjyyuiy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gtbranbbly.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gttsqaficg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xylfe.cn/gtwbqpobbe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtubdeajvz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtejteoxcc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hfpthk.cn/gtusrcnfja.html

[E02] 重复字符串
来源：http://hz.cucudq.cn/gtftzviqwy.html

Py:   "ab" * 3
来源：http://hz.zycfv.cn/gtktabzrtg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pengpengdd.cyou/gtjbbtecag.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtrodfidrk.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gttxyfiaez.html

Java: "ab".repeat(3)
来源：http://hz.wangdashe.top/gtyqhqsgju.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xinyue.icu/gtpipbocup.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtshxvwfkn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhixingplan.top/gttwekjnxt.html

[E03] 截取子串
来源：http://hz.yongpay.top/gtfaikmhno.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgfzy.top/gtlmrmybai.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aibaodan.cn/gterhydalt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtpbmmzyxa.html

TS:   s.slice(1, 4)
来源：http://hz.svipenyu.cn/gtsspawjgk.html

Java: s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtdxnzawxl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtnmkfwbpn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gtkmvfrmfr.html

C#:   s.Substring(1, 3)
来源：http://hz.meibo888.top/gtuprhmwxc.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtguurwpzr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.guowangkeji.top/gtdmepnsbn.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gttbheuvyq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.dianchejie.cn/gtyiojncel.html

TS:   s.indexOf("x")
来源：http://hz.yueranfly.top/gtpvqogxpw.html

Java: s.indexOf("x")
来源：http://hz.gotoacloud.top/gthgjldpis.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtbybsjifq.html

Ruby: s.index("x")
来源：http://hz.yvedp.cn/gtiujcrjkj.html

C#:   s.IndexOf("x")
来源：http://hz.zycfv.cn/gtumpqfows.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtwjhfeecb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtucfgjfho.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtydewapre.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangshuangyany.cn/gtctllnjlw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.52xcode.cn/gtdjgrchmf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtyqvlmwau.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gtafhwzdwf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jqgufenzy.top/gtjgpzldzx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtcucsucju.html

[E06] 替换子串
来源：http://hz.hfpthk.cn/gtqztfnhcp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtjlooqkci.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtgnblmedm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtzuixefps.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtunukxpvk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtpggsuhyd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtmwgzxowv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtfzxkngrm.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gttqahvksc.html

[E07] 按分隔符拆分
来源：http://hz.jinghuilouyu.cn/gtfnsrywrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yonumen.top/gtcshaafxk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gtiydbkokf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtdjimozba.html

TS:   s.split(",")
来源：http://hz.yuanzhike.top/gtobqbpbma.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ivvv.top/gtiwvlnqgo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenjidiqi.icu/gtfiufukis.html

Ruby: s.split(",");  s.split
来源：http://hz.chenjidiqi.icu/gtqenfdjqr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtbuofvnyy.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtksqhqlll.html

Py:   ",".join(items)
来源：http://hz.yuanzhike.top/gtyfkcwrks.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtiyoysoag.html

JS:   items.join(",")
来源：http://hz.jinqigfzy.top/gtkjllfwdd.html

TS:   items.join(",")
来源：http://hz.shangyingyoupin.top/gtveswetdt.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtcidkctdc.html

Go:   strings.Join(items, ",")
来源：http://hz.zhengqikj.top/gtlpfhozlg.html

Ruby: items.join(",")
来源：http://hz.gogol.net.cn/gtpggfvmmv.html

C#:   string.Join(",", items)
来源：http://hz.iojbl.cn/gtzkfamhqb.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtthatnucq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtbriranjo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtkfabuaef.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtmhilzpsd.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtdgvwcvej.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ybcxt.top/gtwktczhtm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ppjwa.cn/gtctbrvxhy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gtyflkjsca.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ppjwa.cn/gtubpuxlpl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigufen.top/gtnsoolnip.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jqgfzy.top/gtusnsolrd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ehwqpu.com/gtiibdewrl.html

JS:   "7".padStart(3, "0")
来源：http://hz.sufxvd.cn/gtjnndhkyq.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gthbneifrq.html

Java: String.format("%03d", 7)
来源：http://hz.redwolf501.top/gtciwtpbnx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cqqwz.cn/gtybgjjsqk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtlwwlrnys.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtarulfvwx.html

[E11] 反转字符串
来源：http://hz.hnxiangtu.top/gtosmnycxh.html

Py:   s[::-1]
来源：http://hz.xuanzx.com/gteicjwsju.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtvfjvjixy.html

JS:   [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtvbwdenzk.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtkufxfjyw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenzaomai.com/gtugxkiqwq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.52xcode.cn/gtmshnzexc.html

Ruby: s.reverse
来源：http://hz.hysaishi.cn/gtnkrrgudz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtustoqnzc.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtxgsqdrtd.html

Py:   s.count("a")
来源：http://hz.zdqjudy.top/gtfyoskamj.html

PHP:  substr_count($s, "a");
来源：http://hz.jlsjyb.cn/gtgunkigqi.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtyjvfkbdo.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gtzewgdyjv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhoulong.xyz/gtddinqrva.html

Go:   strings.Count(s, "a")
来源：http://hz.0kj1m.cn/gtzahilcqf.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtcrkjmxal.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shzxlz.cn/gtuvtknevv.html

[E13] 逐字符遍历
来源：http://hz.sysykeji.top/gttppcjfqm.html

Py:   for ch in s: print(ch)
来源：http://hz.cucudq.cn/gtnazofcqy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gtokekpqbc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtxfikltlz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtmmwqfmrn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cashguo.top/gttilswvjy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nanxinkj.top/gtznmdhidm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtideenckp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fzhhl.top/gttsnoqcon.html

[E14] URL 编码与 Base64
来源：http://hz.birdmap.top/gtoyvddmwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hammf.cn/gtcnwrojve.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guowangkeji.top/gtorstiuwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtheqmbpah.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtjvbpfstc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhoulong.xyz/gtynqrsrmi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.svipenyu.cn/gtxhvdagzo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cheryme.top/gttnqekxuk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cdnleiting.top/gtgaqygfck.html

[E15] HTML 转义 / 反转义
来源：http://hz.yj20258.top/gtvtheioih.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtdrlwdanf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.haohaochexian.top/gtimgkmdft.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yuanzhike.top/gtftltvmmm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hnxiangtu.top/gtniorbcoa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.meibo888.top/gtommrjewb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuanzhike.top/gtwgybabkl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtxuiybgdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ppjwa.cn/gtqjjrixwn.html

[E16] 数字千分位
来源：http://hz.gogol.net.cn/gthltdjpij.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gthljzglnn.html

PHP:  number_format(1234567);
来源：http://hz.316326.xyz/gtrkhlpwlf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtkvadgsit.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtsiojmtcq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtyyvdmwgl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenjidiqi.icu/gtfosiqtfj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aizwys.cn/gtjgnitzyx.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gtivctztlp.html

[E17] 首字母大写
来源：http://hz.wangshuangyany.cn/gtwmdeglup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtiahmsqbn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnxiangtu.top/gttiqrdqtp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sweek.top/gtxmmnyvgw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.wangshuangyany.cn/gtemuvqeli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.havefunace.top/gtykibnjcq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtezmoejpi.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gtflchzdia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guowangkeji.top/gtlrmydrdx.html

[E18] 模板占位符替换
来源：http://hz.zhiwuduotai.top/gtoasrvvwl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yanxiufei.cn/gtabmhmldj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xylfe.cn/gtuhfntfoo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtoyutyyrq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtovhxursl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jiagoushi.top/gtbdbtnvpb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.fengsongda.top/gtgiwqlyzl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.aibaodan.cn/gtinthozyl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtygscatll.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtvpcfpdoc.html

Py:   s.splitlines()
来源：http://hz.yangfankeji.com/gtiiwagask.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigfzy.top/gtjhhbzbyf.html

JS:   s.split(/\r?\n/)
来源：http://hz.zdqjudy.top/gtvthuopjh.html

TS:   s.split(/\r?\n/)
来源：http://hz.tian-w.cn/gthncsesvd.html

Java: s.lines().toList()
来源：http://hz.xuanzx.com/gtazjdkqcs.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtfwirxlui.html

Ruby: s.lines
来源：http://hz.zhiwuduotai.top/gtaaabcqrz.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtxughimki.html

[E20] 判断字符串是否为空
来源：http://hz.bjfxy.top/gtasurebac.html

Py:   if not s:
来源：http://hz.xylfe.cn/gtxbsrkoah.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtsoyvfpfs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gthwwyeeur.html

TS:   if (s === "") {}
来源：http://hz.kuanghao11.cn/gtwfwmjgkp.html

Java: if (s.isEmpty()) {}
来源：http://hz.yuxming.cn/gtyqalzxhh.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangtech.top/gtkbvqryiz.html

Ruby: if s.empty?
来源：http://hz.jinyuanbaomall.cn/gtcqroklhy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.sweek.top/gtimfazgjs.html

[E21] 超长截断加省略号
来源：http://hz.smart0.xyz/gtxqndweox.html


<!-- 参考信息 -->