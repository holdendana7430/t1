代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yanxiufei.cn/gtvpbfcktr.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtmwxxzdce.html

awk '{print $1, $3}' a.txt
来源：http://hz.bjfxy.top/gtfmivtrzx.html

[R49] awk 带条件
来源：http://hz.yonumen.top/gtiresowsr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtombmramm.html

[R50] awk 求和
来源：http://hz.yongpay.top/gtyywnkokv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.smart0.xyz/gtgrximwwm.html

[R51] 排序去重取前几
来源：http://hz.wangdashe.top/gtjsgkbjla.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daxiang520.top/gtshpumvmr.html

[R52] 统计行数
来源：http://hz.ydzc1.top/gtdifxrifs.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtnjmsnvzi.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtyasazffi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtquvaawhf.html

[R54] 比较两个文件
来源：http://hz.hnxiangtu.top/gtkiplaqbe.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gteglndqwr.html

[R55] 压缩与解压
来源：http://hz.feifeiyinyue.top/gtwjrtdnea.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shzxlz.cn/gtbzewuzbq.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtifpzpqrq.html

scp file user@host:/path/
来源：http://hz.haohaochexian.top/gtxecpmwzu.html

[R57] 远程执行命令
来源：http://hz.yj20258.top/gthgvbkjet.html

ssh user@host 'uptime'
来源：http://hz.tian-w.cn/gtujjbpbbp.html

[R58] 下载文件
来源：http://hz.hysaishi.cn/gtzbmwezeo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gttjcmezdo.html

[R59] 发 POST JSON
来源：http://hz.fzhhl.top/gtxqusxsrg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.daxiang520.top/gtytvijqeu.html

[R60] 只看 HTTP 状态码
来源：http://hz.jiagoushi.top/gtqwazgsaj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xuetiantiany.cn/gtrkgjxmhw.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtjhcgnwvs.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gthcytabmy.html

[R62] 找最占空间的文件
来源：http://hz.svipenyu.cn/gteevtqjdv.html

du -ah . | sort -rh | head -10
来源：http://hz.yuanzhike.top/gtyunvkgsi.html

[R63] 内存与进程
来源：http://hz.cashguo.top/gtxbdzaygt.html

free -h;  ps aux | grep nginx
来源：http://hz.zhaomingkeji.xyz/gtzxtystmj.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtezgqkgbn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtwdewbvrd.html

[R65] 查看端口占用
来源：http://hz.yj20258888.top/gtizejdzuw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cqqwz.cn/gtyzfuthla.html

[R66] 定时任务
来源：http://hz.nanxinkj.top/gtlzxdefmp.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtdejgfxhm.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtnqzfqpph.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtsugkbmqv.html

[R68] 计算文件校验值
来源：http://hz.jinghuilouyu.cn/gtaldddmgy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.kuanghao11.cn/gtibbzokjq.html

[R69] 生成随机密码
来源：http://hz.jinyuanbaomall.cn/gtpifpwkiu.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtxmdpdyni.html

[R70] 时间戳与互转
来源：http://hz.cucudq.cn/gtptaxvefy.html

date +%s;  date -d @1700000000
来源：http://hz.redwolf501.top/gtrldhzoef.html

[R71] 日期格式化
来源：http://hz.shanyushiyangtech.top/gtjbovweck.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtpxrapmdq.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtbuxckfkv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtokqlhgfw.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtzsdrxroe.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtpaduxvzp.html

[R74] 批量重命名
来源：http://hz.haohaochexian.top/gtyxxccpco.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tian-w.cn/gtspxlhtfa.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtaojezbjf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtnvbomokk.html

[R76] 使用临时文件
来源：http://hz.jyoumei.cn/gtoallgrjj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtwttenizw.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtxwxbrupy.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtqzgnhkap.html

[R78] 交互式菜单
来源：http://hz.ybcxt.top/gtgpuawcyb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.gzhubu.top/gthtwxdptn.html

[R79] 解析命令行选项
来源：http://hz.shangyingyoupin.top/gtjtskjwon.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hnqzz.top/gtemyzokhb.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtzquafelw.html

time ./run.sh
来源：http://hz.xingfuxueyuan.xyz/gtehzrcdzz.html

================================================================================
来源：http://hz.52xcode.cn/gtsdmakbva.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtvvwnxugj.html

================================================================================
来源：http://hz.xuanzx.com/gtgvkcjokf.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gttbabsrva.html

#include <stdio.h>
来源：http://hz.yvedp.cn/gtqpyycctr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sxryk.cn/gtujsamapo.html

[S02] C：变量与格式化输出
来源：http://hz.dianchejie.cn/gterndtoua.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gtwdygnkns.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtzghzvbhi.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtoiydeasp.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtkvyspsqz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtfwogarlo.html

[S05] C：字符串长度
来源：http://hz.ehwqpu.com/gtdawnjgab.html

strlen(s)
来源：http://hz.ppjwa.cn/gtwoywcwnr.html

[S06] C：字符串比较
来源：http://hz.hfpthk.cn/gtdimtwigb.html

strcmp(a, b) == 0
来源：http://hz.jinyuanbaomall.cn/gtsggvlxrb.html

[S07] C：数组遍历求和
来源：http://hz.mhx1999.top/gtqevmhlgl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtrbussjox.html

[S08] C：动态内存分配与释放
来源：http://hz.ppjwa.cn/gtvficmbrc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cucudq.cn/gtfymodyns.html

[S09] C：结构体定义与初始化
来源：http://hz.ehwqpu.com/gtvlulofcm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hnxiangtu.top/gtgcknvabq.html

[S10] C：指针与解引用
来源：http://hz.tianlin.xyz/gtidwuqwti.html

int *p = &a;  *p = 5;
来源：http://hz.iojbl.cn/gtkqryzruo.html

[S11] C：逐行读文件
来源：http://hz.cheryme.top/gtjanluxxq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinyuanbaomall.cn/gtbmuebbrl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtpvxzyzln.html

fclose(f);
来源：http://hz.svipenyu.cn/gtvbtxwvjm.html

[S12] C：写文件
来源：http://hz.zhoulong.xyz/gtqipcdjor.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinghuilouyu.cn/gtsqjkkpgx.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtfyxnzedx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtubtshmax.html

[S14] C：枚举
来源：http://hz.xuetiantiany.cn/gtowixwrxu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dianchejie.cn/gtjxjlyxle.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtierkoqah.html

(double) a / b
来源：http://hz.gogol.net.cn/gtnjinkemb.html

[S16] C：位操作置位
来源：http://hz.wangshuangyany.cn/gtcfihkmlm.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gtyfvrtvtr.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtdxvltxyy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sxryk.cn/gtwsqeoiyk.html

[S18] C：命令行参数
来源：http://hz.andypj.xyz/gtrgfwmqzy.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtexbomqyo.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtzpvtkqey.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtoshsnxpj.html

[S20] C：二分查找
来源：http://hz.kuanghao11.cn/gtftbqemvq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pengpengdd.cyou/gturolxwwi.html

[S21] C：字符类别判断
来源：http://hz.zhengqikj.top/gtkjrhenzm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtwouzjzhz.html

[S22] C：字符串转数字
来源：http://hz.iojbl.cn/gtpqrdahrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhoulong.xyz/gtgcgyplyg.html

[S23] C：随机数
来源：http://hz.shanyushiyangkeji.top/gtzyjfzodn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtgtbrdtmc.html

[S24] C：获取本地时间
来源：http://hz.vqdsnc.cn/gtdycekpew.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.316326.xyz/gtoawhxaqt.html

[S25] C：内存拷贝
来源：http://hz.ivvv.top/gtliksokfi.html

memcpy(dst, src, n);
来源：http://hz.ydjk.org.cn/gtbtrzxlvb.html

[S26] C：内存清零
来源：http://hz.yj202588.top/gttbkdazpp.html

memset(a, 0, sizeof a);
来源：http://hz.hysaishi.cn/gtxmtsmksz.html

[S27] C：定义常量
来源：http://hz.yj202588.top/gtauaogllg.html

const double PI = 3.14159;
来源：http://hz.cucudq.cn/gtolhhobbu.html

[S28] C：静态变量
来源：http://hz.xingfuxueyuan.xyz/gthzusuyip.html

static int counter = 0;
来源：http://hz.cqqwz.cn/gtwdzxtrlt.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtodwxfusd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gthxypzivg.html

[S30] C：头文件保护
来源：http://hz.snrcjt.cn/gtpwzdhqxq.html

#ifndef X_H
来源：http://hz.chenlongwang.top/gtmlvnptkt.html

#define X_H
来源：http://hz.daria6918.cn/gtvzfiyqto.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtwplwzwqn.html

[S31] C++：Hello World
来源：http://hz.quarkkingdee.top/gtrhnggdsc.html

#include <iostream>
来源：http://hz.hywenlv.cn/gtvfzjjbas.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jqgfzy.top/gttqzjxifn.html

[S32] C++：字符串
来源：http://hz.gzhubu.top/gtfbaxxnck.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtgqdvisji.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtfqvqcyev.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtppjtbrxt.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtomqhhkmk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtunylzpfi.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtfgxoknkt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtqxxggdzs.html

[S36] C++：unordered_map
来源：http://hz.andypj.xyz/gtdsnxmivg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtulyofsee.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtdulajzbn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ehwqpu.com/gtmhdwlbyz.html

[S38] C++：排序
来源：http://hz.yuxming.cn/gtiqcdmmqi.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtusfszyct.html

[S39] C++：自定义比较器排序
来源：http://hz.shzxlz.cn/gtbmdqrsuk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gtiahvxdtu.html

[S40] C++：查找元素
来源：http://hz.bjfxy.top/gtooldwasx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shangyingyoupin.top/gthewiadfk.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtawtsywdj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtyazxjqda.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtxeurqjun.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtgvxlorpa.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gthdgdoarj.html

auto p = std::make_unique<int>(5);
来源：http://hz.cucudq.cn/gtdmmdwugt.html

[S44] C++：引用传参
来源：http://hz.gzhubu.top/gtfdlelaek.html

void inc(int &x) { ++x; }
来源：http://hz.ybcxt.top/gtpgoovdwk.html

[S45] C++：lambda
来源：http://hz.0kj1m.cn/gtgelrcfjc.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.316326.xyz/gtfncudhah.html

[S46] C++：函数模板
来源：http://hz.ywan-chungtsiang.top/gtczhibyov.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxuanxn.top/gtswglxhld.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtmqlvinhr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuanzx.com/gttfrhmjkm.html

[S48] C++：逐行读文件
来源：http://hz.hysaishi.cn/gtxrbeasom.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtehzpexgi.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtpjbfutqm.html

[S49] C++：写文件
来源：http://hz.shanyushiyangkeji.top/gtpicyvgut.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtkloxpjyj.html

[S50] C++：格式化数字
来源：http://hz.jinyuanbaomall.cn/gthgwguswf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gtyxesqfbt.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gthgyjrfkd.html

static_cast<double>(a) / b
来源：http://hz.gotoacloud.top/gtayvofghh.html

[S52] C++：const 与 noexcept
来源：http://hz.daria6918.cn/gtzxnnadaa.html

int size() const noexcept { return n_; }
来源：http://hz.jinyuanbaomall.cn/gtqskdkbxt.html

[S53] C++：移动语义
来源：http://hz.yj202588.top/gtvhejykim.html

std::vector<int> w = std::move(v);
来源：http://hz.yuxming.cn/gtlazvdgla.html

[S54] C++：异常处理
来源：http://hz.yueranfly.top/gtnhgppcrv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtqtghmdni.html

[S55] C++：结构化绑定
来源：http://hz.yuanzhike.top/gtvdhxlkug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.9152youxi.cn/gtaghrnfdm.html

[S56] C++：optional
来源：http://hz.aizwys.cn/gtonisdnok.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinqigfzy.top/gtldxrbkfm.html

[S57] C++：编译期常量
来源：http://hz.fengsongda.top/gtkhgozrkd.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtospojzka.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtrbzncpjv.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxinkj.top/gtjlfkajnu.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtwcrpomly.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fengsongda.top/gtfmmguiwa.html

[S60] C++：遍历并删除元素
来源：http://hz.sxryk.cn/gtegoiexkb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guowangkeji.top/gthybzfnlz.html

================================================================================
来源：http://hz.smart0.xyz/gttqqxlwfq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtglphxqcy.html

================================================================================
来源：http://hz.yonumen.top/gtfvdsugco.html

[T01] Kotlin：Hello World
来源：http://hz.vqdsnc.cn/gtmqutlxiw.html

println("Hello")
来源：http://hz.mhx1999.top/gtpniqhfee.html

[T02] Kotlin：变量
来源：http://hz.ydzc1.top/gtwlzvoqws.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtexxailzc.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtngfvmtwt.html

"值: $b"
来源：http://hz.xinyue.icu/gtetnawulp.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gttothusti.html

val n: String? = null;  n?.length
来源：http://hz.daria6918.cn/gtfzsxbqql.html

[T05] Kotlin：when 表达式
来源：http://hz.ydzc1.top/gtapuaikhx.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtfcnjthct.html

[T06] Kotlin：集合映射
来源：http://hz.jqgfzy.top/gttfoksvif.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sufxvd.cn/gtywrzukln.html

[T07] Kotlin：集合过滤
来源：http://hz.shuidangran.top/gtwlfhimil.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cqqwz.cn/gtreutgblo.html

[T08] Kotlin：数据类
来源：http://hz.gogol.net.cn/gthylufsqa.html

data class User(val name: String, val age: Int)
来源：http://hz.shzxlz.cn/gtjxwjhldz.html

[T09] Kotlin：扩展函数
来源：http://hz.cdnleiting.top/gtuyirexhy.html

fun String.exclaim() = this + "!"
来源：http://hz.chenlongwang.top/gtpbthqfeq.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtbctvtsas.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtgvylscgj.html

[T11] Kotlin：协程
来源：http://hz.chenlongwang.top/gtszggfkih.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtwlmmhqrs.html

[T12] Kotlin：解构声明
来源：http://hz.yanxiufei.cn/gtpykodprr.html

val (a, b) = Pair(1, 2)
来源：http://hz.aibaodan.cn/gtsugnwlrq.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtfgntghgz.html

val m = mapOf("a" to 1)
来源：http://hz.xuanzx.com/gtrdbfkndn.html

[T14] Kotlin：循环
来源：http://hz.hongshengwenyu.top/gtfhvxklwu.html

for (i in 1..10) println(i)
来源：http://hz.yanxiufei.cn/gtqjyaaywb.html

[T15] Kotlin：接口
来源：http://hz.tanke756.top/gtwvpyeqmc.html

interface Shape { fun area(): Double }
来源：http://hz.jinghuilouyu.cn/gtbrfgzufc.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtikxnbais.html

print("Hello")
来源：http://hz.cheryme.top/gtolwxapnf.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtqwuwmohh.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gtiwcdhagz.html

[T18] Swift：字符串插值
来源：http://hz.sxryk.cn/gtnpijuviv.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtlfwusnwk.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtcnmikvtp.html

if let n = opt { print(n) }
来源：http://hz.shangyingyoupin.top/gtuntjwlju.html

[T20] Swift：数组操作
来源：http://hz.yvedp.cn/gtrgmmdssj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.haohaochexian.top/gtoxmycudk.html

[T21] Swift：遍历
来源：http://hz.yj202588.top/gtasriyugt.html

for x in a { print(x) }
来源：http://hz.gaohongyu789.top/gtmtxvlbuc.html

[T22] Swift：字典
来源：http://hz.316326.xyz/gtztamuhsx.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.c1oappe.top/gtwegsrzht.html

[T23] Swift：函数
来源：http://hz.feifeiyinyue.top/gtlhyutoyd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtwuwapyuv.html

[T24] Swift：闭包
来源：http://hz.yueranfly.top/gtxceibcke.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zdqjudy.top/gtgtzrrraf.html

[T25] Swift：结构体
来源：http://hz.snrcjt.cn/gtwdkgprpr.html

struct P { var x: Int }
来源：http://hz.meibo888.top/gtjizdqxqx.html

[T26] Swift：类与重写
来源：http://hz.hysaishi.cn/gtdfzpghkc.html

class A: Base { override func f() {} }
来源：http://hz.redwolf501.top/gtzenrzpmu.html

[T27] Swift：错误处理
来源：http://hz.pengpengdd.cyou/gtofzuxmps.html

do { try f() } catch { print(error) }
来源：http://hz.gotoacloud.top/gtjteqldgr.html

[T28] Swift：枚举
来源：http://hz.nanxinkj.top/gtudlpztjy.html

enum Color { case red, green }
来源：http://hz.chenzaomai.com/gtehzqxqzd.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtycxzlvdf.html

guard let x = opt else { return }
来源：http://hz.feifeiyinyue.top/gtlhebxauz.html

[T30] Swift：协议
来源：http://hz.dianchejie.cn/gtwkkbrybf.html

protocol Shape { func area() -> Double }
来源：http://hz.pycfn.com/gtdmedijmw.html

[T31] Lua：Hello World
来源：http://hz.shangyingyoupin.top/gtlrtqnqck.html

print("Hello")
来源：http://hz.dianchejie.cn/gtsbqfkvjn.html

[T32] Lua：局部变量
来源：http://hz.gzhubu.top/gtesyvobmu.html

local a = 1
来源：http://hz.zhijiandao.cn/gtpgpkujoi.html

[T33] Lua：表（数组）
来源：http://hz.xuanzx.com/gtbsmykead.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtmtnzhvqg.html

[T34] Lua：遍历表
来源：http://hz.cdnleiting.top/gtmyosnwmi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtzxdttpkk.html

[T35] Lua：字典表
来源：http://hz.chenlongwang.top/gtumbqzhyc.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yanxiufei.cn/gtzxvqlfby.html

[T36] Lua：函数
来源：http://hz.ywan-chungtsiang.top/gtxqrmmlmo.html

function add(a, b) return a + b end
来源：http://hz.pycfn.com/gtxgizjezu.html

[T37] Lua：字符串拼接
来源：http://hz.wangdashe.top/gtxsjlttmy.html

"a" .. "b"
来源：http://hz.feifeiyinyue.top/gtekdgebps.html

[T38] Lua：条件
来源：http://hz.52xcode.cn/gtpctirfiq.html

if x > 0 then print("正") end
来源：http://hz.shzxlz.cn/gtycstroje.html

[T39] Lua：模式匹配
来源：http://hz.yj20258.top/gtgxmldfny.html

string.find(s, "%d+")
来源：http://hz.feifeiyinyue.top/gtbjmlfppo.html

[T40] Lua：元表
来源：http://hz.snrcjt.cn/gtkutrfdpj.html

setmetatable({}, { __index = base })
来源：http://hz.jqgufenzy.top/gtbucpfokc.html

[T41] Perl：Hello World
来源：http://hz.hongshengwenyu.top/gtrkuhrcaz.html

print "Hello\n";
来源：http://hz.zhijiandao.cn/gtuxcqscim.html

[T42] Perl：变量类型
来源：http://hz.yueranfly.top/gtpqsjqysv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtygzymrxy.html

[T43] Perl：字符串插值
来源：http://hz.cqqwz.cn/gtflrnrukj.html

"值: $a"
来源：http://hz.fzhhl.top/gtnqsrtylc.html

[T44] Perl：条件
来源：http://hz.wangshuangyany.cn/gtiyhryyxd.html

if ($a > 0) { print "正"; }
来源：http://hz.9152youxi.cn/gtowgasxkd.html

[T45] Perl：数组遍历
来源：http://hz.wangdashe.top/gtmlleyfix.html

for my $x (@arr) { print $x; }
来源：http://hz.mhx1999.top/gtyhandjvh.html

[T46] Perl：哈希操作
来源：http://hz.jqgfzy.top/gtkloihijt.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.zhongyouzk.top/gtzthsktck.html

[T47] Perl：正则捕获
来源：http://hz.sufxvd.cn/gtetiyftgx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.zhiwuduotai.top/gttuyfdxoi.html

[T48] Perl：正则替换
来源：http://hz.yuxming.cn/gtnukteknr.html

$s =~ s/old/new/g;
来源：http://hz.nwbrower.top/gtpcokezrd.html

[T49] Perl：函数
来源：http://hz.jinyuanbaomall.cn/gtpkfwmyqg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shuidangran.top/gtfvtstfmo.html

[T50] Perl：逐行读文件
来源：http://hz.jqgfzy.top/gthzfhcfht.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yuxming.cn/gtyduruycw.html


<!-- 参考信息 -->