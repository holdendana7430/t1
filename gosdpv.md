代发 wailian999

cmd >/dev/null 2>&1
来源：http://hz.ybcxt.top/gtlhyenttf.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtseysvrdo.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtuyvlcrbw.html

[R43] 按名字查找文件
来源：http://hz.jlsjyb.cn/gtfnqdkrqf.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtnlwmmkbw.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtiaqphwta.html

find . -mtime -7 -type f
来源：http://hz.zhiwuduotai.top/gtledeojid.html

[R45] 批量删除
来源：http://hz.jiagoushi.top/gtfnloiohv.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtnxrwzyxu.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtgjqrfxtj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.haohaochexian.top/gtovgjljyg.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtltroabcg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.316326.xyz/gtcictxmia.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gtdlxzrcji.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangdashe.top/gtpakkpgwk.html

[R49] awk 带条件
来源：http://hz.yj202588.top/gtwsmwkzmt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.meibo888.top/gtqroujqbf.html

[R50] awk 求和
来源：http://hz.xziqi.cn/gtbanzleyg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gtmdokctfo.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gttkoswrte.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj202588.top/gtlluvekag.html

[R52] 统计行数
来源：http://hz.yonumen.top/gtqsusrmyi.html

wc -l a.txt
来源：http://hz.zhixingplan.top/gtrinpwghd.html

[R53] 查看文件头与实时尾
来源：http://hz.jianghu66.top/gtkpbzlphi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhaomingkeji.xyz/gteblvhama.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gtpfurbrff.html

diff a.txt b.txt
来源：http://hz.mhx1999.top/gttpwnzlna.html

[R55] 压缩与解压
来源：http://hz.nanxinkj.top/gtwwijikba.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ppjwa.cn/gttrfsrzba.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gtncoremhm.html

scp file user@host:/path/
来源：http://hz.chenjidiqi.icu/gtdszjbwpo.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gtmfockmin.html

ssh user@host 'uptime'
来源：http://hz.sweek.top/gtxfhyveia.html

[R58] 下载文件
来源：http://hz.snrcjt.cn/gtyqtnhfjb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gthhicsysc.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtjqkpdbtz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.feifeiyinyue.top/gthyxlgtrj.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtcgpqbfri.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fzhhl.top/gtyeuplguk.html

[R61] 磁盘占用
来源：http://hz.hywenlv.cn/gtapsumikc.html

df -h;  du -sh *
来源：http://hz.hnqzz.top/gtksyaojoj.html

[R62] 找最占空间的文件
来源：http://hz.zhaomingkeji.xyz/gtadvzodmq.html

du -ah . | sort -rh | head -10
来源：http://hz.xylfe.cn/gtxlsbxuoo.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtchigdgjr.html

free -h;  ps aux | grep nginx
来源：http://hz.kuanghao11.cn/gtikrmkvvp.html

[R64] 结束进程
来源：http://hz.guowangkeji.top/gtaeoqueas.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yonumen.top/gtsuuqcenn.html

[R65] 查看端口占用
来源：http://hz.zhijiandao.cn/gtgjlhtjni.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gteddpiqwc.html

[R66] 定时任务
来源：http://hz.zhoulong.xyz/gtrnupjmdt.html

crontab -e;  crontab -l
来源：http://hz.sufxvd.cn/gtlhjxhynt.html

[R67] 生成随机十六进制串
来源：http://hz.svipenyu.cn/gtyfvgkgww.html

openssl rand -hex 16
来源：http://hz.sxryk.cn/gtvbnazwwa.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtdezgqryt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtmhyzpjmt.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtklxblzem.html

head -c 16 /dev/urandom | base64
来源：http://hz.snrcjt.cn/gtrmuqmthb.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtbyeudsmn.html

date +%s;  date -d @1700000000
来源：http://hz.pycfn.com/gtrhzcoxqy.html

[R71] 日期格式化
来源：http://hz.jinyuanbaomall.cn/gtgkomnmiu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtqpslvekk.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtpccuhazk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ppjwa.cn/gtieavjrrc.html

[R73] 分割大日志
来源：http://hz.yuxming.cn/gtegsrbfac.html

split -l 1000 big.log part_
来源：http://hz.cqqwz.cn/gtitdegkmp.html

[R74] 批量重命名
来源：http://hz.gaohongyu789.top/gthgmkgxpa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.haohaochexian.top/gtmznvphmf.html

[R75] 导出环境变量
来源：http://hz.iojbl.cn/gtwpncghfc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtgycgkajf.html

[R76] 使用临时文件
来源：http://hz.jinqigufen.top/gtucfxpxww.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtirjsohlj.html

[R77] 读取用户输入
来源：http://hz.tanke756.top/gtvjtuucys.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtakybfbyg.html

[R78] 交互式菜单
来源：http://hz.daxiang520.top/gtzsriqkrx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cheryme.top/gtffcecvky.html

[R79] 解析命令行选项
来源：http://hz.meibo888.top/gtpxsysmhy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtrkjefdbo.html

[R80] 查看脚本执行耗时
来源：http://hz.hysaishi.cn/gtpqhrkngk.html

time ./run.sh
来源：http://hz.gogol.net.cn/gtiifucblc.html

================================================================================
来源：http://hz.xinyue.icu/gtetsjxtnl.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gthcrymiok.html

================================================================================
来源：http://hz.cheryme.top/gtarqkbjui.html

[S01] C：Hello World
来源：http://hz.jianghu66.top/gtmoatfadj.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtpiexbufh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cdnleiting.top/gtbwgsdyuo.html

[S02] C：变量与格式化输出
来源：http://hz.yangfankeji.com/gtskuzrsen.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenjidiqi.icu/gtiqekzjno.html

[S03] C：读入整数
来源：http://hz.shuidangran.top/gtejpnvwry.html

int x; scanf("%d", &x);
来源：http://hz.zhongyouzk.top/gttawdpqwa.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtdygfoewc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtobhepblf.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gtmhslxsuh.html

strlen(s)
来源：http://hz.9152youxi.cn/gtgthiimnx.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtqsxypzym.html

strcmp(a, b) == 0
来源：http://hz.mhx1999.top/gtqnjaqnlg.html

[S07] C：数组遍历求和
来源：http://hz.zhongyouzk.top/gtdntusaqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.guowangkeji.top/gtqzgopqjg.html

[S08] C：动态内存分配与释放
来源：http://hz.pycfn.com/gtfjocjoyh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.aizwys.cn/gtyiruyltj.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtgvfkrhlb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ywan-chungtsiang.top/gtgrxjtkci.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtmskoshvc.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtsqjdjyxf.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtxsdukcro.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtlpfgmvnj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.guowangkeji.top/gtaoqoszon.html

fclose(f);
来源：http://hz.jinghuilouyu.cn/gtoqgpmcwy.html

[S12] C：写文件
来源：http://hz.dashuyun.cn/gtqeypgzqy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtyxmahmsf.html

[S13] C：宏定义
来源：http://hz.zhixingplan.top/gtdexatyqd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtjhtimeux.html

[S14] C：枚举
来源：http://hz.sweek.top/gtomohyskx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtnavuqxcu.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gthxlrcspj.html

(double) a / b
来源：http://hz.hysaishi.cn/gttpstykyv.html

[S16] C：位操作置位
来源：http://hz.zhiwuduotai.top/gtrqkubhzl.html

x |= (1 << 3);
来源：http://hz.xuanzx.com/gtlvptcwwa.html

[S17] C：安全拼接字符串
来源：http://hz.pengpengdd.cyou/gtwhdvajuu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yuanzhike.top/gthrcededu.html

[S18] C：命令行参数
来源：http://hz.tanke756.top/gtxihzjlwk.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtvzbamsyf.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtzpbopptu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtazuhvlva.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtrtjxpqfp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtolvtlhcs.html

[S21] C：字符类别判断
来源：http://hz.cucudq.cn/gtcnumefhj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhoulong.xyz/gtclcplvcj.html

[S22] C：字符串转数字
来源：http://hz.daxiang520.top/gtmndhhksn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtfruroxuf.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtfjobkcib.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.c1oappe.top/gtfcmswtem.html

[S24] C：获取本地时间
来源：http://hz.sweek.top/gtydrpdppw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jyoumei.cn/gtcotexacz.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtdasdrwfp.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtlmcfmaeb.html

[S26] C：内存清零
来源：http://hz.zhongyouzk.top/gtdgzacwte.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtkbhlucvb.html

[S27] C：定义常量
来源：http://hz.cucudq.cn/gtogdismtx.html

const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtvxsfkmgm.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtqzdjvzdo.html

static int counter = 0;
来源：http://hz.daxiang520.top/gtavqimonc.html

[S29] C：变参函数
来源：http://hz.daxiang520.top/gtywmjhxug.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtnudyfimz.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gtfketydsd.html

#ifndef X_H
来源：http://hz.jinyuanbaomall.cn/gtkctwztct.html

#define X_H
来源：http://hz.0kj1m.cn/gtalbmkkus.html

#endif
来源：http://hz.gaohongyu789.top/gtjocleqkf.html

[S31] C++：Hello World
来源：http://hz.zhiwuduotai.top/gtrbshvqpj.html

#include <iostream>
来源：http://hz.bjfxy.top/gtknqurrgj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gotoacloud.top/gtwjgafams.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gtzbkepwgs.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtglrqdxfm.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gtsmjquzqr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhengqikj.top/gtpnnthefm.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtiagahffo.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.svipenyu.cn/gtjgvisadz.html

[S35] C++：map
来源：http://hz.meibo888.top/gtypvjxqyp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yvedp.cn/gtlxenjkjp.html

[S36] C++：unordered_map
来源：http://hz.sxryk.cn/gtehreedvz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jianghu66.top/gtgqvnobbx.html

[S37] C++：set
来源：http://hz.9152youxi.cn/gtjqezhmvl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shangyingyoupin.top/gteaoppqal.html

[S38] C++：排序
来源：http://hz.gaohongyu789.top/gtsuaayjmd.html

std::sort(v.begin(), v.end());
来源：http://hz.zhixingplan.top/gthjpepkvm.html

[S39] C++：自定义比较器排序
来源：http://hz.ybcxt.top/gtmirebjfi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zycfv.cn/gthgswvtvl.html

[S40] C++：查找元素
来源：http://hz.gzhubu.top/gtnrpssvlg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhengqikj.top/gtguswknxd.html

[S41] C++：类与构造函数
来源：http://hz.sufxvd.cn/gtnqtuqcwa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yangfankeji.com/gtyvgtadze.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtvrlarxme.html

class B : public Base { public: void f() override {} };
来源：http://hz.kuanghao11.cn/gtmvumxtzl.html

[S43] C++：智能指针
来源：http://hz.xinyue.icu/gtwyrnuplg.html

auto p = std::make_unique<int>(5);
来源：http://hz.jiagoushi.top/gtywlayixh.html

[S44] C++：引用传参
来源：http://hz.xingfuxueyuan.xyz/gtbkzncdzd.html

void inc(int &x) { ++x; }
来源：http://hz.hammf.cn/gttbswdpot.html

[S45] C++：lambda
来源：http://hz.sufxvd.cn/gtfrvfjzgm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cashguo.top/gtnurwfqrk.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtolysqguj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.pengpengdd.cyou/gtamjbgops.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtojotaxve.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yvedp.cn/gtmpsfxvwl.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gteirbuvyn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yangfankeji.com/gtlphbsnfi.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtiitgeooi.html

[S49] C++：写文件
来源：http://hz.hnqzz.top/gtgqitresy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenjidiqi.icu/gtgtfbqfke.html

[S50] C++：格式化数字
来源：http://hz.shangyingyoupin.top/gtwceobzyd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ppjwa.cn/gtxqwxwxwy.html

[S51] C++：显式类型转换
来源：http://hz.andypj.xyz/gtjdgcvlrs.html

static_cast<double>(a) / b
来源：http://hz.vqdsnc.cn/gtzhythmcz.html

[S52] C++：const 与 noexcept
来源：http://hz.meibo888.top/gtwcuqjprx.html

int size() const noexcept { return n_; }
来源：http://hz.dashuyun.cn/gtqqrdqdyg.html

[S53] C++：移动语义
来源：http://hz.yj20258888.top/gtkrzycdad.html

std::vector<int> w = std::move(v);
来源：http://hz.zhijiandao.cn/gtmgfwttzr.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtzokspzbi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.vqdsnc.cn/gtvsvkpoon.html

[S55] C++：结构化绑定
来源：http://hz.chenlongwang.top/gtsiwjqvhh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gotoacloud.top/gtribggsor.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtorsnqcfm.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gthhvvzbvh.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtrlpnofzm.html

constexpr int N = 10;
来源：http://hz.jinghuilouyu.cn/gtyjzegkxx.html

[S58] C++：命名空间
来源：http://hz.yonumen.top/gtlikbuswp.html

namespace ns { int f() { return 1; } }
来源：http://hz.svipenyu.cn/gtdoixuhgn.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtqywkmwpg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtxrppbhcn.html

[S60] C++：遍历并删除元素
来源：http://hz.ydzc1.top/gtidwosayv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.haohaochexian.top/gtlizzpxwf.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtvggrrqlb.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gtswrsdjte.html

================================================================================
来源：http://hz.cucudq.cn/gtkhbiqpqb.html

[T01] Kotlin：Hello World
来源：http://hz.cdnleiting.top/gtzbvhszxb.html

println("Hello")
来源：http://hz.havefunace.top/gtyvlgcxgr.html

[T02] Kotlin：变量
来源：http://hz.daria6918.cn/gtbouitiln.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gtzohppwxz.html

[T03] Kotlin：字符串模板
来源：http://hz.yanxiufei.cn/gtvsfmmaup.html

"值: $b"
来源：http://hz.jinqigufen.top/gthfakzqtx.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gtnymxrgtm.html

val n: String? = null;  n?.length
来源：http://hz.ywan-chungtsiang.top/gtbecygckw.html

[T05] Kotlin：when 表达式
来源：http://hz.shanyushiyangkeji.top/gttdouadja.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jlsjyb.cn/gtixeejihg.html

[T06] Kotlin：集合映射
来源：http://hz.cdnleiting.top/gtqevlaucl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtvabgbotc.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtrypbsfdf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nanxuanxn.top/gtoslzazrc.html

[T08] Kotlin：数据类
来源：http://hz.zhoulong.xyz/gtxupbgibg.html

data class User(val name: String, val age: Int)
来源：http://hz.hywenlv.cn/gtvvgpbjjx.html

[T09] Kotlin：扩展函数
来源：http://hz.sysykeji.top/gtextcpude.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgufenzy.top/gtcsbnxwpx.html

[T10] Kotlin：默认参数
来源：http://hz.gaohongyu789.top/gtlrumcrpe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.guannengcc.top/gtaeodwpwh.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtyuijjtjb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.bjfxy.top/gtqmgxhutd.html

[T12] Kotlin：解构声明
来源：http://hz.zdqjudy.top/gtipznbdgl.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtviwxepbe.html

[T13] Kotlin：只读 Map
来源：http://hz.jinyuanbaomall.cn/gtyzsediuc.html

val m = mapOf("a" to 1)
来源：http://hz.andypj.xyz/gtdindyzxf.html

[T14] Kotlin：循环
来源：http://hz.hnqzz.top/gtniyfdjim.html

for (i in 1..10) println(i)
来源：http://hz.hysaishi.cn/gtkfccgqyq.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtzxvfnvwp.html

interface Shape { fun area(): Double }
来源：http://hz.yuanzhike.top/gtfucdwbrk.html

[T16] Swift：Hello World
来源：http://hz.yanxiufei.cn/gtvzrgkeah.html

print("Hello")
来源：http://hz.pycfn.com/gtylmqzwos.html

[T17] Swift：变量与常量
来源：http://hz.jiagoushi.top/gtaexnhxhp.html

var a = 1;  let b = 2
来源：http://hz.jinghuilouyu.cn/gteocxeuvz.html

[T18] Swift：字符串插值
来源：http://hz.tianlin.xyz/gtglczneeg.html

"值: \(b)"
来源：http://hz.svipenyu.cn/gtspntxtdb.html

[T19] Swift：可选绑定
来源：http://hz.zhijiandao.cn/gttgphueow.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtevkczhzw.html

[T20] Swift：数组操作
来源：http://hz.shangyingyoupin.top/gtpkgizrwc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ywan-chungtsiang.top/gttbkqekys.html

[T21] Swift：遍历
来源：http://hz.nwbrower.top/gtqvvhlgwq.html

for x in a { print(x) }
来源：http://hz.yongpay.top/gtfitccvum.html

[T22] Swift：字典
来源：http://hz.sufxvd.cn/gtotajddlh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinqigfzy.top/gtqtgbphfu.html

[T23] Swift：函数
来源：http://hz.pengpengdd.cyou/gtipklubqx.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yonumen.top/gttnbkzihu.html

[T24] Swift：闭包
来源：http://hz.shanyushiyangkeji.top/gtnusddkrn.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yangfankeji.com/gtgnmvgcmy.html

[T25] Swift：结构体
来源：http://hz.sweek.top/gtvsfanjhm.html

struct P { var x: Int }
来源：http://hz.zhongyouzk.top/gtiwqovbln.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtiyoqzefo.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtucplwuwa.html

[T27] Swift：错误处理
来源：http://hz.jyoumei.cn/gtzsspbbwf.html

do { try f() } catch { print(error) }
来源：http://hz.hywenlv.cn/gtuyufqrag.html

[T28] Swift：枚举
来源：http://hz.iojbl.cn/gtdjoovxwg.html

enum Color { case red, green }
来源：http://hz.tianlin.xyz/gtofieeqst.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtgvzjsvyc.html

guard let x = opt else { return }
来源：http://hz.0kj1m.cn/gtvnqietmg.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtzdyumkzh.html

protocol Shape { func area() -> Double }
来源：http://hz.xuetiantiany.cn/gtroyngilv.html

[T31] Lua：Hello World
来源：http://hz.yueranfly.top/gtauinhwva.html

print("Hello")
来源：http://hz.shanyushiyangkeji.top/gttihtgdrw.html

[T32] Lua：局部变量
来源：http://hz.iojbl.cn/gtyfprshmh.html

local a = 1
来源：http://hz.andypj.xyz/gtufdoaive.html

[T33] Lua：表（数组）
来源：http://hz.fengsongda.top/gtccjkcmfu.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.wangdashe.top/gtkpvlodhs.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gtleyyhjue.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.dianchejie.cn/gtflbxyecm.html

[T35] Lua：字典表
来源：http://hz.zhoulong.xyz/gtazdgixig.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gotoacloud.top/gtvpirkpcb.html

[T36] Lua：函数
来源：http://hz.zdqjudy.top/gtvjlhjrpe.html

function add(a, b) return a + b end
来源：http://hz.jinqigfzy.top/gtlacobstw.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtsffyxhed.html

"a" .. "b"
来源：http://hz.yonumen.top/gtxdihgtxw.html

[T38] Lua：条件
来源：http://hz.cqqwz.cn/gtqleaxlch.html

if x > 0 then print("正") end
来源：http://hz.tanke756.top/gtngtebppe.html

[T39] Lua：模式匹配
来源：http://hz.zhoulong.xyz/gtodlinaak.html

string.find(s, "%d+")
来源：http://hz.vqdsnc.cn/gtvrvnhgkd.html

[T40] Lua：元表
来源：http://hz.yj20258888.top/gtqjhmrwqv.html

setmetatable({}, { __index = base })
来源：http://hz.jianghu66.top/gtmvohvbmn.html

[T41] Perl：Hello World
来源：http://hz.zycfv.cn/gtmoasxdtp.html

print "Hello\n";
来源：http://hz.0kj1m.cn/gtbgyocxby.html

[T42] Perl：变量类型
来源：http://hz.haohaochexian.top/gtjtzzvrsn.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.sysykeji.top/gtqaheejth.html

[T43] Perl：字符串插值
来源：http://hz.daxiang520.top/gtauqvzoju.html

"值: $a"
来源：http://hz.tanke756.top/gtttpyrkrc.html

[T44] Perl：条件
来源：http://hz.zhengqikj.top/gtelxlexyk.html

if ($a > 0) { print "正"; }
来源：http://hz.fzhhl.top/gtgqpmwwgq.html


<!-- 参考信息 -->