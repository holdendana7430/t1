代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ppjwa.cn/gtcqrlwnxj.html

[R52] 统计行数
来源：http://hz.pengpengdd.cyou/gtbsklgdkj.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtdwgbcuii.html

[R53] 查看文件头与实时尾
来源：http://hz.zhengqikj.top/gtaduopmlc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.chenjidiqi.icu/gtppugxokt.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gttsepmehl.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtpmuytzhu.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtgmvgtbds.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.bjfxy.top/gtvzydvdos.html

[R56] 远程拷贝
来源：http://hz.tian-w.cn/gtgstwhdvl.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtlujpxrlg.html

[R57] 远程执行命令
来源：http://hz.jyoumei.cn/gtzpwphvus.html

ssh user@host 'uptime'
来源：http://hz.shangyingyoupin.top/gthauxfigw.html

[R58] 下载文件
来源：http://hz.hfpthk.cn/gtcukfqnyh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.pycfn.com/gtyvhscaoh.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtrsetotfq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtwnrfreyk.html

[R60] 只看 HTTP 状态码
来源：http://hz.yangfankeji.com/gtrtcxrsjm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.daxiang520.top/gtofwhzydo.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtlzhiwepy.html

df -h;  du -sh *
来源：http://hz.tianlin.xyz/gtsjyrpjym.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gtthlmnwvi.html

du -ah . | sort -rh | head -10
来源：http://hz.yj202588.top/gtkghdfsky.html

[R63] 内存与进程
来源：http://hz.havefunace.top/gtfcniezdj.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigfzy.top/gtnrvrghna.html

[R64] 结束进程
来源：http://hz.dashuyun.cn/gtesmfhxbq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtxfwgewad.html

[R65] 查看端口占用
来源：http://hz.zycfv.cn/gtubcxxcvk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gtqxuxxeum.html

[R66] 定时任务
来源：http://hz.wangdashe.top/gtrpqiyakg.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gtaiuputtr.html

[R67] 生成随机十六进制串
来源：http://hz.aibaodan.cn/gtpmlzlsvb.html

openssl rand -hex 16
来源：http://hz.gogol.net.cn/gtjsswmytv.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtxvbmruck.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtzwnjdork.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtocbofqae.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gterhfuzqx.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtxrgtjchy.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtkwypixba.html

[R71] 日期格式化
来源：http://hz.yj202588.top/gtffpszpcx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtjscmikhm.html

[R72] 等待端口就绪
来源：http://hz.cucudq.cn/gtygqwndil.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtdltyxhfc.html

[R73] 分割大日志
来源：http://hz.gogol.net.cn/gtgsfssbpt.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtjahdihaw.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtmrqiofqo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cdnleiting.top/gtbvqttjgm.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtuwbkcvkm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gttbclpnjr.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtivfeihjv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtfkwxaumw.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtgmgpgjbk.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtiaaikzaw.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtpeclcpvy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.andypj.xyz/gtzgbhktrc.html

[R79] 解析命令行选项
来源：http://hz.gogol.net.cn/gtixhaejrg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.gzhubu.top/gtgrflrpwa.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtfrdsctiu.html

time ./run.sh
来源：http://hz.tanke756.top/gtihmtikcu.html

================================================================================
来源：http://hz.havefunace.top/gtakpfibfz.html

S. C / C++ 专题
来源：http://hz.aizwys.cn/gtxqbenhne.html

================================================================================
来源：http://hz.cheryme.top/gtpwccezmq.html

[S01] C：Hello World
来源：http://hz.0kj1m.cn/gtebflywrs.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtzlcebduy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gthclwvqgv.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtkollptnj.html

int a = 10; printf("%d\n", a);
来源：http://hz.havefunace.top/gtncyrzeiq.html

[S03] C：读入整数
来源：http://hz.cashguo.top/gtfanpjmzx.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gtntmnpcke.html

[S04] C：字符串复制
来源：http://hz.shangyingyoupin.top/gtrwiucott.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cdnleiting.top/gtxiaidviq.html

[S05] C：字符串长度
来源：http://hz.ivvv.top/gtuelsbved.html

strlen(s)
来源：http://hz.316326.xyz/gtgoflhyjt.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtlgkbgylx.html

strcmp(a, b) == 0
来源：http://hz.wangdashe.top/gtoduvuajz.html

[S07] C：数组遍历求和
来源：http://hz.cqqwz.cn/gtpuvgogvv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtoogcmopf.html

[S08] C：动态内存分配与释放
来源：http://hz.nwbrower.top/gtxgcpqtsi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenzaomai.com/gtmefgoqnf.html

[S09] C：结构体定义与初始化
来源：http://hz.shanyushiyangtech.top/gtwwmatsjc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.316326.xyz/gtktvcsqgl.html

[S10] C：指针与解引用
来源：http://hz.haohaochexian.top/gtvafuoyou.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtkyfprxud.html

[S11] C：逐行读文件
来源：http://hz.zhoulong.xyz/gtzkoeavmd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtxvweolwl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtepbzzkuv.html

fclose(f);
来源：http://hz.shuidangran.top/gtlyqnzxod.html

[S12] C：写文件
来源：http://hz.cheryme.top/gtokjvawuy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.316326.xyz/gtevhphzyr.html

[S13] C：宏定义
来源：http://hz.cashguo.top/gteehzqlkr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hammf.cn/gtvecuozpe.html

[S14] C：枚举
来源：http://hz.0kj1m.cn/gtopyltciu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenzaomai.com/gtungsshgk.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtjvycwzkn.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtkgqozjqg.html

[S16] C：位操作置位
来源：http://hz.hammf.cn/gtywunyvkg.html

x |= (1 << 3);
来源：http://hz.iojbl.cn/gtpkngeewy.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigufen.top/gtxlodljfd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtegaxydgj.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtgtoyfpgy.html

int main(int argc, char **argv)
来源：http://hz.jiagoushi.top/gthhbdctqz.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtguymjpcp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jiagoushi.top/gtvhmanfko.html

[S20] C：二分查找
来源：http://hz.shzxlz.cn/gtxodykvab.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtfvdusnlk.html

[S21] C：字符类别判断
来源：http://hz.feifeiyinyue.top/gtepttdiqk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgfzy.top/gtcwyovysz.html

[S22] C：字符串转数字
来源：http://hz.jiagoushi.top/gtxqmmgtuk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxuanxn.top/gtbynqofou.html

[S23] C：随机数
来源：http://hz.zhijiandao.cn/gtbwplvuqw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinghuilouyu.cn/gtfrvuzzqn.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtxbaueyzb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zdqjudy.top/gtebqnzewi.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtlbaxlfen.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtukwkbqrc.html

[S26] C：内存清零
来源：http://hz.redwolf501.top/gtarbuvylz.html

memset(a, 0, sizeof a);
来源：http://hz.chenlongwang.top/gtsqehwicr.html

[S27] C：定义常量
来源：http://hz.hnqzz.top/gtljnnztwe.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gttlxytjhz.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtydszuzig.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtrmdobwon.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtfgstuemj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ydzc1.top/gtzmvewuto.html

[S30] C：头文件保护
来源：http://hz.daria6918.cn/gtksgsamjl.html

#ifndef X_H
来源：http://hz.yonumen.top/gtccuwnfzz.html

#define X_H
来源：http://hz.gzhubu.top/gtqsmjwzfn.html

#endif
来源：http://hz.zhengqikj.top/gtsbbajjed.html

[S31] C++：Hello World
来源：http://hz.jinqigfzy.top/gtmbzjzucj.html

#include <iostream>
来源：http://hz.hysaishi.cn/gtgknddpuu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.feifeiyinyue.top/gtynkvopvu.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtdwkdbopb.html

std::string s = "hi";  s += "!";
来源：http://hz.vqdsnc.cn/gtkszlgmld.html

[S33] C++：vector 增删
来源：http://hz.cashguo.top/gtntnwkkud.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.daria6918.cn/gtprdswsni.html

[S34] C++：遍历 vector
来源：http://hz.c1oappe.top/gtxxmlezcq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtpnrqddfl.html

[S35] C++：map
来源：http://hz.cdnleiting.top/gtjxswhhzq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtuloxuqad.html

[S36] C++：unordered_map
来源：http://hz.wangshuangyany.cn/gtktoolzci.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtdtixwlem.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtevcwaern.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shzxlz.cn/gtkhhpctgh.html

[S38] C++：排序
来源：http://hz.jyoumei.cn/gtolhczlmv.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtdfnetvsj.html

[S39] C++：自定义比较器排序
来源：http://hz.cucudq.cn/gtuojbyltt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtcjuotfni.html

[S40] C++：查找元素
来源：http://hz.svipenyu.cn/gtpwzaotnt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.haohaochexian.top/gtpxnamohx.html

[S41] C++：类与构造函数
来源：http://hz.tanke756.top/gtmbcjeakl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hongshengwenyu.top/gtuhbblgzo.html

[S42] C++：继承与虚函数
来源：http://hz.pengpengdd.cyou/gtnhrfqqkg.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtmlfjdofd.html

[S43] C++：智能指针
来源：http://hz.zhaomingkeji.xyz/gtztinvqgv.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtpbpzblzv.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtjvcnpxxl.html

void inc(int &x) { ++x; }
来源：http://hz.mhx1999.top/gtaizkcwys.html

[S45] C++：lambda
来源：http://hz.redwolf501.top/gtoacwozbh.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtbmbxnnaa.html

[S46] C++：函数模板
来源：http://hz.cqqwz.cn/gtwcyrbmeb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtzepfchuj.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtzaoidgsj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.vqdsnc.cn/gtbfiwygjs.html

[S48] C++：逐行读文件
来源：http://hz.shangyingyoupin.top/gtukbuyqre.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhoulong.xyz/gtxdlujvpb.html

while (std::getline(in, line)) { }
来源：http://hz.gzhubu.top/gtkpeybngy.html

[S49] C++：写文件
来源：http://hz.yueranfly.top/gtqqwckkzw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtudrojvyu.html

[S50] C++：格式化数字
来源：http://hz.daxiang520.top/gtbuwpmcte.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sysykeji.top/gtnhugigru.html

[S51] C++：显式类型转换
来源：http://hz.yj20258888.top/gtxiaofqav.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtrlhfhwwi.html

[S52] C++：const 与 noexcept
来源：http://hz.bjfxy.top/gtafgskrdl.html

int size() const noexcept { return n_; }
来源：http://hz.tanke756.top/gtfbzwxxhu.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangkeji.top/gtorehjywz.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtzgvptrtj.html

[S54] C++：异常处理
来源：http://hz.bjfxy.top/gtjldtyntd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhongyouzk.top/gtutxhtuoq.html

[S55] C++：结构化绑定
来源：http://hz.sxryk.cn/gtifmmlnsb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.iojbl.cn/gtgfxdobcb.html

[S56] C++：optional
来源：http://hz.hnqzz.top/gtlqkdeqpd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hywenlv.cn/gtxrraptea.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtmczadffz.html

constexpr int N = 10;
来源：http://hz.0kj1m.cn/gtbqxzzcvp.html

[S58] C++：命名空间
来源：http://hz.yuanzhike.top/gtyolrsgpe.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtgdkjiaoc.html

[S59] C++：静态断言
来源：http://hz.yanxiufei.cn/gtwzdsufmh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ybcxt.top/gtkciylmki.html

[S60] C++：遍历并删除元素
来源：http://hz.zycfv.cn/gtqytuoazg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhaomingkeji.xyz/gtucdowtrh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtyfijknxt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtpvzbbkit.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgedveosr.html

[T01] Kotlin：Hello World
来源：http://hz.dianchejie.cn/gtvhirblrw.html

println("Hello")
来源：http://hz.yj20258.top/gtaffvbvei.html

[T02] Kotlin：变量
来源：http://hz.kuanghao11.cn/gtgukztihi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ehwqpu.com/gtcwwbzore.html

[T03] Kotlin：字符串模板
来源：http://hz.yuxming.cn/gtdreafltz.html

"值: $b"
来源：http://hz.0kj1m.cn/gtgzfyyrut.html

[T04] Kotlin：空安全
来源：http://hz.yangfankeji.com/gtmkieeiam.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtxunjmxhc.html

[T05] Kotlin：when 表达式
来源：http://hz.jqgufenzy.top/gtbnlkwlsy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhiwuduotai.top/gtkhtdhyjw.html

[T06] Kotlin：集合映射
来源：http://hz.pengpengdd.cyou/gtrjazmmuy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gtxxekavtj.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtaqkykpdf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtzxraszbp.html

[T08] Kotlin：数据类
来源：http://hz.yvedp.cn/gtkvbnhorq.html

data class User(val name: String, val age: Int)
来源：http://hz.fzhhl.top/gtrrgphbps.html

[T09] Kotlin：扩展函数
来源：http://hz.iojbl.cn/gtmydfpkvp.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtydnadtts.html

[T10] Kotlin：默认参数
来源：http://hz.xuanzx.com/gtublzctjv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuetiantiany.cn/gtnuryxykt.html

[T11] Kotlin：协程
来源：http://hz.quarkkingdee.top/gtbzlcotjq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.pycfn.com/gtzekofaop.html

[T12] Kotlin：解构声明
来源：http://hz.wangshuangyany.cn/gtggrmtswi.html

val (a, b) = Pair(1, 2)
来源：http://hz.yongpay.top/gtgzayzqge.html

[T13] Kotlin：只读 Map
来源：http://hz.haohaochexian.top/gtzwpzefyz.html

val m = mapOf("a" to 1)
来源：http://hz.ybcxt.top/gtdwlcoljw.html

[T14] Kotlin：循环
来源：http://hz.xinyue.icu/gtigsrdvkw.html

for (i in 1..10) println(i)
来源：http://hz.yonumen.top/gtpygebbql.html

[T15] Kotlin：接口
来源：http://hz.tian-w.cn/gtemvmnyoj.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gtbjvevylu.html

[T16] Swift：Hello World
来源：http://hz.iojbl.cn/gtatybkaif.html

print("Hello")
来源：http://hz.snrcjt.cn/gtvspukdau.html

[T17] Swift：变量与常量
来源：http://hz.ehwqpu.com/gtlxipjufx.html

var a = 1;  let b = 2
来源：http://hz.mhx1999.top/gtvuqeqyzn.html

[T18] Swift：字符串插值
来源：http://hz.chenlongwang.top/gtrxkrzkkv.html

"值: \(b)"
来源：http://hz.gogol.net.cn/gtekubrxmb.html

[T19] Swift：可选绑定
来源：http://hz.birdmap.top/gtckrvmuhg.html

if let n = opt { print(n) }
来源：http://hz.pengpengdd.cyou/gtluhsfmvg.html

[T20] Swift：数组操作
来源：http://hz.birdmap.top/gtedqirfcj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.gaohongyu789.top/gtfmczryqa.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gtwbxwykma.html

for x in a { print(x) }
来源：http://hz.yj202588.top/gtiocxarix.html

[T22] Swift：字典
来源：http://hz.yj202588.top/gtmkclbnyr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gtunpcwlbn.html

[T23] Swift：函数
来源：http://hz.havefunace.top/gtmkbbnrwf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shzxlz.cn/gtzwwlyqij.html

[T24] Swift：闭包
来源：http://hz.ivvv.top/gtbusujhwo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.nwbrower.top/gtaejsrhal.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gttulndxdv.html

struct P { var x: Int }
来源：http://hz.wangshuangyany.cn/gtmyxndzjg.html

[T26] Swift：类与重写
来源：http://hz.0kj1m.cn/gtyzixekwq.html

class A: Base { override func f() {} }
来源：http://hz.birdmap.top/gtinvukjbu.html

[T27] Swift：错误处理
来源：http://hz.havefunace.top/gtvycdosos.html

do { try f() } catch { print(error) }
来源：http://hz.iojbl.cn/gtcxbfbltt.html

[T28] Swift：枚举
来源：http://hz.zhixingplan.top/gtydkubvpu.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtmioimoqg.html

[T29] Swift：guard 提前返回
来源：http://hz.gotoacloud.top/gtmhziavkk.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtswsxpxbh.html

[T30] Swift：协议
来源：http://hz.hammf.cn/gtqgralper.html

protocol Shape { func area() -> Double }
来源：http://hz.fengsongda.top/gtttzzwini.html

[T31] Lua：Hello World
来源：http://hz.c1oappe.top/gtcmjlbrek.html

print("Hello")
来源：http://hz.jinyuanbaomall.cn/gtvtjjzais.html

[T32] Lua：局部变量
来源：http://hz.dianchejie.cn/gtidlokyfu.html

local a = 1
来源：http://hz.dashuyun.cn/gtyzjrhdhp.html

[T33] Lua：表（数组）
来源：http://hz.xuetiantiany.cn/gtrakghgqp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtuoppvtrq.html

[T34] Lua：遍历表
来源：http://hz.dashuyun.cn/gthebsccml.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.redwolf501.top/gtzqmrfvyg.html

[T35] Lua：字典表
来源：http://hz.jyoumei.cn/gtzqpesofv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.feifeiyinyue.top/gtfdlvkhvp.html

[T36] Lua：函数
来源：http://hz.zhixingplan.top/gteokrikzb.html

function add(a, b) return a + b end
来源：http://hz.fzhhl.top/gtjgbnmvip.html

[T37] Lua：字符串拼接
来源：http://hz.52xcode.cn/gtqdachxbu.html

"a" .. "b"
来源：http://hz.yongpay.top/gtkjvuduii.html

[T38] Lua：条件
来源：http://hz.hnxiangtu.top/gttunggcsd.html

if x > 0 then print("正") end
来源：http://hz.tianlin.xyz/gtfqvkyiua.html

[T39] Lua：模式匹配
来源：http://hz.yangfankeji.com/gtlpvvaqmj.html

string.find(s, "%d+")
来源：http://hz.pengpengdd.cyou/gtlioavisv.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gttsplragy.html

setmetatable({}, { __index = base })
来源：http://hz.fzhhl.top/gtxzczjgfh.html

[T41] Perl：Hello World
来源：http://hz.feifeiyinyue.top/gtonxybnlk.html

print "Hello\n";
来源：http://hz.zhoulong.xyz/gtfudrqfgj.html

[T42] Perl：变量类型
来源：http://hz.cheryme.top/gtaklbnmij.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cucudq.cn/gttyejxjpr.html

[T43] Perl：字符串插值
来源：http://hz.gaohongyu789.top/gtppoiwpnz.html

"值: $a"
来源：http://hz.guannengcc.top/gtwmguwglz.html

[T44] Perl：条件
来源：http://hz.smart0.xyz/gtznlqvpbv.html

if ($a > 0) { print "正"; }
来源：http://hz.xinyue.icu/gtuuxovmvx.html

[T45] Perl：数组遍历
来源：http://hz.zdqjudy.top/gtiqxemjxo.html

for my $x (@arr) { print $x; }
来源：http://hz.smart0.xyz/gtfkzldffa.html

[T46] Perl：哈希操作
来源：http://hz.shzxlz.cn/gttfjkfxnf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sxryk.cn/gtdwprjuyp.html

[T47] Perl：正则捕获
来源：http://hz.hysaishi.cn/gtcmwfgvns.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.gotoacloud.top/gthexgjmou.html

[T48] Perl：正则替换
来源：http://hz.hfpthk.cn/gtbwngccsz.html

$s =~ s/old/new/g;
来源：http://hz.quarkkingdee.top/gteumcdadf.html

[T49] Perl：函数
来源：http://hz.chenlongwang.top/gtiqryqcez.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.xinyue.icu/gtqitbofel.html

[T50] Perl：逐行读文件
来源：http://hz.chenjidiqi.icu/gthzuuxdzy.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.redwolf501.top/gtfvpkanrb.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.xuetiantiany.cn/gtqhtpvgms.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtphezkkdw.html

println("Hello")
来源：http://hz.yueranfly.top/gtnhgeatvg.html

[T52] Scala：变量
来源：http://hz.bjfxy.top/gteoszgutn.html

val a = 1;  var b = 2
来源：http://hz.shzxlz.cn/gtmcgoylie.html

[T53] Scala：字符串插值
来源：http://hz.52xcode.cn/gtyhlnhcuj.html

s"值: $b"
来源：http://hz.xylfe.cn/gtsxonfwnn.html

[T54] Scala：集合映射
来源：http://hz.xingfuxueyuan.xyz/gtluvvjglb.html


<!-- 参考信息 -->