代发 wailian999

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gttjwfmtsf.html

[R58] 下载文件
来源：http://hz.iojbl.cn/gtdefmaein.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtgdgdifvp.html

[R59] 发 POST JSON
来源：http://hz.ybcxt.top/gtclaaqxtr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhongyouzk.top/gtrzogyssz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtkoqljcxs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hnxiangtu.top/gtxbrubhmb.html

[R61] 磁盘占用
来源：http://hz.shzxlz.cn/gtshxikyag.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtwesjzauy.html

[R62] 找最占空间的文件
来源：http://hz.chenzaomai.com/gtsfnorclg.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtphtmniss.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtmuapknxq.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gttkttlbxb.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtrodkykrb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtnpcrrvod.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtzqmsgqvt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj202588.top/gtliarnhug.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtduosapgk.html

crontab -e;  crontab -l
来源：http://hz.xylfe.cn/gtnhthpejd.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gttkmkkiuy.html

openssl rand -hex 16
来源：http://hz.bjfxy.top/gtohlveblk.html

[R68] 计算文件校验值
来源：http://hz.cheryme.top/gtfjqutwpq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sxryk.cn/gtdpozgbwq.html

[R69] 生成随机密码
来源：http://hz.xziqi.cn/gtmsoskvni.html

head -c 16 /dev/urandom | base64
来源：http://hz.xuanzx.com/gtxvrywims.html

[R70] 时间戳与互转
来源：http://hz.zhiwuduotai.top/gtdgbileyp.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtzxbbjfbn.html

[R71] 日期格式化
来源：http://hz.ivvv.top/gttpqfvgnj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtmleufbev.html

[R72] 等待端口就绪
来源：http://hz.yangfankeji.com/gtccamtlcx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.aizwys.cn/gtormcdgks.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtimqiksft.html

split -l 1000 big.log part_
来源：http://hz.shangyingyoupin.top/gtxpmkvmie.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtmrlnmitf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtntqgqjnp.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtfqvxalvg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yangfankeji.com/gtstpyklvi.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtirytsbjz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtojcebrip.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtbsachjmb.html

read -rp "请输入: " ans
来源：http://hz.sufxvd.cn/gtuwwmmmlq.html

[R78] 交互式菜单
来源：http://hz.hammf.cn/gtansvlpeg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtkuyycuyp.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtezaazsax.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gtdsejkvox.html

[R80] 查看脚本执行耗时
来源：http://hz.yonumen.top/gtoeikskfq.html

time ./run.sh
来源：http://hz.zdqjudy.top/gtgxruelmm.html

================================================================================
来源：http://hz.quarkkingdee.top/gtubzwylze.html

S. C / C++ 专题
来源：http://hz.bjfxy.top/gttlcgcdew.html

================================================================================
来源：http://hz.zdqjudy.top/gtisncqaes.html

[S01] C：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtbsrcijhw.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtfkdxjcfs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtsclkfudj.html

[S02] C：变量与格式化输出
来源：http://hz.chenlongwang.top/gtennjxzuw.html

int a = 10; printf("%d\n", a);
来源：http://hz.guannengcc.top/gtalmpmorq.html

[S03] C：读入整数
来源：http://hz.wangshuangyany.cn/gtlmhutvtu.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gtipheruxz.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtlipzmdps.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jqgufenzy.top/gtmvlzlfjd.html

[S05] C：字符串长度
来源：http://hz.yueranfly.top/gtbnontaxi.html

strlen(s)
来源：http://hz.yj20258888.top/gthixkziov.html

[S06] C：字符串比较
来源：http://hz.fengsongda.top/gtksaonbrt.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtnppwqyba.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtyhrylszo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.nanxinkj.top/gtvqzuljqf.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtaiwvawle.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtfdxqgpsm.html

[S09] C：结构体定义与初始化
来源：http://hz.daria6918.cn/gthotdhfkw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fengsongda.top/gtcamsxohg.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtgkxnoyjo.html

int *p = &a;  *p = 5;
来源：http://hz.cucudq.cn/gtymwcfpuq.html

[S11] C：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtyuetbrza.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cashguo.top/gtsqcikwuw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtnvfwkbvc.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtmnrvaasq.html

[S12] C：写文件
来源：http://hz.jiagoushi.top/gtvtelesbk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ppjwa.cn/gtntkzmomi.html

[S13] C：宏定义
来源：http://hz.zhongyouzk.top/gtxobdutbt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.sxryk.cn/gtkjojaqbt.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gttkrjwkgi.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtconwduwq.html

[S15] C：类型转换
来源：http://hz.yueranfly.top/gtlhjdybjw.html

(double) a / b
来源：http://hz.havefunace.top/gtwlpjijxr.html

[S16] C：位操作置位
来源：http://hz.yonumen.top/gtpjmzbppn.html

x |= (1 << 3);
来源：http://hz.chenzaomai.com/gtdtsddptx.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtlmoaaqxr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.pycfn.com/gtauyaeccv.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtledykovg.html

int main(int argc, char **argv)
来源：http://hz.jlsjyb.cn/gtdmjwulvr.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtbrgwkneq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtiddchxvg.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gtdphaliwi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtbpooervl.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtqgvjsqow.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtgvljejna.html

[S22] C：字符串转数字
来源：http://hz.chenjidiqi.icu/gtjnnkqdka.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenjidiqi.icu/gtvmdywxww.html

[S23] C：随机数
来源：http://hz.xylfe.cn/gtqqivmuxk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.nanxuanxn.top/gtcuzuwgnf.html

[S24] C：获取本地时间
来源：http://hz.zhiwuduotai.top/gtttmrhyvg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinqigufen.top/gtmwqfqfpt.html

[S25] C：内存拷贝
来源：http://hz.yangfankeji.com/gtgkntgzxe.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gtfwiszbvm.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtcrkpdxge.html

memset(a, 0, sizeof a);
来源：http://hz.hongshengwenyu.top/gtapntomug.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gticeikrqe.html

const double PI = 3.14159;
来源：http://hz.daria6918.cn/gtvvcecoun.html

[S28] C：静态变量
来源：http://hz.tanke756.top/gtqzjckfrv.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtjurjatoi.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtenmwjsav.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.iojbl.cn/gtvtgxvbxv.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gtdlzwuxzx.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtzbnatjjg.html

#define X_H
来源：http://hz.iojbl.cn/gtxfqrnegr.html

#endif
来源：http://hz.ehwqpu.com/gtimennmec.html

[S31] C++：Hello World
来源：http://hz.jinghuilouyu.cn/gtxssedmje.html

#include <iostream>
来源：http://hz.nanxinkj.top/gtvoczqxhx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gtzeffayzn.html

[S32] C++：字符串
来源：http://hz.tian-w.cn/gtqodkdmxa.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtqkjragji.html

[S33] C++：vector 增删
来源：http://hz.xziqi.cn/gtbhjdgqso.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jqgfzy.top/gtewiaxhsi.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gturygdafw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtqahzgyou.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtjulsnwqr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtaeobptoy.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtszhggyul.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cucudq.cn/gtwnripncq.html

[S37] C++：set
来源：http://hz.fzhhl.top/gtuinwbszv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxinkj.top/gtytvbexqx.html

[S38] C++：排序
来源：http://hz.xylfe.cn/gtkinkpfat.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gttrgfqvlz.html

[S39] C++：自定义比较器排序
来源：http://hz.shangyingyoupin.top/gtqndedaqf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xinyue.icu/gtosgmisgv.html

[S40] C++：查找元素
来源：http://hz.xziqi.cn/gtjxdhqxnp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtzdnrmmct.html

[S41] C++：类与构造函数
来源：http://hz.gaohongyu789.top/gthacmkxws.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hywenlv.cn/gtrfruqrij.html

[S42] C++：继承与虚函数
来源：http://hz.chenlongwang.top/gtlsmfquon.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhixingplan.top/gtqhevqext.html

[S43] C++：智能指针
来源：http://hz.zycfv.cn/gtvccmnwid.html

auto p = std::make_unique<int>(5);
来源：http://hz.chenjidiqi.icu/gttvptpikz.html

[S44] C++：引用传参
来源：http://hz.hammf.cn/gtrewverry.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtayewmqab.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtkepmucad.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gturlavqhm.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtokkcwren.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xinyue.icu/gtzxfohrhg.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtxxkffssy.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gthubyirxc.html

[S48] C++：逐行读文件
来源：http://hz.birdmap.top/gtvjetqbgu.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtpqyivana.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtmuyavgzu.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gteupxvcmd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pycfn.com/gteqtpbfkq.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtjapzkswb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ydzc1.top/gtckjaqfnv.html

[S51] C++：显式类型转换
来源：http://hz.guannengcc.top/gtockvaosi.html

static_cast<double>(a) / b
来源：http://hz.ywan-chungtsiang.top/gtulaffibz.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gteuufizok.html

int size() const noexcept { return n_; }
来源：http://hz.ivvv.top/gtuxxmqylz.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtwhjfbyqf.html

std::vector<int> w = std::move(v);
来源：http://hz.hnqzz.top/gtzvfwvpjt.html

[S54] C++：异常处理
来源：http://hz.xziqi.cn/gtobkcrocm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gteekoqcxv.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtqypacmgh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.cheryme.top/gtzcgjwepw.html

[S56] C++：optional
来源：http://hz.zhongyouzk.top/gtpuerguah.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinqigfzy.top/gtjyicjxnr.html

[S57] C++：编译期常量
来源：http://hz.xylfe.cn/gtrcgettrb.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtiidpwiza.html

[S58] C++：命名空间
来源：http://hz.jianghu66.top/gtqwjgvbxl.html

namespace ns { int f() { return 1; } }
来源：http://hz.gogol.net.cn/gtwcwiqyfz.html

[S59] C++：静态断言
来源：http://hz.zhongyouzk.top/gtapxwwmbg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhiwuduotai.top/gtpsyrmnqf.html

[S60] C++：遍历并删除元素
来源：http://hz.gotoacloud.top/gtvhezglpi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtlnyfedjh.html

================================================================================
来源：http://hz.ehwqpu.com/gtnnzjkkcx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtjieasddl.html

================================================================================
来源：http://hz.9152youxi.cn/gtpcijlbif.html

[T01] Kotlin：Hello World
来源：http://hz.zhiwuduotai.top/gtddllgrej.html

println("Hello")
来源：http://hz.jlsjyb.cn/gtgsdhjpte.html

[T02] Kotlin：变量
来源：http://hz.quarkkingdee.top/gttrnwpkoo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtiboacfkh.html

[T03] Kotlin：字符串模板
来源：http://hz.gogol.net.cn/gtzuuvzuxp.html

"值: $b"
来源：http://hz.sysykeji.top/gthwxmhlev.html

[T04] Kotlin：空安全
来源：http://hz.zhengqikj.top/gtekzqmgbo.html

val n: String? = null;  n?.length
来源：http://hz.yj20258888.top/gtvnzkkpkb.html

[T05] Kotlin：when 表达式
来源：http://hz.chenjidiqi.icu/gtevsrmzed.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtohfscwky.html

[T06] Kotlin：集合映射
来源：http://hz.redwolf501.top/gtcdmrdijg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.birdmap.top/gtorklvenb.html

[T07] Kotlin：集合过滤
来源：http://hz.snrcjt.cn/gtlzinezbq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtcjdirmyh.html

[T08] Kotlin：数据类
来源：http://hz.nanxinkj.top/gtrpoblxxr.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtpwfmkaeg.html

[T09] Kotlin：扩展函数
来源：http://hz.zhengqikj.top/gtyysqszfu.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtrsubddef.html

[T10] Kotlin：默认参数
来源：http://hz.pengpengdd.cyou/gtvgdbbufh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yvedp.cn/gtfhrffyjp.html

[T11] Kotlin：协程
来源：http://hz.svipenyu.cn/gtqsyzobyv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhaomingkeji.xyz/gteghifbtg.html

[T12] Kotlin：解构声明
来源：http://hz.jqgfzy.top/gtuqoudpzv.html

val (a, b) = Pair(1, 2)
来源：http://hz.52xcode.cn/gtuisvceij.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtkgownrea.html

val m = mapOf("a" to 1)
来源：http://hz.bjfxy.top/gtzklzlpzi.html

[T14] Kotlin：循环
来源：http://hz.sysykeji.top/gttdgrnelj.html

for (i in 1..10) println(i)
来源：http://hz.zhengqikj.top/gtatjlamho.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gttpkctxzg.html

interface Shape { fun area(): Double }
来源：http://hz.jyoumei.cn/gtywvaxnbq.html

[T16] Swift：Hello World
来源：http://hz.sxryk.cn/gtckjgpwnp.html

print("Hello")
来源：http://hz.iojbl.cn/gtmtxhyztq.html

[T17] Swift：变量与常量
来源：http://hz.chenjidiqi.icu/gtqkhtbfzt.html

var a = 1;  let b = 2
来源：http://hz.redwolf501.top/gtiidzxjih.html

[T18] Swift：字符串插值
来源：http://hz.sweek.top/gtbjxlwgzg.html

"值: \(b)"
来源：http://hz.yongpay.top/gtkhgredvd.html

[T19] Swift：可选绑定
来源：http://hz.yongpay.top/gtfrfzaqvq.html

if let n = opt { print(n) }
来源：http://hz.ywan-chungtsiang.top/gtsefudkwm.html

[T20] Swift：数组操作
来源：http://hz.hnxiangtu.top/gtjpllkudg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtmgslqyql.html

[T21] Swift：遍历
来源：http://hz.tianlin.xyz/gtrjnntelg.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtghguzuem.html

[T22] Swift：字典
来源：http://hz.daxiang520.top/gtlvdsdnid.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.redwolf501.top/gtsszivjqk.html

[T23] Swift：函数
来源：http://hz.svipenyu.cn/gttfppudcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.wangdashe.top/gtkfoqyuwt.html

[T24] Swift：闭包
来源：http://hz.cdnleiting.top/gtrkufijdr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtqvsjxkfq.html

[T25] Swift：结构体
来源：http://hz.shuidangran.top/gtikmoruis.html

struct P { var x: Int }
来源：http://hz.svipenyu.cn/gtwdvrlymd.html

[T26] Swift：类与重写
来源：http://hz.hongshengwenyu.top/gtgcwbdvtj.html

class A: Base { override func f() {} }
来源：http://hz.hongshengwenyu.top/gtvlackzlr.html

[T27] Swift：错误处理
来源：http://hz.zhaomingkeji.xyz/gtmjambzpr.html

do { try f() } catch { print(error) }
来源：http://hz.guowangkeji.top/gtokryifau.html

[T28] Swift：枚举
来源：http://hz.shangyingyoupin.top/gtxadcfatn.html

enum Color { case red, green }
来源：http://hz.wangdashe.top/gtwavwuawf.html

[T29] Swift：guard 提前返回
来源：http://hz.gaohongyu789.top/gtumnhfepk.html

guard let x = opt else { return }
来源：http://hz.nanxinkj.top/gtjjnjxwzu.html

[T30] Swift：协议
来源：http://hz.zhaomingkeji.xyz/gtmojvcrbc.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtraqrmrmm.html

[T31] Lua：Hello World
来源：http://hz.sysykeji.top/gtiyflphfb.html

print("Hello")
来源：http://hz.yj20258.top/gtjklyqigh.html

[T32] Lua：局部变量
来源：http://hz.havefunace.top/gtkyqqyqdn.html

local a = 1
来源：http://hz.c1oappe.top/gtfjqvstwn.html

[T33] Lua：表（数组）
来源：http://hz.yvedp.cn/gtskpqqldu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtfnigkhse.html

[T34] Lua：遍历表
来源：http://hz.pycfn.com/gtpdtvxkqb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.bjfxy.top/gtwffccgjc.html

[T35] Lua：字典表
来源：http://hz.haohaochexian.top/gtrkmmiebt.html

local d = { a = 1 };  d.b = 2
来源：http://hz.smart0.xyz/gtkzaqmrhk.html

[T36] Lua：函数
来源：http://hz.nanxuanxn.top/gtpzcisryy.html

function add(a, b) return a + b end
来源：http://hz.daria6918.cn/gtfqvkgqxh.html

[T37] Lua：字符串拼接
来源：http://hz.kuanghao11.cn/gteodmsddy.html

"a" .. "b"
来源：http://hz.xziqi.cn/gtddvcsstj.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtpgudtsuq.html

if x > 0 then print("正") end
来源：http://hz.nanxuanxn.top/gtsgsoeetc.html

[T39] Lua：模式匹配
来源：http://hz.nanxuanxn.top/gtjmqbrnwb.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtwfpehcwa.html

[T40] Lua：元表
来源：http://hz.shzxlz.cn/gtyyxdncfs.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtamivtopf.html

[T41] Perl：Hello World
来源：http://hz.mhx1999.top/gtyxiyzsli.html

print "Hello\n";
来源：http://hz.svipenyu.cn/gtrsbjymps.html

[T42] Perl：变量类型
来源：http://hz.zycfv.cn/gtgqlvnoud.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yonumen.top/gthvwhquae.html

[T43] Perl：字符串插值
来源：http://hz.dashuyun.cn/gtxonsozjb.html

"值: $a"
来源：http://hz.smart0.xyz/gttpdxtkxz.html

[T44] Perl：条件
来源：http://hz.dashuyun.cn/gthoqtreju.html

if ($a > 0) { print "正"; }
来源：http://hz.52xcode.cn/gtopdqverp.html

[T45] Perl：数组遍历
来源：http://hz.cdnleiting.top/gtmoqboudp.html

for my $x (@arr) { print $x; }
来源：http://hz.ydzc1.top/gtkajbwwxn.html

[T46] Perl：哈希操作
来源：http://hz.sysykeji.top/gthdpryihf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtiisfenyu.html

[T47] Perl：正则捕获
来源：http://hz.tian-w.cn/gtmutfxkmt.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.hywenlv.cn/gthzzizdmv.html

[T48] Perl：正则替换
来源：http://hz.ywan-chungtsiang.top/gtwkphlhsp.html

$s =~ s/old/new/g;
来源：http://hz.yj20258888.top/gtqcbozkcb.html

[T49] Perl：函数
来源：http://hz.zhaomingkeji.xyz/gtgpatufyy.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.ppjwa.cn/gtkhxqjcxl.html

[T50] Perl：逐行读文件
来源：http://hz.jlsjyb.cn/gtobbatdwy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.shanyushiyangtech.top/gtlhtcuxlt.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.andypj.xyz/gttpguysoo.html

[T51] Scala：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtrxesroah.html

println("Hello")
来源：http://hz.meibo888.top/gtapbnpmud.html

[T52] Scala：变量
来源：http://hz.zhixingplan.top/gtjcwxabwo.html

val a = 1;  var b = 2
来源：http://hz.smart0.xyz/gtjdttvows.html

[T53] Scala：字符串插值
来源：http://hz.zdqjudy.top/gtfeaztuvs.html

s"值: $b"
来源：http://hz.zhijiandao.cn/gtkfjjelex.html

[T54] Scala：集合映射
来源：http://hz.haohaochexian.top/gtvwhmeliy.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.yuxming.cn/gthstxmvag.html

[T55] Scala：集合过滤
来源：http://hz.dianchejie.cn/gtihviymat.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.shangyingyoupin.top/gtsmunwnon.html

[T56] Scala：样例类
来源：http://hz.chenlongwang.top/gttuaestoe.html

case class User(name: String, age: Int)
来源：http://hz.shzxlz.cn/gtghszvlfo.html

[T57] Scala：模式匹配
来源：http://hz.zhaomingkeji.xyz/gtapwksazm.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.316326.xyz/gtpxralxvs.html

[T58] Scala：函数定义
来源：http://hz.52xcode.cn/gtvebyvlcq.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.tian-w.cn/gtrjumsyrn.html

[T59] Scala：循环
来源：http://hz.smart0.xyz/gtwvnodzkc.html

for (i <- 1 to 10) println(i)
来源：http://hz.yj202588.top/gtxkkprive.html

[T60] Scala：折叠
来源：http://hz.xingfuxueyuan.xyz/gttidnwvxi.html


<!-- 参考信息 -->