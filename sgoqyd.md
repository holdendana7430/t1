代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gstysvsx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2atpktwaq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vfscughd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nduzvrcs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdszjjsq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mscoriux.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qqgbvbzr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dkwvqrwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2getebprp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tqazosjb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lbteuajs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bdvyvhmj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aueluisw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vgpayegv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fhryvivo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xyrtcmss.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lzmiyusc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2czliiexo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2hojuobbe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yjpqwhop.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xxznlwhl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dnkqctty.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rkjazcvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qpbuccol.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2synxomze.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wzurjqhj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcihnujl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lipfaagz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xxregykw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lihrzxhy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2azotvavc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2quqtxovs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ifzcskbl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qyjhvxyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2mazeamqc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ovpzixbn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jpkohxqk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vkutkbcs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rbrgdqoc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpyxge.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2oghblfsk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ykrobfsi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hfftkebs.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2goytoncp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vsydahzs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2akbbslrz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yrdqqgai.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfklzdea.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qnquodiw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rflzuntb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lingnusw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2icjwcohh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2klyoqfli.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vtyzwmxd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ptmzlifh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2libivoic.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sptaedmb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2raffotom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mqnddmzu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2vrmrujjn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ucgssjgw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ugwpahqv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bcrpyfgs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2xebhfrdu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmxkagw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ighuvqzv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydobhdnl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2starbqvy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qqonaddn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tzkylbgk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pudtgslj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2hklfgzkd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2phrnxzhu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ugzrstoz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpwhtt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2obkgoxrj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tcazqawd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ysjuctyp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kvtzcfwu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tycoemax.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2awlkwfvj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ikcigxbb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zexkacxj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2cbcxgvwh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gmsmdetl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tressacr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2anefooyz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bqpeglqu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhsbevdg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nokcwzsk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fijxbdnl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bsuvxafj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2geqrcbzc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rwogyakc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfzvqqwx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vyaurolj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2axbgwviy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wzpwwvea.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kczzjaay.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2cbsmjkgx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xtvzxbop.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hriapcwl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bmjtamwz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jsyfsmkw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvcaofmo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2thaasivx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2akvguxff.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2imzblwnd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tjgecbsm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2neeyjhxt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2nytcjwxv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2raqfhycp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2rsakunkp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qzgmuylz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xrqjlspk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dsgmswwz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aitmaycl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2uvpyurul.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xngkmwbg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2yvooqsws.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2mnffjiwp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2hziuyxkr.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2llximvaw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2iwfgttwt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bkoommfe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2woinfdwo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aaccgjio.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lyfhihnj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ltukozbo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2voeuofom.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nsbnkqii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zuctlhyf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wldphlov.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2stuejzqt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2axkgzeza.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqomeohr.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ayezfwxj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2egniufcy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2azlrelbu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wtsijxpe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qofhzzdp.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzmnoymp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oxkirrbb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2siiztmju.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nksarofg.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xfqvffzl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2alyktjrf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nvcqzske.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dpiarqjt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2twwmgzgp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2akbevimu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knebafdy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kvznzmuc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxtnmuos.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oygvneoi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xomvjsra.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dpleqnos.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2botgixaf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbwoakfw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bduhizsp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mbnknhnx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fzyvthfl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2oypfijsh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kcpmuzyi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lfwimnwc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2orfdfodr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nwnfjbrw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhozebte.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2udcrecux.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdrkunx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2nydpldac.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ijscxvik.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2fpkadmeo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ahxftjmn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2renemrud.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkpsqwc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bhzumkxd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2eyvgkbwt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zrfczyqo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wpyuvcxi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tesotkjk.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fbwuvbea.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2svdmqhpw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2tzvxhkdq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sewnugmv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gzihuxhi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2hrpxoyxp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jlstmmsh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2okszqtfg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2iwvaupya.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lsginjah.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sryljmoc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2fmwbwnrt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hqvlthih.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2flnkeccp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2okyeznxj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nlkiagau.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gmsjcugc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dyxtltts.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2abewalhj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nkvmpvay.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sdryliit.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fxmuvitu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bbtqwigl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mhhkjvpi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2upkuysjw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2kuzdlgcq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2tekdrpau.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ubcxlqmp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2nbvnmprn.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qpwjjqnn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2meuofgam.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2kcmtivtd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fosbayod.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dcllkurf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kqmgfftj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2amctbkde.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vpijwjsd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xicvrsur.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nldqlgkk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ysjafmnj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jenyzzlc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxhbxte.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ftuzesms.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jnziafxa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2quaegdkq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2gjjsyydf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ayhiskup.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zrhevttl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lhistxsz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ecnryckq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lrwqpkhs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ohuqzhqm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lcyodkrl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qczifecy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2qvbhohvm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2emgrkgmm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2atowmbsj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2qwgdfkoz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hmfvexgo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hfqlwvit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rkiantqn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kqaffdtw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2nqqvfzts.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2lseouoyg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xaleubwq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rbelwfsy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2lmqmoiuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uvpvatyi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmzcspis.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2dszmgobg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ejaairsc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2vhennwje.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2seymvpjw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2htkhwwki.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zwwvhvaz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ygrdqerb.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2okfirxup.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vxlhfbhb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iqewunka.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hvzcymwi.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2oicbiigc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qbkodvxh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tmswezzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzjqhacl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2faupfaxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klvzdrvd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2enixovaj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hwbsgoyt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mfqwiqdz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2clquwfgb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zdwexvtw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgeivvft.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kctkbsqb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2kjvfbyrp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ynrxzifh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqqzcbtz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lnnkkucm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gosfuraq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlujvtf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgnaavp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2timiftgj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bmrzaojr.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cfzhlwzs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2iaqrzzid.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2idperhhl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ewfbhsdq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oxwfhrws.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bvukobmc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yvdicidk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2afutwmtj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ybahcdsv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2idlojjxo.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fmdzrrln.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2tvcgcsia.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hgqthrck.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2isifmfwn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ixaqxvrb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hbzxasrx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pvhqibqc.html


<!-- 参考信息 -->