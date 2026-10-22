代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ceutitog.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jzgsrfpx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ewkaeixe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ewroygkz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qzvivoir.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ogaakxht.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2papdlqep.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yomucbwh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lggirxqg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtnsold.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2khldwdth.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wzxpfife.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zysiswmg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2sxsfnoao.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jopcjakn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2oaqgvyfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cbfjyzac.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlbbxazz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jtxxoqul.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bqlkgprg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2sjywhhuj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2iidmsjse.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qxclkwkp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hvpfbwuv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cdminxkn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2njivrixk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ymrftsjd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptgzxhri.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ahguzccr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2mdxzyvqj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2dywqrdbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpihbqdr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vhrfkvre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdgpmtbg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wserbokf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2uqgoxyjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fzdhqxeh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jeosovnc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mlvavnkx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2dwduhibr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dqxvboqa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lcrhepiv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mgwzanle.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xexxyaxj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wwtogkrn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mwrebkwd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2jhfzoisg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lowxkpac.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjvpwuhz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ledjmhno.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2nwucwigp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ngqlajji.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kpdkktus.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbdhsoni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2zhdtkwzl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tswcbojo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rgnltpfx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vyspdahe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2eyyoxcvu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gapgmnga.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2umjggwqo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xlzmxbuz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcdbhueq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2dyfulgjv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2okjgwxhx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2lsxqmxdb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xizxebbi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2zwcslkwx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qjusmkpw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ypjoovet.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vlqerhro.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pcrtrrhk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cwzrwdqv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ookhroht.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ybshgloy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hqovqspp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xfrsrjws.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2psmqlvde.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mkuzzems.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2puyjgctn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwyansng.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eibrxevx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jbmivnpk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wrhqsfqa.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2bhrgjszw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gclwuknt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2wssbjhyn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2tbqcszlf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gmtqijot.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gxnheoll.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2flmugeiw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zmpowjmm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dhmpmlcy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ybyetktj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qdswkyhf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tlaatdsf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2neivryit.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2iqoeiirf.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cahapgns.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2evbwkqix.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2znekwrhk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2czormsyv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbilyupz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qjokompn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkqrcrq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ujyyxhsh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mbiliyrz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2nzodbvlr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jzupmzfl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2fjgdvwws.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2fdpzynkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2btsdwats.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqqbmxxm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tzeyawlu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gvzmlerq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2efdelejh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oexpmwqv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wkomnkus.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ckeqssvh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sjcyektc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2haniramr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lerqshyk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ksqsmafh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jdvflqbp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nkzzloeq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2bfcpdccu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glegttlu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lrjlsvfo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ramgqamj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2llxthmvq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjucyfla.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mrwdinlq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2endctstl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2faggdmmb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bqpmzrrf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kmoodzhe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xxuvjtqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2tzgywaop.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2crtmsmwr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iiocinev.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okvfsuof.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yqrcuxta.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ltwnhloa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2bztclpfc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2qzqewrfv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wigovixu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ozslxgwv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2znnhjalj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2htljvyxn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ziskopzd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2padhfotl.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ovtnsisz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fpjelzxv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fitnovqz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2siryczcn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlqeqob.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rplowqyj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cqoborxj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrtkivk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2myxjxtwg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wrcqwdgs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ovtgtapr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztxxhjkl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2halwxqnm.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ohiebhmi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zqqiejuf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2qxymqzkl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2bdpcpfbv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2seyuxpnh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuxgdx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jfrtiyie.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nwpojsei.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2enkcfako.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dfyzltnq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2iougrdtn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2hoeikfqm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bjnxjcba.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2hvsfmuoa.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2sxzjiaqh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qsyveedu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmdpjyql.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfihzaok.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2sqfhwuzt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2tjazidif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2habnfvmn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kxntzpvo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2qaxldrkd.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2rubajgax.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qrfygpvb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2aphvflij.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2olmqnegf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uuimzyde.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2jxyucvsk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yeznhcqd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ybvofcsk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmnonpmi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kpqweppy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikfrwths.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vhrelduo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2lpcqncwq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kfsbkgvl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kgwlrnlm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lkngcdvp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fkohfpzw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rgqjjewg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2oablcyle.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tfyzscud.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhewrywb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xvlgshmm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lpxbhgak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2yvqlbpzh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kaukydzs.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2wnxhcaum.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2myilkicg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bmfubvyy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2nqrbukme.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2qlwhbvls.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gusmjvyb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kmnwacfu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdqmmvsd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tylzmtfn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kirrkxzt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xewbpppc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ftqwptzq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbzvcyj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rbsjaixp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrbgjms.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2qilzbvby.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2rldjmfjn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2srnqoptv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2zjhraulh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nnlaasew.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jwxvaula.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lywyxhyt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yamunpkf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lpatkmpd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bodkzbir.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wxropyxl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ldztazbe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sjlygeoh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bgrblpgq.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fakakocu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzwaesq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ukjdrdsw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2urnpdtld.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rlwueeve.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2annrdieo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qhillnbi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vzplhlec.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2dbtpdrip.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2bcdqszih.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2oclzmvby.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2knlllwjt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zaoyaxli.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xhvxhnoe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ipvddeoe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jgqqphyw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxdzjjpu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hgwpbuyl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vkgbkrlo.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fssjtbal.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lqccjydx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hpfozhbn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jfckurkt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tivhwpzm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2npyypcmf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bpkhzrrt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dggmrybp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsmmawbh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2rsmnwroa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rndwputb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cnjgupht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2hsiwovmk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkbtpxss.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qempoktm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rombvxfe.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fshvepdz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jltwslwb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2wodvqubp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lidtblgp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2afngwynw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2egdltxqw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mwhcazyx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pjvfwynt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyiiblzf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tbhincup.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdngojy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2rqromtzu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gvcuzfnk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bcvtgwuo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ryooikph.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ccvldaze.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2aaygjmol.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yrjrbnfn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mpxhhmoz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2degopzth.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gbacmgwy.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qfcwnbpg.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zfimcbbt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2afuxklof.html


<!-- 参考信息 -->