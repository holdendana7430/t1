代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pnsemncv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2juesfykn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dqcfepai.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zjdflknq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2svkkpzai.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eagkrfqp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rhrucdcs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ulfqhozy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bzzppdka.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2empeolaq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pkjvsomp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gcmhlagu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2nmjizgad.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zztjasns.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2otvqfdxh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sbpfalla.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nubgxmnz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gikydfzv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zzwlfttb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kintfxwp.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2tnqmuhkc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ybjrkkvz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2efpskezb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkvpdyhl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pxskyrnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvhjgkfo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2anaymqpe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zliqvurl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ysrkeytz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rimpkmws.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2dellxseu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zoyhcmzq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2xayksevf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qjlxzwcs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2izwbbwln.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2lwplthyw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ckyqduvf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2szhajkzj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ojpqvtfa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uepdqwcg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2akgojvnu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mkpyjmzj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvjweyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wqscyply.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2oxrapvsf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vbqbsrvh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dpbagtlx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fhiichli.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2weuqvuwq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mjfilycm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2eoeozbqz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrezknx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ihiqrjvp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2dtywhyxk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2egxmkoud.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2veslbjqq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yyxpmukc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2krkfuzll.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ssmklvdm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wfawkmju.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cjxqsteg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bzzptlxs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zfwvqcrh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ikijecnu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jiivwqtx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vqocryau.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ljqlfguq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qsbvkgjs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zujqmzyd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hrjymfml.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dxiyrewe.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ufmcrtnm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bajxfgpy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fajnhcsf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dtjzukjt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2riozkqtb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rzynobfn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eevybcku.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2eoqeepvr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wvppoilb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2naaieihd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dzjgpfyl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iofttcrs.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uayoxcuc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qdicwgzy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kveuwfbx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2kylszfrp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2hyumdlcq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cjywocte.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2loeqvuin.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvedfrzz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dsgkqtar.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2trfqjuuf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xkdhbcmb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpugitud.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wphehsac.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzydhfx.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rxgiufoj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zhdxarlp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wunuyqge.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qeuhpqkj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jrxxfcna.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lbxrguhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2zcuvagxg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgzgjqqh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tgmaikna.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2tzupyfrl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2goofjgyu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eryorqnr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oogeuibh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2buvrftva.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kstyvnfr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ekhhvpgw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2htsrhoqa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wbkyofao.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jntpvahg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lceyqpng.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2lxrbigcc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxqscezp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2haytwxme.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vsmgrkxe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eggxenuj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2oyppkpau.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzzxugpi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kqvwfdqa.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wxiwkwbi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hwtqoqka.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hdytcdte.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvqsiimb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hidjbygc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mlbtwecq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wmqxiwpg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rmzksiau.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2veblkqtb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2txkadglc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2olkvzaau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjdnsmol.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qaslzybn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ljqsqpff.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xehkllgk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2lrbcfrms.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2brrsxheh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncxslcfb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2okgkggbb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kgpsrayn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2slwveqzp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wynvewxn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iplfccap.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ebqaztwh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jyjuavru.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2numqgqyo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vplrqiel.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2khrpwjms.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2smrpsyno.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2svswqlam.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2exysmxvo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dcgcrihg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ufsntzkk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ktnxkarl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yadygfwl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nqwvdavo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2guxvorhr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uuuocbln.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wchrtsdj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wirwvcxa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrxmvicq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2nfyglezs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2uvxlsmiu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2nqnmlexz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kvgqokqf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dpmjavby.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nncjyykn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghjdpjbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zsiikzcz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qbxwcjim.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2upbsudcd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bbxdgzer.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2hhpskead.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oxhejuel.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbdbzjil.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2uzbmenzc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2oektuanr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2agyeatti.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2fkndadsp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dotijalm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xaxxyfpt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rnsczjbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2klxmkkkn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ijojijwv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2humauykw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hbcouhik.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pgpitzrp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2iodidyeq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wvclwqbn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2cfovdbta.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ikfkeoer.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2izmchooo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gxkgtxis.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tswcxwuz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tfodyprg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lpgqcpwr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wagugqak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ltiyrifj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2zsbdacvh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2mtherkfq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fcwqquzx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gcgmchpe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qrrjzzwo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sbfhxiwb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lignxdya.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msviygrt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xftnqhii.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bfmnpvdz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gebygggo.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oreubyru.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2enqudofv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcenevpb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vskdtsyj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqwdslls.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zkvrwatx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ggjsdcfq.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxlocqn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yfuctogb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xriaikxw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iblcflsb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2oxtcznop.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ixgwkxnq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2njpumpim.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpvlwg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xtpifmkh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zksxzdeb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mukzbzrk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2uruqxzyu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2keeemafz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hxgurhns.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kekvcffg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2vtzlbtvz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kigblsax.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2rpagojda.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2skunzmnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dgbnevmp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2pxgzrrbg.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2khvwgrhu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2dldhcgsg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qangcikf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pdqudcqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2nkbizglp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lhhkwyzi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bigmryuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2apmrfucw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbtnzqg.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jmqmibyh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wthurxpy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jepdvmrp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2eswawgeb.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xjhzjzpm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ezcewlrf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2obwjwtur.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tzoourvw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kxuiaors.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2imuspdgl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2edvotpug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iamyitmb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubveybzz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2btanhmkm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vzdizlsk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qymxrszf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tdjfxmhp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ggwkilkp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lxxpkshd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2djnnhpfd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ksurlqcu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gkgpnmxc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2iwmvklmo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fygfyrdw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wthbulnc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlbruuf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lyccukkn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2eofwwpry.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vbkaaxzd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ghhuecdv.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2owelyzlj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2skgsuulo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aqimpwno.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2exxxzkss.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2fmshaalq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tlgrlqqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cxtqqkyb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fyyphxro.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2otyltxfe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2evcmsjfk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2knmtzgvc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vlncfaho.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sjnfsvac.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2racdwrtv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xublbwrk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2mteieiiy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2dllmkejr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dzrihtgb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vxhsckum.html


<!-- 参考信息 -->