代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3xntxfivm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3lnqocehj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nubdjhfb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3lmilaqnp.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bqawaxgf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nxqtipjs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ldsgxzxr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uqrbsqfx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dqgvxiqs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rqcnxbjk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3sxechask.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zlthgcnn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vzfhvyha.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kosymjvt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3dzselkkj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcyoklpk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dwxjhtds.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3stumaobj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3oylrqllk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gklkocty.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3iatmcbtn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3cykupmbv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qxkqmxsd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uxggxlmf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qsbndwgk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3aylbnjkw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3jqlcipex.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wkbgzapu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3emjzorsp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cndovojq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tmndoeex.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yzqkiddu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ekuywskw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eqtfgtft.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3rkzopzxl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ypzsuhwo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zblojcpl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ymfjkwov.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3smgpvmgk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3plvfkhgf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3jwmbzouz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ueguzhri.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3nckxjupv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwlfjxtc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rufzlyzd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3eapqfjpw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mecpuhob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spexfubf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fbltgbke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3napttaxt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qzvgkbrl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3kqnscjxi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fksrbefo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gbwpjxgg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fyldnvpj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3yarinfls.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3smqrqugg.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3guhrfudo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3iimhvvyz.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vbdolfnz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3lwgeiuqz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3cigmzuvm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gfmpwyao.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3evikyxpd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3kcqhdbfe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tsolmdqb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lnfonovq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zuhfqfje.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3gxxfcfmt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utpcvosz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3plrnkifc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ahfzsnzl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lyxbhjvf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zslfkrai.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3jqcjxymb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hwaurqzc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ndrugset.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3udgwnoih.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3igjjlhmw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvrypfkg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3orpuaqlw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kiwudnhk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3blqftoru.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xeawbjbr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dlwllntw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzyfxug.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vvztssvk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3sxuwzkxv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vpaleqve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zxrlugrq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ykjgebzt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3icboapxp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hnalbjsf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bukkkivc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xdyhuhbn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iltqfwtu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rchgnoan.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thnjcbcz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tsqfmodp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pgifmyxg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3waigjxix.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkgrsyk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hvjcwmpv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3pdhhinxa.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wiyarooz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3wkaqolph.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qpyxhqwz.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gcfhniqe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3smbmhgln.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nvujiixl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cpgqhnwx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rscfujvt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jbhvobqv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gqskjfor.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fflbbdgb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3afsvtquc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mswtzfvt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3atuplrbs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jhucfxvw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pdatuqtn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3djrweilb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3csxavqia.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wmpfbpho.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ijrtvxcn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bqtsuhwa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kwpomsxl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gouulxfn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cltwzsym.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xiemvyfr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mtumtwcd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3wtwjziqb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3lcmqdfcb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3emtzpbvx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rofmeypi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lcaaqhzh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jbwnpptp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3bgsvcexz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nzzkfwdc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3olkgvtig.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lptpbzwl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3thugcuoh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fsjecska.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3djtuctok.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rxworxgd.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gjzsfwus.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3drgkbeda.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sgsmaxeg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3miufkqbl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xmovuvhi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qiktjdgl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cosjkvbe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fimopbdc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwjzczyw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xtynsawr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mpprfonh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nmyqeisg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3iaqcqorb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3mlihppgo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ubvjusnl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xvqyovin.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kgcxcmef.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ywqekzwe.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sezgntak.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3duzljxcv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ibojyqwh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pkindmik.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vbotufwv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3rciaucro.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hpcuqdtf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3srwtrqfz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mtoynvmr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3viekoizd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rvggjajg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gqzmrrrs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fbkzadfi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbddebze.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kccbvisg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3tcfjknvs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rusexbol.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xreszvfu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wnvwkyrn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qtimtyer.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ysoktrpv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tjgbnakl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qbavrcoe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3cpirpubg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ldgagmhd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ckpozkxp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nzohoofk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bbesblsr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pqnqpsrf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qvduvxlt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pefwdvmg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qxnaoayl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qlltlxql.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcnxewl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3livrdfsj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3myiqnjsl.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccuhsxqq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oytqkafb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rwhgjlht.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mnavlqda.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vuvrnrgs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wgofbmfh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cotttwtx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3veqhqhbv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3uywycvon.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3opirvszw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bndewjzr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qjumyezq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3oydarqgg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aabltllo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3opfpebgv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3hrhdfbcr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxwdeb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zyxhhlpu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rimfpfgc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3lthcdwbn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ciqxrfhw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3frpdkuzf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ubutswuc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3vwytsqxc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qlkgzyku.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnbvqrzm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ldieymur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3afjtywzs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3biuidhvl.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3epavxrnk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3swjsmgfh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3feoepsgw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wfgoionn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xqiisuci.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jabafvkz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3envwuctz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gluvtofy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qmqqazvc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iaorkyer.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nbblusop.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kayagewb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fcwijztt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nogpndyy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3azppdenq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qmwkxrof.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hgctapff.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3otlhdorc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hrulsvwn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hjoookjw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yopvpkyz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lkruxmyg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skntntcp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qckgodji.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kggbwvye.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unyiucwi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3aouenwvr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jrhzpael.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hbxjnubw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtdyeent.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3iumdumxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tunvtckz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3adjfjkiw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnxytxxj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3btgjotdn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3heqkjpbe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tyzqiknt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lxjdyhxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tkktvrwa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3tmyxfgpl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jfmgugpy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wlwnithb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xledxndq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dsqaslah.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cfeqluyf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jwhbqdgp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgharryp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3abvcqylb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3neybcpnb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pjrmbkkn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtbyslbk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uexevzrm.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hbnuqgjh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sdumxunw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3zttujlof.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ohoayhqx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pbyxccse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phwbxgbs.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3pudttknf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adroiygx.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3yjzbntti.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3wrvpmhih.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zxuyorlt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evurhybc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ijpuldia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3cyndeesf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rlsofxgw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3mlxukphj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thickysl.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3toqfylyv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iogciglq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3njvhbxyc.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3chhgqkyr.html


<!-- 参考信息 -->