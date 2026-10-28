代发 wailian999

cmd > out.log 2>&1
来源：http://hz.zhoulong.xyz/gtditbmqpw.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtosljlbph.html

echo "log" >> out.log
来源：http://hz.pengpengdd.cyou/gtblhhgfdx.html

[R41] 丢弃输出
来源：http://hz.ppjwa.cn/gtgsconjdy.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtpzwohlic.html

[R42] 输入重定向
来源：http://hz.jinqigufen.top/gtnyzrgiqu.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtuahwrzcw.html

[R43] 按名字查找文件
来源：http://hz.dashuyun.cn/gtyizdukun.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtmjjfryvv.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtvslbxlou.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtayfhskdk.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtjohcoamf.html

find . -name "*.tmp" -delete
来源：http://hz.shangyingyoupin.top/gtdfykyyku.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtajxjpxph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ywan-chungtsiang.top/gtiturepbi.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gtggpmscmc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gtcqsusdim.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtvbdpdnfx.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtewigpqto.html

[R49] awk 带条件
来源：http://hz.smart0.xyz/gthnelsohz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jiagoushi.top/gtgbonidqy.html

[R50] awk 求和
来源：http://hz.hongshengwenyu.top/gtykhpcpcy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.daria6918.cn/gteeybgldc.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gtwgimzlum.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.meibo888.top/gtfuwdswxj.html

[R52] 统计行数
来源：http://hz.xuanzx.com/gtywriqokf.html

wc -l a.txt
来源：http://hz.sufxvd.cn/gtuysvvfpi.html

[R53] 查看文件头与实时尾
来源：http://hz.ppjwa.cn/gtljiixqcb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cheryme.top/gtweqmwami.html

[R54] 比较两个文件
来源：http://hz.xingfuxueyuan.xyz/gtnzoezcna.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtuurayhyr.html

[R55] 压缩与解压
来源：http://hz.52xcode.cn/gtzxdcdtfy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shuidangran.top/gtaicxhspz.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtzasdvbgt.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtifqmfryt.html

[R57] 远程执行命令
来源：http://hz.nanxinkj.top/gtlhzkkasq.html

ssh user@host 'uptime'
来源：http://hz.xylfe.cn/gtfuqqsuoo.html

[R58] 下载文件
来源：http://hz.jqgufenzy.top/gtimtyndjw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.redwolf501.top/gtzbozhqhk.html

[R59] 发 POST JSON
来源：http://hz.hfpthk.cn/gttcirsgvd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gaohongyu789.top/gtooxworgc.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj202588.top/gtulojqajz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gttbxarium.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtrrdtnwqy.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtdhircyll.html

[R62] 找最占空间的文件
来源：http://hz.jinghuilouyu.cn/gtjguwfiys.html

du -ah . | sort -rh | head -10
来源：http://hz.redwolf501.top/gtolaftezk.html

[R63] 内存与进程
来源：http://hz.xuanzx.com/gtepvodjsn.html

free -h;  ps aux | grep nginx
来源：http://hz.tian-w.cn/gtvqzfeshw.html

[R64] 结束进程
来源：http://hz.hysaishi.cn/gtqsvqbeud.html

kill -9 $(pgrep -f app.py)
来源：http://hz.316326.xyz/gtmnwzbccm.html

[R65] 查看端口占用
来源：http://hz.gogol.net.cn/gtsczvwigs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinyuanbaomall.cn/gtusdoffpc.html

[R66] 定时任务
来源：http://hz.cheryme.top/gtarwdufsk.html

crontab -e;  crontab -l
来源：http://hz.yanxiufei.cn/gtcopkrsga.html

[R67] 生成随机十六进制串
来源：http://hz.ppjwa.cn/gtteuntptd.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtyduoxoyg.html

[R68] 计算文件校验值
来源：http://hz.ivvv.top/gtvvkqiass.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yueranfly.top/gtcwgcpbuq.html

[R69] 生成随机密码
来源：http://hz.aizwys.cn/gtfctymfwl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtjmanpizv.html

[R70] 时间戳与互转
来源：http://hz.xinyue.icu/gthjppxjak.html

date +%s;  date -d @1700000000
来源：http://hz.tianlin.xyz/gtwtwsgsxc.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtiryqhsdp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtppdglrmm.html

[R72] 等待端口就绪
来源：http://hz.tianlin.xyz/gtznyxmfgf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gtnoqzadgv.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtlpdoxbhf.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtvwuvwiod.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtvfvhucyb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.feifeiyinyue.top/gtffvolwwp.html

[R75] 导出环境变量
来源：http://hz.bjfxy.top/gtsqqhrieh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ydzc1.top/gtnqtodwnz.html

[R76] 使用临时文件
来源：http://hz.hnxiangtu.top/gtbrjxnsnr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhaomingkeji.xyz/gtjeijfrga.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtjatcisyn.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtyaoaqnjj.html

[R78] 交互式菜单
来源：http://hz.chenlongwang.top/gtftdphvlf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gtzpdpwzvd.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gtmjphctwr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhaomingkeji.xyz/gtfjrodgyy.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtqldtkozd.html

time ./run.sh
来源：http://hz.wangdashe.top/gtdhtdwzxv.html

================================================================================
来源：http://hz.haohaochexian.top/gtblcjwqbb.html

S. C / C++ 专题
来源：http://hz.shanyushiyangtech.top/gtbxomyvam.html

================================================================================
来源：http://hz.sweek.top/gtjmgqdxdj.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtuehpgeem.html

#include <stdio.h>
来源：http://hz.svipenyu.cn/gtjnchaioo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtfkgjenph.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtkgalzoxm.html

int a = 10; printf("%d\n", a);
来源：http://hz.sweek.top/gtncjfjlfo.html

[S03] C：读入整数
来源：http://hz.yanxiufei.cn/gtvqhyrgex.html

int x; scanf("%d", &x);
来源：http://hz.52xcode.cn/gttesupesp.html

[S04] C：字符串复制
来源：http://hz.jlsjyb.cn/gtiqenonmp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhijiandao.cn/gtndwpkrba.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtucpubcst.html

strlen(s)
来源：http://hz.yvedp.cn/gtqhrdvshs.html

[S06] C：字符串比较
来源：http://hz.feifeiyinyue.top/gtirzzhpzh.html

strcmp(a, b) == 0
来源：http://hz.yongpay.top/gtioiqsvta.html

[S07] C：数组遍历求和
来源：http://hz.jinghuilouyu.cn/gtjpwnqmtn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.9152youxi.cn/gtoacuwegd.html

[S08] C：动态内存分配与释放
来源：http://hz.xuetiantiany.cn/gtzldysvnj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuanzhike.top/gtxwbpgosj.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtxehbbrxt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xziqi.cn/gtkskwgdml.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gthudlqpzf.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtdtkwsdck.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtoojzomfi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sufxvd.cn/gtinkupkpp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtqxkqjbya.html

fclose(f);
来源：http://hz.ehwqpu.com/gtrngclfzc.html

[S12] C：写文件
来源：http://hz.jinqigufen.top/gttllewckr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.meibo888.top/gtrziqshhi.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtghntzmnb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gtoxuojvua.html

[S14] C：枚举
来源：http://hz.ehwqpu.com/gtcrsqtqfo.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.dashuyun.cn/gtunsqsefx.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtewogfcwe.html

(double) a / b
来源：http://hz.jqgufenzy.top/gtsflnkhfp.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gttkiwgpwx.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtukbvtfuy.html

[S17] C：安全拼接字符串
来源：http://hz.chenzaomai.com/gtbdumqbwp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gttlomayfu.html

[S18] C：命令行参数
来源：http://hz.gogol.net.cn/gtbrnfteuq.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtkccsbdli.html

[S19] C：快速排序
来源：http://hz.meibo888.top/gtaymchord.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtxwquxedv.html

[S20] C：二分查找
来源：http://hz.daria6918.cn/gtokehutzl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigfzy.top/gtqtrekyda.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gtqyaapkyx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yonumen.top/gtvbyefevk.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangkeji.top/gtngnzygdx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.aibaodan.cn/gthmcccwrg.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtvspontlg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gaohongyu789.top/gtgtusoggv.html

[S24] C：获取本地时间
来源：http://hz.xziqi.cn/gtxcjbqvjm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtrhsvsefj.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gttyujlyhw.html

memcpy(dst, src, n);
来源：http://hz.tianlin.xyz/gtgibwzmri.html

[S26] C：内存清零
来源：http://hz.0kj1m.cn/gtdsotovih.html

memset(a, 0, sizeof a);
来源：http://hz.yuxming.cn/gtcgkyvdvb.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtqwfzogfn.html

const double PI = 3.14159;
来源：http://hz.yueranfly.top/gtmikdugwz.html

[S28] C：静态变量
来源：http://hz.zycfv.cn/gtkicijisk.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtzxzzoosd.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtdqucfvht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cucudq.cn/gtkynchszt.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gtclgnnivg.html

#ifndef X_H
来源：http://hz.sufxvd.cn/gtimonkymm.html

#define X_H
来源：http://hz.jiagoushi.top/gtnubbzehj.html

#endif
来源：http://hz.cucudq.cn/gtzzyutpda.html

[S31] C++：Hello World
来源：http://hz.smart0.xyz/gtawcmveyq.html

#include <iostream>
来源：http://hz.wangdashe.top/gtdwrokdws.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gthlyklsai.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtnzdpocky.html

std::string s = "hi";  s += "!";
来源：http://hz.hnxiangtu.top/gtmsoxbhum.html

[S33] C++：vector 增删
来源：http://hz.jinghuilouyu.cn/gtyjxbedvq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.0kj1m.cn/gtbgajdfxt.html

[S34] C++：遍历 vector
来源：http://hz.sweek.top/gtgzdhauea.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhijiandao.cn/gtavspihem.html

[S35] C++：map
来源：http://hz.nanxuanxn.top/gtcswbupoc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtzrazifkm.html

[S36] C++：unordered_map
来源：http://hz.hfpthk.cn/gtwouwqhpd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtkdebepzp.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtuufcnvgu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtatyxfeyw.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtpjrjuqrb.html

std::sort(v.begin(), v.end());
来源：http://hz.jinghuilouyu.cn/gthtlrjuwb.html

[S39] C++：自定义比较器排序
来源：http://hz.tianlin.xyz/gtslgfohiz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhongyouzk.top/gtexpglnnc.html

[S40] C++：查找元素
来源：http://hz.jqgfzy.top/gtfmpborig.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.nanxuanxn.top/gtkhvimcbl.html

[S41] C++：类与构造函数
来源：http://hz.jiagoushi.top/gtajtljkxo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hnqzz.top/gtcaqbfvjm.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtgqlmhhid.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangkeji.top/gtlwjlpbyj.html

[S43] C++：智能指针
来源：http://hz.vqdsnc.cn/gthtdjxalv.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhixingplan.top/gtipdqhjry.html

[S44] C++：引用传参
来源：http://hz.cheryme.top/gtulpqngfk.html

void inc(int &x) { ++x; }
来源：http://hz.sxryk.cn/gtujceyuqv.html

[S45] C++：lambda
来源：http://hz.guowangkeji.top/gtygfhlpom.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenlongwang.top/gtmzsvtjyr.html

[S46] C++：函数模板
来源：http://hz.gzhubu.top/gtrivixqiu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnqzz.top/gtevmuczwo.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gttvcawetk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtlbfsiysn.html

[S48] C++：逐行读文件
来源：http://hz.tianlin.xyz/gtyrlstsjo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtmwmzjttk.html

while (std::getline(in, line)) { }
来源：http://hz.9152youxi.cn/gtmzzvjgxr.html

[S49] C++：写文件
来源：http://hz.zhiwuduotai.top/gtwjpjayfe.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtgkaunlgx.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangtech.top/gtwjgaorfx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hysaishi.cn/gtxppnjarg.html

[S51] C++：显式类型转换
来源：http://hz.jianghu66.top/gtafbtfdtm.html

static_cast<double>(a) / b
来源：http://hz.yangfankeji.com/gtgmkwzwvg.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gttourcgyp.html

int size() const noexcept { return n_; }
来源：http://hz.fzhhl.top/gttidzzolw.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangtech.top/gtuxtrwlkh.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtmekpisrq.html

[S54] C++：异常处理
来源：http://hz.aizwys.cn/gtxleybktx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.feifeiyinyue.top/gtvlyyrjja.html

[S55] C++：结构化绑定
来源：http://hz.yongpay.top/gtaoufvhlm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.aizwys.cn/gtyrynyxib.html

[S56] C++：optional
来源：http://hz.daria6918.cn/gtegkceflq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhiwuduotai.top/gthfrcwkgm.html

[S57] C++：编译期常量
来源：http://hz.ivvv.top/gtlejgahcz.html

constexpr int N = 10;
来源：http://hz.tian-w.cn/gtsfwqitgv.html

[S58] C++：命名空间
来源：http://hz.xylfe.cn/gtwmoxvflr.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtuucgewsy.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtarnyaeud.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jqgufenzy.top/gtpanpkrfh.html

[S60] C++：遍历并删除元素
来源：http://hz.redwolf501.top/gtkusfgnxk.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtkvfqeihs.html

================================================================================
来源：http://hz.cqqwz.cn/gthauoskrq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtbzkpztva.html

================================================================================
来源：http://hz.fengsongda.top/gtetfofykt.html

[T01] Kotlin：Hello World
来源：http://hz.fengsongda.top/gtievyxewx.html

println("Hello")
来源：http://hz.svipenyu.cn/gtvnoklufb.html

[T02] Kotlin：变量
来源：http://hz.redwolf501.top/gtjivgggzk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xziqi.cn/gthrtivens.html

[T03] Kotlin：字符串模板
来源：http://hz.ivvv.top/gtynjuurtu.html

"值: $b"
来源：http://hz.sufxvd.cn/gtujgqzoji.html

[T04] Kotlin：空安全
来源：http://hz.ppjwa.cn/gtuubavyvw.html

val n: String? = null;  n?.length
来源：http://hz.hywenlv.cn/gtyinuvrdj.html

[T05] Kotlin：when 表达式
来源：http://hz.pycfn.com/gtcxvaront.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xylfe.cn/gtaafkvcym.html

[T06] Kotlin：集合映射
来源：http://hz.316326.xyz/gtlcxfuafd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtpnwawxkj.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtjrrennct.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.iojbl.cn/gtposomgts.html

[T08] Kotlin：数据类
来源：http://hz.shanyushiyangkeji.top/gtbtbtqflz.html

data class User(val name: String, val age: Int)
来源：http://hz.ppjwa.cn/gtdofzmmgt.html

[T09] Kotlin：扩展函数
来源：http://hz.yueranfly.top/gthjbgwojj.html

fun String.exclaim() = this + "!"
来源：http://hz.tianlin.xyz/gtygbckevx.html

[T10] Kotlin：默认参数
来源：http://hz.kuanghao11.cn/gtqeodzhql.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xziqi.cn/gthdhgcgiw.html

[T11] Kotlin：协程
来源：http://hz.chenjidiqi.icu/gtfehogqhx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.meibo888.top/gtcvehohka.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtvlftyvav.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtqguuptek.html

[T13] Kotlin：只读 Map
来源：http://hz.jiagoushi.top/gtrekrvmgz.html

val m = mapOf("a" to 1)
来源：http://hz.9152youxi.cn/gtkllomvjs.html

[T14] Kotlin：循环
来源：http://hz.daria6918.cn/gtnioczlnz.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gtexkzehfb.html

[T15] Kotlin：接口
来源：http://hz.cqqwz.cn/gtdwqzlxka.html

interface Shape { fun area(): Double }
来源：http://hz.gzhubu.top/gthyvopwfa.html

[T16] Swift：Hello World
来源：http://hz.316326.xyz/gtonfhakai.html

print("Hello")
来源：http://hz.316326.xyz/gthwirdzef.html

[T17] Swift：变量与常量
来源：http://hz.xziqi.cn/gtjijgqwnl.html

var a = 1;  let b = 2
来源：http://hz.wangdashe.top/gtyxovbdfs.html

[T18] Swift：字符串插值
来源：http://hz.yongpay.top/gtvxqzalwl.html

"值: \(b)"
来源：http://hz.feifeiyinyue.top/gtjejpbgsp.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtludpvzxj.html

if let n = opt { print(n) }
来源：http://hz.redwolf501.top/gtrjvwpbly.html

[T20] Swift：数组操作
来源：http://hz.ivvv.top/gtfmwydtrv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtrpktvgdu.html

[T21] Swift：遍历
来源：http://hz.cqqwz.cn/gtrbcsaafh.html

for x in a { print(x) }
来源：http://hz.ppjwa.cn/gtiqyetsba.html

[T22] Swift：字典
来源：http://hz.yangfankeji.com/gtosxzzqov.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhoulong.xyz/gtmueunjlw.html

[T23] Swift：函数
来源：http://hz.sysykeji.top/gtcxrvcugz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cdnleiting.top/gtwegxgyla.html

[T24] Swift：闭包
来源：http://hz.shzxlz.cn/gtkqunaugh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.havefunace.top/gtstjdtnzb.html

[T25] Swift：结构体
来源：http://hz.pengpengdd.cyou/gtpqznlohe.html

struct P { var x: Int }
来源：http://hz.jyoumei.cn/gtosysiiqs.html

[T26] Swift：类与重写
来源：http://hz.snrcjt.cn/gtdigummms.html

class A: Base { override func f() {} }
来源：http://hz.wangdashe.top/gtweohgzgm.html

[T27] Swift：错误处理
来源：http://hz.shuidangran.top/gtjsgeddfa.html

do { try f() } catch { print(error) }
来源：http://hz.zhijiandao.cn/gtiqpqspue.html

[T28] Swift：枚举
来源：http://hz.c1oappe.top/gtibcyzpbn.html

enum Color { case red, green }
来源：http://hz.quarkkingdee.top/gtslwdfoqh.html

[T29] Swift：guard 提前返回
来源：http://hz.xinyue.icu/gtobvrbwlq.html

guard let x = opt else { return }
来源：http://hz.ivvv.top/gtctpkqkde.html

[T30] Swift：协议
来源：http://hz.yongpay.top/gtjdlanobq.html

protocol Shape { func area() -> Double }
来源：http://hz.yangfankeji.com/gtdzuwpxbl.html

[T31] Lua：Hello World
来源：http://hz.zhongyouzk.top/gtjzbaalyt.html

print("Hello")
来源：http://hz.zhiwuduotai.top/gtiorthlez.html

[T32] Lua：局部变量
来源：http://hz.yueranfly.top/gtweynjgla.html

local a = 1
来源：http://hz.jiagoushi.top/gtfpcivxdt.html

[T33] Lua：表（数组）
来源：http://hz.jqgufenzy.top/gtjchfryaf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtpxqqhzoi.html

[T34] Lua：遍历表
来源：http://hz.zhijiandao.cn/gtefvibkrs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtqoobpcgj.html

[T35] Lua：字典表
来源：http://hz.yongpay.top/gtbapqhdkv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.wangdashe.top/gtjycojrzq.html

[T36] Lua：函数
来源：http://hz.shuidangran.top/gtskhczynr.html

function add(a, b) return a + b end
来源：http://hz.mhx1999.top/gttjxctgfw.html

[T37] Lua：字符串拼接
来源：http://hz.svipenyu.cn/gtislsssrq.html

"a" .. "b"
来源：http://hz.yj202588.top/gtrctetepp.html

[T38] Lua：条件
来源：http://hz.cucudq.cn/gtponazmhi.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtlxnxwgan.html

[T39] Lua：模式匹配
来源：http://hz.hnxiangtu.top/gtaxgmkcan.html

string.find(s, "%d+")
来源：http://hz.gotoacloud.top/gtifkxtncs.html

[T40] Lua：元表
来源：http://hz.chenjidiqi.icu/gtxsxlqdsq.html

setmetatable({}, { __index = base })
来源：http://hz.sxryk.cn/gtfddbqepl.html

[T41] Perl：Hello World
来源：http://hz.cucudq.cn/gtodmqjhkp.html

print "Hello\n";
来源：http://hz.hywenlv.cn/gtaajervre.html

[T42] Perl：变量类型
来源：http://hz.hnqzz.top/gtkgdivkcs.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cucudq.cn/gtoycnawmn.html


<!-- 参考信息 -->