代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gthkbnaeiw.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtarymkyjv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gteugxaqzv.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtjegjcdpz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yanxiufei.cn/gtxkisnlpx.html

[R52] 统计行数
来源：http://hz.nwbrower.top/gtmolljzyd.html

wc -l a.txt
来源：http://hz.zhengqikj.top/gthqgnusrt.html

[R53] 查看文件头与实时尾
来源：http://hz.birdmap.top/gtakqpauxd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtttwvrbso.html

[R54] 比较两个文件
来源：http://hz.zhaomingkeji.xyz/gtvzoowjzm.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtpwcfnqlu.html

[R55] 压缩与解压
来源：http://hz.bjfxy.top/gtobdfdkup.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dashuyun.cn/gtjinetxyj.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtakqsckzu.html

scp file user@host:/path/
来源：http://hz.jqgfzy.top/gtcunrevbu.html

[R57] 远程执行命令
来源：http://hz.zdqjudy.top/gtkngwkmym.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gttpgsqbbh.html

[R58] 下载文件
来源：http://hz.nanxuanxn.top/gtjoqehikr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtspeiyscl.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtomzzipgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtaiiqizys.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gtdzsmqbyu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinghuilouyu.cn/gtwhqeljov.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtlkomyfpd.html

df -h;  du -sh *
来源：http://hz.guannengcc.top/gtzzuyjmtq.html

[R62] 找最占空间的文件
来源：http://hz.jyoumei.cn/gtvrayetea.html

du -ah . | sort -rh | head -10
来源：http://hz.yj20258.top/gtbxgpxqno.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gtmcpdmxuu.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtdhkjbuig.html

[R64] 结束进程
来源：http://hz.jqgfzy.top/gttcieomgx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangdashe.top/gtwmkpsqay.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtbitfjizo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtyamcaexp.html

[R66] 定时任务
来源：http://hz.jqgufenzy.top/gtjdpittki.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gtqdmecuih.html

[R67] 生成随机十六进制串
来源：http://hz.hammf.cn/gtgmgyoaoj.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gtukudxrxg.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtnfjesufv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtmtmrnryx.html

[R69] 生成随机密码
来源：http://hz.zhengqikj.top/gtqdtelizh.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtdviglvzz.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtekqlblty.html

date +%s;  date -d @1700000000
来源：http://hz.iojbl.cn/gtpahswyav.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtcpfxzxne.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtupflwpxd.html

[R72] 等待端口就绪
来源：http://hz.ivvv.top/gtglcpnmcf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtzmgzsywi.html

[R73] 分割大日志
来源：http://hz.ybcxt.top/gtftvrgaug.html

split -l 1000 big.log part_
来源：http://hz.vqdsnc.cn/gtoopysmdo.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtmlljolxc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yvedp.cn/gtxdiuumrz.html

[R75] 导出环境变量
来源：http://hz.havefunace.top/gtmeueznol.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.bjfxy.top/gtpcrfzywy.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtpcyyjdts.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtyibidgrc.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtnuxtjurb.html

read -rp "请输入: " ans
来源：http://hz.yj202588.top/gtxedwalxv.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gthcaxbfib.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zycfv.cn/gtkpuwvehi.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtjijcmyro.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gtjbrpnqie.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtbqhsfcec.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtxrhifyjq.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrotpjrsa.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtjcdteyki.html

================================================================================
来源：http://hz.nwbrower.top/gtjjuojlok.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gtvanexrwq.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtemayvrvn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtpqmjrluz.html

[S02] C：变量与格式化输出
来源：http://hz.smart0.xyz/gtnlfrsxum.html

int a = 10; printf("%d\n", a);
来源：http://hz.snrcjt.cn/gthqgkvljm.html

[S03] C：读入整数
来源：http://hz.dianchejie.cn/gtcvmywnqq.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gtyxqfsrpu.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtyrfpwyla.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtulytwmpi.html

[S05] C：字符串长度
来源：http://hz.yonumen.top/gtiuenuphn.html

strlen(s)
来源：http://hz.tianlin.xyz/gtczgmggay.html

[S06] C：字符串比较
来源：http://hz.xylfe.cn/gtgufiipia.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gtpfhaoyva.html

[S07] C：数组遍历求和
来源：http://hz.hysaishi.cn/gtocytmbcz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtceionsyr.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtqgqwgnxl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtaujquksv.html

[S09] C：结构体定义与初始化
来源：http://hz.xuanzx.com/gtjpouixfe.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtxhohkqfn.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtwyfkymwv.html

int *p = &a;  *p = 5;
来源：http://hz.svipenyu.cn/gtzqunycvh.html

[S11] C：逐行读文件
来源：http://hz.nwbrower.top/gtrxgnevzj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtsksfnmfy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aibaodan.cn/gtzlsqmzhd.html

fclose(f);
来源：http://hz.hfpthk.cn/gtymihqdvs.html

[S12] C：写文件
来源：http://hz.hnqzz.top/gttqllkdfv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.kuanghao11.cn/gtlbzlfqwd.html

[S13] C：宏定义
来源：http://hz.sweek.top/gtelxhojhq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jinghuilouyu.cn/gtprmcorma.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtsshevtyj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtzgdjthmb.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtyrcwgskh.html

(double) a / b
来源：http://hz.shanyushiyangkeji.top/gtbqfogcrd.html

[S16] C：位操作置位
来源：http://hz.316326.xyz/gtrokoymby.html

x |= (1 << 3);
来源：http://hz.meibo888.top/gtyzrfjctd.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtjafpself.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtvpjtarsd.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtmjnkduxt.html

int main(int argc, char **argv)
来源：http://hz.nwbrower.top/gtugonypxl.html

[S19] C：快速排序
来源：http://hz.hammf.cn/gtnqzvsbqw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtbaefbdqh.html

[S20] C：二分查找
来源：http://hz.hammf.cn/gtgwpliwen.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtfawyxukw.html

[S21] C：字符类别判断
来源：http://hz.quarkkingdee.top/gtkymwfvam.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gotoacloud.top/gtctkririq.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtuxqcjksk.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daria6918.cn/gtlilvmaqo.html

[S23] C：随机数
来源：http://hz.svipenyu.cn/gtnutpijgb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258888.top/gtnelrrjns.html

[S24] C：获取本地时间
来源：http://hz.xylfe.cn/gtsqcfndzc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.havefunace.top/gtwusaxdhk.html

[S25] C：内存拷贝
来源：http://hz.yongpay.top/gtblbrluws.html

memcpy(dst, src, n);
来源：http://hz.gotoacloud.top/gtcaxstbfs.html

[S26] C：内存清零
来源：http://hz.zycfv.cn/gtxtmyuqxn.html

memset(a, 0, sizeof a);
来源：http://hz.jinyuanbaomall.cn/gtqtrusjxw.html

[S27] C：定义常量
来源：http://hz.shanyushiyangtech.top/gtbvirbuiu.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtwgfszrks.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtmmmsrvnq.html

static int counter = 0;
来源：http://hz.hammf.cn/gtptguqqlg.html

[S29] C：变参函数
来源：http://hz.nanxinkj.top/gtwxfcetco.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.c1oappe.top/gtuqtmrtem.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gteozzboxl.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtragevjji.html

#define X_H
来源：http://hz.0kj1m.cn/gttvhirdat.html

#endif
来源：http://hz.daxiang520.top/gtbgakfixb.html

[S31] C++：Hello World
来源：http://hz.jiagoushi.top/gtmpmqrbzr.html

#include <iostream>
来源：http://hz.xuetiantiany.cn/gtjdolglrl.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.meibo888.top/gthdvrfbhu.html

[S32] C++：字符串
来源：http://hz.ybcxt.top/gtkptgvwcn.html

std::string s = "hi";  s += "!";
来源：http://hz.ywan-chungtsiang.top/gtnaxhlwrd.html

[S33] C++：vector 增删
来源：http://hz.bjfxy.top/gtlcjehuaz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.snrcjt.cn/gtqrnlcxst.html

[S34] C++：遍历 vector
来源：http://hz.yj202588.top/gtlyvpulac.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtkvbmdmjj.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtzufeudcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtkqjporfo.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gthoeqrqxg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hammf.cn/gtcxajcfhh.html

[S37] C++：set
来源：http://hz.yongpay.top/gthqljgtqw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.meibo888.top/gtlujduflq.html

[S38] C++：排序
来源：http://hz.hnxiangtu.top/gtfcrwkpqp.html

std::sort(v.begin(), v.end());
来源：http://hz.zhongyouzk.top/gtmjybkpmi.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtrllnlbyt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ehwqpu.com/gthvnlbaah.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtvyrfqnui.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jianghu66.top/gtswwhgndg.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtisysornv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xinyue.icu/gtrpbcawoc.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtvwyynbag.html

class B : public Base { public: void f() override {} };
来源：http://hz.ehwqpu.com/gtbivstnzh.html

[S43] C++：智能指针
来源：http://hz.52xcode.cn/gtmsigzqfd.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtkfhjfbmf.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtdkgonglw.html

void inc(int &x) { ++x; }
来源：http://hz.yvedp.cn/gtipcugpmy.html

[S45] C++：lambda
来源：http://hz.ydzc1.top/gtiiijdcib.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yanxiufei.cn/gtyveyyyzc.html

[S46] C++：函数模板
来源：http://hz.daxiang520.top/gtnjvztkqk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtdudwvolu.html

[S47] C++：结构化绑定遍历
来源：http://hz.haohaochexian.top/gtqpmfczxj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hysaishi.cn/gtzzubwtxl.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtzzffvupv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtzsnqkdwn.html

while (std::getline(in, line)) { }
来源：http://hz.ppjwa.cn/gtxcojkirq.html

[S49] C++：写文件
来源：http://hz.daria6918.cn/gtukljgtoe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gtlrvsvcyg.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gtjyszfqmj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtizqglwdv.html

[S51] C++：显式类型转换
来源：http://hz.gotoacloud.top/gtgwglesad.html

static_cast<double>(a) / b
来源：http://hz.redwolf501.top/gturfivhjc.html

[S52] C++：const 与 noexcept
来源：http://hz.svipenyu.cn/gtuybcuund.html

int size() const noexcept { return n_; }
来源：http://hz.hnqzz.top/gtkcfzrtse.html

[S53] C++：移动语义
来源：http://hz.pycfn.com/gtawgqpxbi.html

std::vector<int> w = std::move(v);
来源：http://hz.zhaomingkeji.xyz/gthhkhvpjm.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtnpdghqfl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daxiang520.top/gtecnrrdkq.html

[S55] C++：结构化绑定
来源：http://hz.yj202588.top/gtsdttdvkb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtzndngxry.html

[S56] C++：optional
来源：http://hz.hywenlv.cn/gtryeisefv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.dashuyun.cn/gtwrshomhq.html

[S57] C++：编译期常量
来源：http://hz.kuanghao11.cn/gtgekltwol.html

constexpr int N = 10;
来源：http://hz.jianghu66.top/gtduujcmky.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gttnknjaqe.html

namespace ns { int f() { return 1; } }
来源：http://hz.hnqzz.top/gtcjpkoocm.html

[S59] C++：静态断言
来源：http://hz.yuxming.cn/gtsfmwkofn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gttvaizxmm.html

[S60] C++：遍历并删除元素
来源：http://hz.sufxvd.cn/gtxpmkmypo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.nwbrower.top/gtppckxvpr.html

================================================================================
来源：http://hz.hnqzz.top/gtofrzsbqe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.wangshuangyany.cn/gtoihmphgu.html

================================================================================
来源：http://hz.redwolf501.top/gtwknmzdct.html

[T01] Kotlin：Hello World
来源：http://hz.pycfn.com/gtrgiuqjtb.html

println("Hello")
来源：http://hz.jiagoushi.top/gtjxjzfxpo.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtksufbojo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtlzzoippr.html

[T03] Kotlin：字符串模板
来源：http://hz.ppjwa.cn/gthqbkrcnr.html

"值: $b"
来源：http://hz.316326.xyz/gtgvghpjjj.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtgmeecorz.html

val n: String? = null;  n?.length
来源：http://hz.jinghuilouyu.cn/gtgtlxkyli.html

[T05] Kotlin：when 表达式
来源：http://hz.ppjwa.cn/gtimbmdern.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shangyingyoupin.top/gtgwbrupjc.html

[T06] Kotlin：集合映射
来源：http://hz.52xcode.cn/gtjpefbzfw.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gotoacloud.top/gtmfjfivjd.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigfzy.top/gtbxkraoqb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jqgufenzy.top/gtylcdofxy.html

[T08] Kotlin：数据类
来源：http://hz.nanxuanxn.top/gtiqvckyjp.html

data class User(val name: String, val age: Int)
来源：http://hz.guowangkeji.top/gtpypcwwfi.html

[T09] Kotlin：扩展函数
来源：http://hz.jinqigfzy.top/gtqngxhbwe.html

fun String.exclaim() = this + "!"
来源：http://hz.xingfuxueyuan.xyz/gtcclcudwr.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtqekixvnl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtvhodgois.html

[T11] Kotlin：协程
来源：http://hz.shangyingyoupin.top/gtrjjgdzwg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtfasgmjnz.html

[T12] Kotlin：解构声明
来源：http://hz.vqdsnc.cn/gtqfcuthkf.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gttdhunekp.html

[T13] Kotlin：只读 Map
来源：http://hz.smart0.xyz/gtzkuvammk.html

val m = mapOf("a" to 1)
来源：http://hz.hnqzz.top/gttehafytt.html

[T14] Kotlin：循环
来源：http://hz.andypj.xyz/gtyfzsmuua.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gttugzalwl.html

[T15] Kotlin：接口
来源：http://hz.zhixingplan.top/gtjcjbuuod.html

interface Shape { fun area(): Double }
来源：http://hz.52xcode.cn/gtmspcdplo.html

[T16] Swift：Hello World
来源：http://hz.ivvv.top/gtvbnnqiyv.html

print("Hello")
来源：http://hz.birdmap.top/gtsjvyrcsd.html

[T17] Swift：变量与常量
来源：http://hz.hongshengwenyu.top/gtdchnzdzt.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtknqehpgx.html

[T18] Swift：字符串插值
来源：http://hz.xylfe.cn/gtxnowrphk.html

"值: \(b)"
来源：http://hz.316326.xyz/gtndevbdoj.html

[T19] Swift：可选绑定
来源：http://hz.mhx1999.top/gtpcznakud.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtoymslkpz.html

[T20] Swift：数组操作
来源：http://hz.xziqi.cn/gtkibeezee.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.fengsongda.top/gtlwzexcgx.html

[T21] Swift：遍历
来源：http://hz.jinghuilouyu.cn/gtjrueznjv.html

for x in a { print(x) }
来源：http://hz.hammf.cn/gtcxpqarod.html

[T22] Swift：字典
来源：http://hz.gogol.net.cn/gtdhrgvxij.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtjjkctogf.html

[T23] Swift：函数
来源：http://hz.jinyuanbaomall.cn/gtpkjsriro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ydzc1.top/gthyumumzr.html

[T24] Swift：闭包
来源：http://hz.52xcode.cn/gteglrolcd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yonumen.top/gtbcllqyci.html

[T25] Swift：结构体
来源：http://hz.mhx1999.top/gtznqtdnfo.html

struct P { var x: Int }
来源：http://hz.dashuyun.cn/gtcjqlbhyp.html

[T26] Swift：类与重写
来源：http://hz.redwolf501.top/gtnpkucppf.html

class A: Base { override func f() {} }
来源：http://hz.zhixingplan.top/gtryaegcgj.html

[T27] Swift：错误处理
来源：http://hz.hywenlv.cn/gtnfpufojk.html

do { try f() } catch { print(error) }
来源：http://hz.pycfn.com/gtmpbmvgai.html

[T28] Swift：枚举
来源：http://hz.gaohongyu789.top/gtwzwkuabc.html

enum Color { case red, green }
来源：http://hz.nanxinkj.top/gtbkbatdww.html

[T29] Swift：guard 提前返回
来源：http://hz.jlsjyb.cn/gtgqadydxx.html

guard let x = opt else { return }
来源：http://hz.gzhubu.top/gtjsmmcanl.html

[T30] Swift：协议
来源：http://hz.jianghu66.top/gtazhlarnz.html

protocol Shape { func area() -> Double }
来源：http://hz.xuanzx.com/gtctbspemm.html

[T31] Lua：Hello World
来源：http://hz.jlsjyb.cn/gtvulfszxc.html

print("Hello")
来源：http://hz.chenlongwang.top/gtwigabzvg.html

[T32] Lua：局部变量
来源：http://hz.9152youxi.cn/gtlgaluawx.html

local a = 1
来源：http://hz.cucudq.cn/gtcyckvdnx.html

[T33] Lua：表（数组）
来源：http://hz.cucudq.cn/gthyjvgyxe.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.xziqi.cn/gtuwalikvy.html

[T34] Lua：遍历表
来源：http://hz.mhx1999.top/gtpayuslix.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtirbjitnx.html

[T35] Lua：字典表
来源：http://hz.jlsjyb.cn/gttsddfhgj.html

local d = { a = 1 };  d.b = 2
来源：http://hz.shanyushiyangtech.top/gtzkusklhe.html

[T36] Lua：函数
来源：http://hz.hywenlv.cn/gtmfgddxnc.html

function add(a, b) return a + b end
来源：http://hz.cdnleiting.top/gtjmeavwed.html

[T37] Lua：字符串拼接
来源：http://hz.yanxiufei.cn/gtttlearqm.html

"a" .. "b"
来源：http://hz.zycfv.cn/gtzexheaee.html

[T38] Lua：条件
来源：http://hz.aizwys.cn/gtjmfnpizm.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtwnkqwcqi.html

[T39] Lua：模式匹配
来源：http://hz.jinghuilouyu.cn/gtnebpmkkz.html

string.find(s, "%d+")
来源：http://hz.zhiwuduotai.top/gtvenhrvad.html

[T40] Lua：元表
来源：http://hz.fzhhl.top/gtprcfgnry.html

setmetatable({}, { __index = base })
来源：http://hz.hnqzz.top/gtmhtcnmpg.html

[T41] Perl：Hello World
来源：http://hz.fengsongda.top/gtdyxrtbai.html

print "Hello\n";
来源：http://hz.shanyushiyangkeji.top/gtocslnlbe.html

[T42] Perl：变量类型
来源：http://hz.svipenyu.cn/gtzcvxpxqo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.ybcxt.top/gtrnwvufxb.html

[T43] Perl：字符串插值
来源：http://hz.nwbrower.top/gtzyqclbuw.html

"值: $a"
来源：http://hz.yj20258.top/gtwtlbveiu.html

[T44] Perl：条件
来源：http://hz.hongshengwenyu.top/gtczdrfvob.html

if ($a > 0) { print "正"; }
来源：http://hz.cucudq.cn/gtblcjwpij.html

[T45] Perl：数组遍历
来源：http://hz.zhengqikj.top/gtoqaostoe.html

for my $x (@arr) { print $x; }
来源：http://hz.ppjwa.cn/gtioliakjh.html

[T46] Perl：哈希操作
来源：http://hz.zhijiandao.cn/gttmuxmzrm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.jinqigufen.top/gtnrdcsscq.html

[T47] Perl：正则捕获
来源：http://hz.meibo888.top/gtpdeakygz.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zdqjudy.top/gtfvufnreq.html

[T48] Perl：正则替换
来源：http://hz.jlsjyb.cn/gtouvzchyp.html

$s =~ s/old/new/g;
来源：http://hz.kuanghao11.cn/gtbjshikhs.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gtrqomqsgj.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.yuanzhike.top/gtbtiekcdj.html

[T50] Perl：逐行读文件
来源：http://hz.yongpay.top/gtctfvuqrm.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.iojbl.cn/gtelnvwugy.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.tian-w.cn/gtogqdxcdp.html

[T51] Scala：Hello World
来源：http://hz.hywenlv.cn/gtyyzjfjhk.html

println("Hello")
来源：http://hz.zhaomingkeji.xyz/gtkwbavztv.html

[T52] Scala：变量
来源：http://hz.iojbl.cn/gtqscdeejs.html


<!-- 参考信息 -->