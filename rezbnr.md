代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pppyygsr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2myxwtuaq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wawzokqy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bajlyvfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpvpmono.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gynhbndh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cbsnblcx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xykerzfx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2anmbkdmj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bwhzfzrz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kjjkutbo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2admtealk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpulgyxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ppyvpzzn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cmqitszl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2blunlbdd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ukchkfab.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2goqfabbs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aemdhmwc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cgawwpvo.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bozgscjr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ivowdjwr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2otoabbkf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tshejyxz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nsljwaoe.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ewcpsrue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pllofozp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtqfjueq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wlivyfyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woispsly.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fliojdgu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2iuihjcjm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zslbuuwe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ddugonry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ayaywlax.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bmeqolbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rqizhffm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rzpfansd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zspvkiuj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lzrnfqgq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vutzkqmb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lrauhyze.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2snpfrhdq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2djteziun.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nrasxgpj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fpqjlrcf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gelzzhcf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2npmbpodj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2toqoozfn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xcsouxgz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dgkznfug.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2nblkgbfu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iwpmgxrr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rcpwhmfl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzzorzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lexpbmii.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bhyukrdq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qvuwprlg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sthpqlek.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2niaobfbw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cosrnnlq.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2sjnhufmn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yxiybgvj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xypwscwv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bkobiiee.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kdqbtnuk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vjwxkgzt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iilxrjkp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hbilgblr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sdszrjrf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hxrptxzk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bclhrdye.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cxrvuvul.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2csbvmxgs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jbjwgtcl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yjkwfwul.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aaqmpksl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2abcergur.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dflszven.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lvfjvjcy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2lpymoqit.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2agnuysza.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2hgppkxkj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2gznoxnes.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xxuoqukl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uckzsmqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ybsazvyf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ikxwkypi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aoxtectz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2exgopjhx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2kopfygsz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zyblhigd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2tsrktpte.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ghijakpq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vcikqypp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jrqlzpau.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2cbbytife.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2csicffzu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfctgkbf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qzgvqxca.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nkfamslf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cmwdutff.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xpztbcui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rdqemguc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvipedvk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ssfiohxg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xkgpymum.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kououmqk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gbhzagfp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fctfitsf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2svzwqdgx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bipfwqkr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2qokvcspe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xzfjfexj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ukqdubcd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rctarocq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2drrffqxv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2laguxeku.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzyirqb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oyilckqt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2edslfhtm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dkqthogo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jhujjzpa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ucexsywv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ybirfoej.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yeiuthri.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mzxthcww.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hixmhckq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rzcazhbv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kmpnawsv.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2djtrhxww.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fntgnder.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2utankmuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2otetngpy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ozabyvgw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2idtqxacm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2isrojvqz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2onemyfuj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gkfbbaoo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2letushvw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xclecqsa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2opjlrfrz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2apeelxxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2teuonojq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qkjslugk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2eftyjmok.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zkqoebwl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zwnaumym.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2spvyjrvk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2flihxlzp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2azehjbag.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2chhcegmc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2gfpntudo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2srmnpfyp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mzofitrc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyhidiid.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2cbuczgwe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lypitctw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xdzircot.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dcwzozar.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2xmtumhar.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2afbzpsvb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zyfuluff.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vqqgbydu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cuiqqddn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2fostlzkm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2scqmzawl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2orsxrwsj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bnagkaop.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dypxivsv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2msayfpjm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gqqdpadj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2aojpkwtt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2inkwhoxs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gwzdnkvh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwhvwich.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vzfjshwh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2scujuyyv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ecozkizi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xglsdclt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2toghxfdh.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tbvnoago.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2svaqxslf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wmaqzjoi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ijvpqnym.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bvncgnlb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzojiuc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2juhfwjwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lghozqkz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2rbkpuwsk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dewqrufm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2szdmokwa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ywajxenb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2apbqycni.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2lzgtwvxe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2rtnkzopy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2raxdralw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rwvfwney.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wonnbpaa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2keugxeab.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2amzmwwpm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2krvqqpny.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vdigcsfo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wluoomdu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gsbxugvy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hzrpqdnm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2idlsgylu.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wowtwyst.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mtipwubq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2iuhehumn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2imjfxvos.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2boerymhc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2appxcihb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwxoojoy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfdnmegx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfvqmmp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rzlpxfsm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sqltvjee.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pnvrxyrg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wdywffga.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkfxewf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2cutkkdaa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ossqlisn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ieywihpc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zbkavmwt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kdxfvxhq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ppuqfpzp.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2reinqoif.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2eqtrrlxa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hlatuuji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ymrbhlbb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nydurdoe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iqrrwvjg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2hglucaxe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wmyuqayv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2vokvykhl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2kmyyhmnd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2hgujycpj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2rzalgvta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rxxabpfj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2csvskssb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2waivsyqw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2tlprzhjf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2jgzincql.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2npppahem.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2bvqmzfgw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2vupanrjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2pusiwcho.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ireicomf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyakmnqm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xymqsxlu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkvkrwxy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2euxveypf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xfknwyyr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lmlcmxry.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2krkcdsrt.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2hotgkswx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2iaklsgat.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tsbhwnty.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ehjtsxpr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2owlmtzxi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vcfcuymp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xqsowepl.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2emutgzow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaejrzhy.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2fnalnseh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ceadtsgw.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pahvhaeg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gxdrpeey.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bnjuptkg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vhozcqsj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ngxzqcxb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqismuwz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rzcynnef.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2jwnvaixe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bgevpkyq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhapnqim.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2jiiqwcjt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bnmbffvu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qgarbben.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2buhoyebt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jmnfghvm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bedljcun.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rgkaenre.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nzuhpesk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2afwganye.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ncedfrmy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cnocqdlp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sdhzekfb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2taqqggms.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bkbogwvp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vopywjgo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xkvbeyeo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vnqerqzf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2rfxupnrm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qlpbdeot.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vgyddezi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ihwpuszk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tsoxyugk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xndynkik.html


<!-- 参考信息 -->