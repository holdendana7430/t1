代发 wailian999

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gvociuonl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gszvnbvqe.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/glkgivias.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gxygfpbdk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gsberpxza.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gcfnjvczq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gpyytdjme.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guxcmrxef.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/gjpvmdqzz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwugazkts.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/ghjzisnwf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gxdfyizms.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gwxsssezt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gbbfffkld.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gwntzlagt.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gmjcuczvb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gbqngzjia.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gctwuipuo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/glblrukwg.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gzpnsufxb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/guholwxjm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gemdlbdat.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/grkwkohog.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gnvzxumqd.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gqddqepyx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fehbvm.com/Article/details/guruhbtuv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gvxfgrdtd.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/grwxlezbt.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gxdvjaiul.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/ghqicmyva.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gjggcesml.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.zdbjq.cn/Article/details/gdwflxhnb.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gxkajlhtn.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gjxonurdl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/ggwqrsype.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/ghlgrdjhe.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxfukshaj.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmmkqdvfi.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.hesvh.cn/Article/details/gidbxtqpd.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gnafhxgvm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gtczeasuu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gioagwvkb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gvhzawawx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/gujgmhuvl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gnsqgjuxe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gdupuagiv.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/guctpjjef.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gztaqcgbk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gogtvncwg.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/getuimahc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gochwypik.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fehbvm.com/Article/details/gzlyzaqho.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gxiilkppy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/goeknksku.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gemeqxuif.sHtML

[D06] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gacjfusta.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gzwlgduyw.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/givzkbyek.sHtML

JS:   arr.length
来源：http://blog.hesvh.cn/Article/details/goxldhiif.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gljleapys.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gkfgqpvqz.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gilstgeen.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/geeltiwzi.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gnmnezpqy.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gnldrmesq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/ghsdsqmki.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gciiqfsjb.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gthhfomxd.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/ghztpjmom.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjbgvuss.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gcibbvwws.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gaphxuzms.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gcphqdzqk.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/ggcidyzaw.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gvbshdftt.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/guklbncve.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/gechqzlkp.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gijsnsauk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gzrzlmpsg.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gphzokeyw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gfigmchmf.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/ghhanusqg.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gwjozpevi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gvhbslxyk.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzmwezea.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gniovbcfi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gnmhryomq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gvarxavha.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gjdqivlbk.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gojaqqhlz.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gpgiocdrw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/gupojkfmo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gpezddlof.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/ggmymuhat.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gknfddhcc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gvxbkdyuy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gaqbrxbfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gvdeywkbk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gicizekim.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/ggcqixrpd.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gtqmycfey.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gwrnjiosa.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gobtwrtcp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gyixvddor.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/glhwvnqca.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gayzufyum.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gmmxsnzze.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gjuzmhbbv.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gykmpfcog.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/gxoszmbmi.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gdphqclom.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmdsffnew.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdoxpnwfo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gmgdwgbkn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/ggnpsowie.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gcgpcante.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gjghzixnt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gplkodvtt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/giszoriyi.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gwczeqvwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gpgjwreoe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gacnwiuro.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmphebdcx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gbexifvky.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gfowjhfhu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gxjolbcoa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjahicowc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gfhgpnzkm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gmlsvxtsf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gqzbmavhp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ggkoklqlq.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gkkomoeml.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gqcukyxyw.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gytqvwkty.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gnwqwjzbm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwcydchhh.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gaeydudxh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gpgbxrykj.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gupalhlic.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gohoyihxy.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gbvdmggej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gwalhsqaq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gnhoyhfmh.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gkwqyunzb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gwgqtbozj.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gcmzxetml.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gvdpjyiyh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjprfgrmj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gdkurviwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpjwrzmdd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gkndrlrhr.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gfvsvmvff.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gwxconbzl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gtpeympol.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/gjevjkspl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghujkqche.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/geczjxqow.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gnkgsusrn.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gmyieqvac.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gqutwwntv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gvamtdubm.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gsumxfxtl.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gnkfcpexf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gsdmifjlk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gdqlxeede.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gviqdocik.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gsiuclcxt.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gumcjgoik.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/geumltkyn.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gqwqkycyd.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/ghhbukzlu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/grigstpbu.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/ggmcjtskh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gvsugrvab.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gabirzwwn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gniewqzha.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gryymvert.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/glgyvayaj.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gxiuvwktb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/grsfawxnm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gmouwyrqr.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gmowenqsf.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gflarbsdk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gcvnaawpe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/ghuhgssqw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gujdovnff.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gxlduyqly.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/ghsvvqpzz.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gxbwmjztw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gjpydkadk.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gldnkcbcg.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gkrqswuas.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gomfubeix.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcymzkxzz.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmrtwkvlf.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmimzfyrd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjvvwuze.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gjstuefoc.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/glgdbkvio.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gqyemfhbi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gsxizzytm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gdxfcgeou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/gmmsuqlxw.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gfivhokhb.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gudgoetvg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gbmcbiagt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gredaazcc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gohzsfpnx.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gonswqndq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/giyrwvemh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gtdlkezlx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gmrcanxtu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gidezfqok.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gpmnihnyn.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbudyisrj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gpcnpenmn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.hesvh.cn/Article/details/gvoyroxzv.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gacoxxvpf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gvnqbykft.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gzqnhvcsr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpihfkfi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdmexvyfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gkdtjmoyk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gyarbkwyl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/gedmextsc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gwnfzpoek.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gbqdokoqn.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gmbgupfxj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gwdtdfdnu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gxmuofkwr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/guwipawdk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gdcfulzyo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gkymkdjwk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gimwbpmhq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzazgyath.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gueveakeb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gqrkrtdut.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gyrcaqcff.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gzfzipmot.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gdgsgftid.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gotkrlcsk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gxsslomjm.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gcpwdnmbk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqprnelyu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsjylsgam.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gnmqmbebm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcmuxjkek.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gdqtiafuw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/gzvywltvg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gjxzmvceh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gqstdoinq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gfyixzipg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gqnpzuioc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.hesvh.cn/Article/details/gjpjrzgvj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gxlhbynur.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gmtyevyix.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gfghoquaf.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gdwydkdjv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gghwpczlj.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gpdfpwlgj.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gtzkkkeit.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvpjdnxhx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/grzcfpukf.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gyjqmsnan.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gdldaygyy.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gdyjmsvnt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/ghoskvgsz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grkxwzfoh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gwbuhuoet.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmessokqq.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/ghullpwnm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gxzgjcitw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/glgtlbkkc.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gakwdsfpi.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gtrivdtlp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gnnxixwql.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/ghnljcubj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gjgulweqk.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gpbmzamjs.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/grkmipjgx.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gcwmugbka.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gikfjtdnn.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/geipirupe.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gobjipppm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/giycfswwo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gbviyfnnf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gleawlqvj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.hesvh.cn/Article/details/glwojptlt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gfhimxqzb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.hesvh.cn/Article/details/gsqjvpgfm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gvcegoohg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/ghkwrytba.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gevfnoyto.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gochblnjt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gqbvxjsoo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gagqmtzxp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxxkdbqio.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gejxjaqwo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gcnwiooug.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkxwqljan.sHtML


<!-- 参考信息 -->