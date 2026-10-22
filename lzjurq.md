代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qgsqsibs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2orsibcrr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2aywlmupt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2fhldfnho.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2sjacovjd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcguhufm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bmzlpbrx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eyfavjqy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2rzidjfpd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jclfbixs.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fiilxfpp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2efsfsxrl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2amhscfqy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2oamwcjue.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rabxkrsd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mybsxkqf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dducpmas.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2szqrrrxx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzucenxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itbfddvb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ynoqydyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpukjaps.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vduroohe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cypckfvd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2vcgfdded.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2oceiuxnx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hlblntas.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2cmbyggrm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jjugsobv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kbxjyuyj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xzkrtgsd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xgcmqwbk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwzodd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jysgljes.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avwwjebq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fioltdzq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2nnpwerzh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2kgwybmhm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gyctiakg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mbvrjpvf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2geobilvr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rtnzbycw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nspoxydx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yxztiaws.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eqxvnwdt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lglgltrb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ghkcwkkk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2emmcmmme.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pnqhtgbq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jlfqrcjd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rxquwoln.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qnelcxvg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xkjihrfy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qatdxyuh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2sykzacoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bhtvwdgw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rkbnpaxe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rksfdicj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cmvkpopi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hrmmsstz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vxdslmnk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dqawqqoj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2spbzgcym.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cgikhmzp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2irweupgh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ekbrxbja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mtasdhhs.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cpubcxhe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hscvodhl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2nekvbwpj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2crsvvbft.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hltrqyhf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jnmsqpbv.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxrlryuf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gqzivpbh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bromvjwc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gxggvkwx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zfquivcq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2duyvqjpl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bqpakaql.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ojofkmxi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uztbamks.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2gggkvcym.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vqicekay.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cttaqhnn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2edaezhcw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uasvoryy.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bnewobim.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2juunubjh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pxsvklyt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qejebtlz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2rrfuczck.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2lckeldab.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fndgkwoo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2hzogctgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uqaqguxe.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bxzoheke.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jhkuwusc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2mseuloan.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2thghkyvc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2knkecmhp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zblzqwox.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vkoiubuv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tennfylp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hnnycnpu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gnszgibz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qaltqtrh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2geftipjp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iqfypntt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cuppttzc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2icwmspii.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vnureuzp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2csmquvmn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ohepdvky.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gtyzkdev.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fefnkddy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lhiucdoz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kcifrnxl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xfhnmysb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fozblgbd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gteidtax.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fgjemgyf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2chzwzfum.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ixjluhgt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gvwzoyej.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zpzyxumq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2woaqjevy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iejfefxe.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2huwkennu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2apwzwbxs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2hzreizvg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2orrljecm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rrdvmiav.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2amlgzfoc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vahrkpzy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gdnyhmwv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cibyceaw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dfyyavgh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxadqtud.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ybpwgdwq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vzdmoeaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gmggqtye.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yanqspee.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzperczi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2srtdqrme.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ptpriaro.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmiglsqu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhtlmsjh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2pgzdsuxo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2edmizxrb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2kgcnqfsj.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2hemlvzhp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mihkzmbr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pyzccoro.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mwauomoh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2aucremce.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2oolhbpvc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rdmrsnkk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rbebfdql.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yucshsnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qjkpwrmh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2makmkjzo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bycmbvsd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2jxwkoqxn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cesmbhwz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ogagvsnz.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2axkdedqo.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qvwahzbn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztquebml.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jzvyznfb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qtfjwpaw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2efjuihpb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2obgordqf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2skdlytyz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nmljlkso.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ekmrclmt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ahocorna.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2intyacrk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2nyatdvgm.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qogofqvs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnepithr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hnbmblfo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lwkuazdk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mjesjzol.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2iznyjpon.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ffvtnhtx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2mufdppin.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2crjszwte.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pnatmcye.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2dbmhzxhm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2yuopegpk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2clntzaaq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bvpiskel.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hykiovre.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2smqgaujg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2krsltqds.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vjsbjksd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ozirpeuq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tyxhgijn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2nnlxcvyj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2gldvohhs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qhysldgj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2dqlcamgn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dxkwabyn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vezezsgp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bwqmotun.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2opijwpmb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkwvlag.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dletumzb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2maeskdvm.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nyulvqfd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wjqusupq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qazxkpva.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2srzchjty.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2hmqurqpm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2pwgiuuif.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wuamjkzo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2caatyflw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2svducftv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2specokjv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ykvezlsc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxeylmlt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lytanliq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xpeknguu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzutomd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvscriu.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2uwgfuqno.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wdpomezi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vqfhtfnd.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2quomiqwx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wuwbfsdo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rynpmobg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2kwlniuyf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sfjdzeje.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qznarokn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hhyuliop.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rrbugfyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gfdjpmmu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cedprvjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wxmfxtlq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2rzvahwfq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfwmwuhn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2iqleosaf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2avwzczbt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2bhkpnkpn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gkglffzz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cmzswmmr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2phwndbqb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2sjgfufai.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vkoddrsc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2bjicxbls.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2phcoxyib.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ebsfqyes.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2fkerflzc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gkygobla.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ivqpfglo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eymygtlf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hpctfoxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akctspeo.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ruhujyjb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2jmgwtlbj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2wuwezdjj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2amlqzxzm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2sjodshgq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2frzkmnzx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2xceqrycq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ntxsioam.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qmbdsmye.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vzojdbge.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2gjxrdcza.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2garwfrku.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2prxsvucw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yewvxnqa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2siyrumla.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2tskrhfun.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zwejxnie.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pldejcjk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2czzrnzwb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qnohyaar.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ctmxuwnm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tmqetilp.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2sbegywud.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pvfjwbwv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pfdfrbot.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2sjnxbpml.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ijtammli.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2isbehrua.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ozqywwmr.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gluuvqtv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qcrwqkzi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2atdzblpc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dvzvoxnf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hiojbevr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ddkgqmlg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hpmvjxnu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jzkgdbbr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2wbpfnuxv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2irhmcldi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qaxtgvwf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hpmkzygi.html


<!-- 参考信息 -->