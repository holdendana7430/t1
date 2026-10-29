代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghihzzqcz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gkhjujupm.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gnpzcspfu.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/grdvgfdkc.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzcoyzbav.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fehbvm.com/Article/details/gjqbjjqjd.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gnxsttzpc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/grclhtfus.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gskiqjijb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gwmcsnhcq.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gqspgsqrv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/gtglecbri.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gvrjbocni.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gvhkdclbo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gundmhssd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpktkvcox.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/ggoirmliw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqmfzyufx.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gbvwcnhxm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gyotbnhrj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gkehfnuue.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gwyfvbkjl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/ghjfbjrpn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/glftvhykx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gwjggejte.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/ghaoedumk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/glpgilyyq.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gjigohhra.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/ggvpqjbij.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gjmlnaseg.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gaunhplmk.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gbxkbxfzk.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gnfspxrdr.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpthvzckm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gfdxsmfrp.sHtML

C#:   list.Add(4);
来源：http://wap.zdbjq.cn/Article/details/gidxvspys.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gkbkwxkzr.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/ghthdrhfr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gnzhrfrmv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/ghodziuin.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/ggiudcwtk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/grargcytl.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gzunbmwba.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/goayxwysr.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/glhtxdzzd.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gyrwifpuw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gpaaglsgz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gcehggxdu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/ggfaavdxb.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gzndmbnet.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gshqsbznk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gwezjonfw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gfktinrai.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gzyqggrdw.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gkjrmvxbg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gzxawddox.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gudlnrvfs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gsldeulad.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gmxhgxche.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gyeokcoci.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gnpzxgcuw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gbdykykiw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/ggjgmkdtq.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gepfxbvqg.sHtML

Py:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gxsmsdjcd.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmqwvahry.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gdkpfzhuh.sHtML

TS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gjfmiadrh.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/guhwersav.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gcvqoxxdz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gwytzjlox.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gpzmwaqrj.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gluurgrph.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gkimvwbbg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/guncfrrys.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gackdhhnz.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gnbkwovxp.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gtdynjqgi.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gacjaibmk.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gtlezzuwp.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/genvrzimd.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gskqhxkmj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/gelmwwgum.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/govjrwjox.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gphspywqt.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gycpedhgr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/gyrucqipf.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/grjfdakxn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gqohihvoc.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghyrfzvgg.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gbzhnndmr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gviktrqfa.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ghyuojmal.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gzhxjoxen.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gsrphgpao.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gfkyqnupg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzrpykjah.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gqaqpjxqc.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/geaiimwwm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gyhdlrxcu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gjtoakdkc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gwuslpxfw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gwnbhwoaj.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gjjgawhvc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gyixujcrd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gddvyupzu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/ggsbfknft.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/ghoiyrxoc.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gtkhikvee.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gbuffawdp.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gdkikiuqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gzuugorfn.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gpmbxhzvl.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gjedrssjw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gkbnwzggq.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gnqjmknbr.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/guyfhvnim.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gbciwooyw.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gyyczgnbt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/goboinxzm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/grvtkcnoc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gidhjtydj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gmindyugz.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmdonzipa.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gcsfzdxty.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gylgcjkeg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gqvzlatdk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gzyjakgyp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gfhtjbexs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gkbdreagz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbwsssxru.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gllcqylgq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gxaffvwzi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/glnqnwnxu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gplqkmqar.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gefzygwnj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.hesvh.cn/Article/details/gcsdqtckq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gtgdbswut.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gnjcilupb.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gvfczaqkc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqckgdvff.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gkrhkvqyl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gevlzhgat.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gskhxmzlr.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gewispzwf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/grchkgmkf.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwzgpdrqv.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gbrvabcnp.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gggtnwsxt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gzajxuszt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gkbusbaxs.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gaeimwtbr.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gwthhtorc.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gnsvhjkgh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ggkftkxce.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gjrqygyul.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggaqptars.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gedvultll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/glesnuwdz.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.zdbjq.cn/Article/details/gpuyygjuz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gzaqnnvwr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gfdzzipgc.sHtML

[D17] 最大值与最小值
来源：http://baike.fehbvm.com/Article/details/ganzndelr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/gmdsjdpkm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggxvgpezf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gihnrgqwr.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gvjvliekr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gsmadudij.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/guetecnxx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gzyuxiikh.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gbponkrzp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/ghnueogoj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gpwkgflzf.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gmnqgcrfo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gskfibbxu.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gdevcngfh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gmasfhiwr.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gqlnmxekj.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/giubwdjcl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gejsspzun.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gayaegykg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gduxnzwaa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gthigayzc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gokehrldu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gzchymsdy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gdlrgokfe.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gzsnbaxvv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/gkfofmagx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gjnnjjiww.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gpvcefoxa.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gekbqeafl.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gqvthqwwf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gozjposji.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gmwpchzjy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gcdnyqfpb.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gqlbxfthu.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gyrfbqlqe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gkwyhcijp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gmygktegy.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gunejbpaj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gttrxhuon.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gbtblzubw.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gddomrjse.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/grrqamqua.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsoubvfyn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghllhyrdf.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/guwjsudla.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.zdbjq.cn/Article/details/gpzdpzkxo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtuszhbid.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gilpzvesj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gpyemfcbb.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gczntnusi.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gacskrfrn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gveadawnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/giquaxwwi.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/guionosqg.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gofotgunx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gshfosqtt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gttfymfhm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnvzulxnx.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/goxjmdbar.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gybrzquql.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gbbkvhceg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gpeueepri.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/ghhweebnk.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gluttapcg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gfvrapazk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gpwionccp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gpflvqugn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gerpoybuu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gvhwyhiou.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gffyvercp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/ggyyuemfm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/glcurtqkr.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gsjraajeh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gjkxjyanq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gcmcvpjkd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gfezhhjfx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gpclxicsm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/gesmigmvc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/guagipyib.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gjjjxmcqh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gfhqjskuy.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gyoiwredw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gjuhrzbjp.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/ghwlzqedp.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gpdubsfho.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gsxzxwhzq.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gglnyvibo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gppjzmybz.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gjslqshyb.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gotpxedpr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvnrrkljz.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gdvhheyju.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvmrzanjq.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gztaszfkp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gviskunmy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gdzylzrgj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gspoouayr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/giorjdceq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gwvylglau.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/ghjfthtkv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gnqfbhiyv.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gaprdgrbc.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gbxjqiwxz.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gxpcgbyhr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gbrmldyij.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gwvssdxac.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gtlzjylnr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gzbpfthlv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gtnaelwos.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gzwwrwypo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gqyalobnj.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfyedpmzv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gunwhraag.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gqxnejeyn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gjzhvetvt.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gwqoqrxsx.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcjrzheju.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gbshbvzdt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gnndqztid.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gmqsnddda.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gixxezild.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/giwfvetgs.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gxueizjvu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.hesvh.cn/Article/details/gjqvyhxtv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/greonosrm.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gajbkuaom.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gufvkoluw.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gxgjzpvsm.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxhnkgich.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gozsdbokn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gofdrkgiw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gfdxscyir.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gpaooowwv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gzgdgvalz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gavyfrest.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gjuyfqqdf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.zdbjq.cn/Article/details/ggzfkeivu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gnvkwbrbt.sHtML


<!-- 参考信息 -->