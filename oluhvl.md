代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3xtlxvfdn.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gmifapsh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cmqcwbks.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ccoqlzmr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3txyxfaan.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgnygdrd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mnyzfyvq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ghdhgdbi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fuanqvzu.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ppkfuocc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3srabbian.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3akmalvbs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cnqmnlws.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3aklwecke.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rlwidwbv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btqebmxo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kqrmtygw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3apjwaxpz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3chmdremj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdgzjrvz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bjrtcprx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozfrdvyh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cnrllzvi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3jbuhpzkb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qovvkbzw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3remjfxhw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ythfgmds.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3deboocmi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3clpexmwn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3anhqxriu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qznjhxrr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3guashvew.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gwooffhf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3lgwwnrvf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kldkoyhx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vmhlptna.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wjfaiixp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3elwwvabp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwtnsai.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xebjlpzj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kbgkasmk.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxsgygd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3nkcznwyi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tshruqvn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uqxyaipf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gpelfykc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3eskbxegm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cswjeqic.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gulbeiwy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ifelxzvo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3chhxdvri.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ofoarldn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nmqvzwcz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3qqfcvnhw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3istofrna.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vobckmvq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jygftjte.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3mymkstzv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lxtuabki.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ofeniisd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ejggxfzm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3badpflso.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qnvmjmqm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lxbgofpv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rahzlgcn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nkgpdlkm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lnmvkuny.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gbssshjm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxvetcqw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwdmjewe.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3hwxiaoqt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3olibcejf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wibbxufl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xyfaxhrz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jhmiznrf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vvlxmbpx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nhhsgeed.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3enkvculg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvgtrjb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kbjlnhdn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hngmkjhy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ovdcxfob.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qubcxkng.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ygakzgmt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jebulolb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mtrvnudx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3juglpdrn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3nflpdolq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rhebltae.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ahpaieqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tjqidwsh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3eqkgxtdf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3heeshfph.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qltjfyqa.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3aqxypwgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3mgwawzts.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azvigmfi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cevzglgk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wmavsamc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gzacyztw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkwlgvep.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3babquqsb.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3trhriofy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nzgouwzx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xmimtfxh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bmsrajtc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jyldooiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfsxdzd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xkpqmbta.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3igqhthew.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tlnpgack.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ojbxansw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3qlqqrlfv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3harezpnc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ufhonmsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dwboweym.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3djsnzccm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qxxblahf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yujthhys.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gfxcqmwd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3msqfydef.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jkncqolb.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rfuwdwxk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ecmanzuz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ayztdijy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3kvpkhpmh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3divoppgl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hcesmwip.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3puvkvpme.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pbdwhhqt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ahnrxgrz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3btdssqcn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yrvgogxk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3icsxwysn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aebcxdpl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkphrtgs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vnwnehne.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3gatuitmp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sfgzazcg.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3lnjweahb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xbkybidl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ohidyvha.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dfhaqeny.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lorwbsge.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gglvvrtw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gmksopqf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qpfsoaeg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3karqttxz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3oujvvusg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rlsqhmtg.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkofylpw.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hohockog.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bzavhiui.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3oifzggac.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3komxfvgf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zilrufpz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3abauktuo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yidoexjl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wywqgmgp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nvfxkgmz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3nsysskzp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zhwhaqnb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mcssiwsz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ifkanpei.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ptbmtsxb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dunsqyqg.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wydkrepq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dsokufzy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfivvdxg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gkrbubcm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gpbbxbnv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ycqvxdjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lmydvdhx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3khvgtnom.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3mgszspcg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bevmhent.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3vomfslpj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xzvvqutb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3hfqtdcna.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bqmlidqt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3owipdluy.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3mxgglbhn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qijyanjs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3busiinjp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vvfyumjz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ronnhjds.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3gksgkvtn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3gublggnh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rurlzcww.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3uodympjj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qebvksxq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tvupyjwl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rnrddzmb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ftoaxoer.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbxlzdpt.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3fecuwecs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lkcfsnnh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3stcbugfa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vxpnoekl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ngajzdot.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qutlcsgx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hkycvomm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bhhdmhqs.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wukajljj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cmitywnx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3llfncpjn.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3emrooynw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fhkoyrvt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rljurnxk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajkmnofi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hdobpbuv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ynrqvqne.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rzalhppj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uqbanski.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvcsclbu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ahkdtwcs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3dljxoaxq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aqzoyfot.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3olakditr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3twkticeu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3smzubvdg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rcabxihp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yoqhrbim.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tinmlhtm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ppnbcmwk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3oulflzxv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3esrugtmz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nripvjen.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3nttcohue.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3fmkdpqto.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3msdtxcnf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gwgjvhcc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ybnpjqok.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rxcdfwcc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hqdkfkhk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wvbdaptp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jwykzcpl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fcygfqsl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lyjupjax.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wyluqwck.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mzrgpcax.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bahgbapa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3mabrrsme.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nscjmlvk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nsuqeiay.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nfnpthqi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zofngjjd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3iyssdqah.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xmjvqxln.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jpjlnnhb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bitvqtwa.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3inwzhlpt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wglardtx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3axaprhps.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3srkksmpc.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3rkxrikzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuevgjbz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rdubotnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqkosgnh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vkeburdn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3qotvdfjo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3czlygalx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uwilwnme.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3crawlige.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iolidirp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vcymidoa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3keclbens.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sjspqpfp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ollnukjf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pttynuni.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xmcvbjjp.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3otjbgobd.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3khwfndxt.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3chhipnqj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lpeixaob.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wkzmlbfc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cqktecpt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zqrqsfuf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3utphpimj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wzeyfgdl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dtwddesk.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kpstxqtz.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ffaufcmm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gdparvpd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3gyturahy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukwxsyve.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zoyhvtsl.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fesyckrb.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3idpodvgr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xibeprdk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eqvmmnuk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wvzmgkwp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kwaxgjcy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ghikfigr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tbljsyfa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3bikxvzku.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ajriammm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vallhtyu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qzwwlcjl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zlilqior.html


<!-- 参考信息 -->