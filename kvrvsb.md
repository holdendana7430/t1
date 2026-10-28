代发 wailian999

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtdccbejgl.html

[R38] 管道串联
来源：http://hz.fengsongda.top/gtfszsymcp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guowangkeji.top/gtsrznodew.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtiupzoxdz.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtognzncao.html

[R40] 追加写日志
来源：http://hz.jiagoushi.top/gtplmcusly.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtpmxrlsbk.html

[R41] 丢弃输出
来源：http://hz.jqgfzy.top/gthivmvfqj.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258888.top/gtcmxpakgv.html

[R42] 输入重定向
来源：http://hz.jinyuanbaomall.cn/gtpqnvrnnf.html

wc -l < a.txt
来源：http://hz.yueranfly.top/gtdxelurwb.html

[R43] 按名字查找文件
来源：http://hz.wangshuangyany.cn/gtpysxtfum.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtunoiwqfs.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtvlgvqitj.html

find . -mtime -7 -type f
来源：http://hz.jiagoushi.top/gtxbgewfbc.html

[R45] 批量删除
来源：http://hz.zhoulong.xyz/gtrkjfkcfl.html

find . -name "*.tmp" -delete
来源：http://hz.yongpay.top/gtfyltekqb.html

[R46] 递归替换文件内容
来源：http://hz.iojbl.cn/gtezygppyb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shzxlz.cn/gtmvgyeila.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gtjocgcyme.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gtslztupic.html

[R48] awk 取指定列
来源：http://hz.birdmap.top/gtolnpsbqu.html

awk '{print $1, $3}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtyyjjsxdj.html

[R49] awk 带条件
来源：http://hz.hywenlv.cn/gtihixebeu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydjk.org.cn/gttosynqxr.html

[R50] awk 求和
来源：http://hz.sufxvd.cn/gtepsuopfj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtvefjxeua.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtobjcgpft.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gtghtjrvvd.html

[R52] 统计行数
来源：http://hz.0kj1m.cn/gtsgmdvyaw.html

wc -l a.txt
来源：http://hz.yueranfly.top/gtokfyjxlc.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtsahflpwv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhongyouzk.top/gtpskoomnj.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtsrbjnbus.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtjrptrono.html

[R55] 压缩与解压
来源：http://hz.yuxming.cn/gtxczvdppa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtdtjeufxy.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtgaduvbfc.html

scp file user@host:/path/
来源：http://hz.hnxiangtu.top/gtzbddqoxs.html

[R57] 远程执行命令
来源：http://hz.jinqigufen.top/gtkgmmifnj.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtajqjtrpd.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtsyhrqivq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtksvfpgse.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gttjyvfxok.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ppjwa.cn/gtpdtbahtr.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gtzphjwcpx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangkeji.top/gtvitlnrtc.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtpmchyicq.html

df -h;  du -sh *
来源：http://hz.aibaodan.cn/gtajqfphct.html

[R62] 找最占空间的文件
来源：http://hz.nwbrower.top/gtretcboci.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtepjjxlti.html

[R63] 内存与进程
来源：http://hz.yanxiufei.cn/gtbfhyickg.html

free -h;  ps aux | grep nginx
来源：http://hz.sysykeji.top/gtxskfiuqk.html

[R64] 结束进程
来源：http://hz.shzxlz.cn/gtqhezmvcc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhongyouzk.top/gteywwzprg.html

[R65] 查看端口占用
来源：http://hz.sufxvd.cn/gtxkvguojv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuxming.cn/gtxvlucrha.html

[R66] 定时任务
来源：http://hz.sweek.top/gtboilxeqn.html

crontab -e;  crontab -l
来源：http://hz.wangdashe.top/gtsorsriil.html

[R67] 生成随机十六进制串
来源：http://hz.tanke756.top/gtxjejywll.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtlrinskba.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtikxmanyu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtbggbnkjp.html

[R69] 生成随机密码
来源：http://hz.nanxuanxn.top/gtwtkkfzgl.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtpdcbmeok.html

[R70] 时间戳与互转
来源：http://hz.gogol.net.cn/gtadgnfucy.html

date +%s;  date -d @1700000000
来源：http://hz.yanxiufei.cn/gtkfyzgypz.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtnqmlvjyt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gtuginigry.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtwxbluhtc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jlsjyb.cn/gthalcnpkn.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gttxhgafau.html

split -l 1000 big.log part_
来源：http://hz.redwolf501.top/gtczygsvco.html

[R74] 批量重命名
来源：http://hz.redwolf501.top/gthmjgvaut.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtssjgbcdh.html

[R75] 导出环境变量
来源：http://hz.gogol.net.cn/gtnhnpzjws.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj202588.top/gthkibqieu.html

[R76] 使用临时文件
来源：http://hz.yangfankeji.com/gtaqxywciw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yanxiufei.cn/gtgzxnaxzl.html

[R77] 读取用户输入
来源：http://hz.jinghuilouyu.cn/gtmzylrfnr.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtlbboxpnl.html

[R78] 交互式菜单
来源：http://hz.nwbrower.top/gtcumwexew.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtozknsuke.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtxnsyogjo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtzctwnwof.html

[R80] 查看脚本执行耗时
来源：http://hz.shuidangran.top/gtxgpglotd.html

time ./run.sh
来源：http://hz.zhengqikj.top/gtzmjxzeug.html

================================================================================
来源：http://hz.sxryk.cn/gtixvpbiaw.html

S. C / C++ 专题
来源：http://hz.jinyuanbaomall.cn/gtmbicikpo.html

================================================================================
来源：http://hz.daria6918.cn/gtfivnufan.html

[S01] C：Hello World
来源：http://hz.guowangkeji.top/gtbzmgtwcb.html

#include <stdio.h>
来源：http://hz.jyoumei.cn/gtcxwogyzw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hywenlv.cn/gtbiboiytv.html

[S02] C：变量与格式化输出
来源：http://hz.cheryme.top/gtjufekavw.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtnnhkaedv.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtawbqnwmq.html

int x; scanf("%d", &x);
来源：http://hz.0kj1m.cn/gttkintkpy.html

[S04] C：字符串复制
来源：http://hz.0kj1m.cn/gtdiufzjua.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tian-w.cn/gttatvenyp.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtazajkagr.html

strlen(s)
来源：http://hz.birdmap.top/gtlkocqjwf.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gtszzpbdpq.html

strcmp(a, b) == 0
来源：http://hz.nanxuanxn.top/gtqklmyges.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtodixktpx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sweek.top/gtlcbejxjb.html

[S08] C：动态内存分配与释放
来源：http://hz.zhoulong.xyz/gtqngbvpxa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtjgabnbgh.html

[S09] C：结构体定义与初始化
来源：http://hz.hnqzz.top/gtcthlqpfy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtbhwxhkxg.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtxemglcue.html

int *p = &a;  *p = 5;
来源：http://hz.yonumen.top/gtmcmtrgbc.html

[S11] C：逐行读文件
来源：http://hz.jlsjyb.cn/gtlfbkbjzy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenjidiqi.icu/gteswspkps.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jlsjyb.cn/gtceysqbxo.html

fclose(f);
来源：http://hz.gaohongyu789.top/gtirhmxkrv.html

[S12] C：写文件
来源：http://hz.shanyushiyangtech.top/gtaozxkczo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.iojbl.cn/gtqtzfecpy.html

[S13] C：宏定义
来源：http://hz.quarkkingdee.top/gtbnsknpng.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.0kj1m.cn/gtecdztrub.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtfegrhvnr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jyoumei.cn/gtleorzxxz.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtkyjjumkp.html

(double) a / b
来源：http://hz.ywan-chungtsiang.top/gtmorbajlr.html

[S16] C：位操作置位
来源：http://hz.guannengcc.top/gtalbjggyw.html

x |= (1 << 3);
来源：http://hz.nanxuanxn.top/gtdkptjtxp.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtmcjjygit.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtputnyiwr.html

[S18] C：命令行参数
来源：http://hz.bjfxy.top/gtmcllfkxn.html

int main(int argc, char **argv)
来源：http://hz.tianlin.xyz/gthazmprnl.html

[S19] C：快速排序
来源：http://hz.aibaodan.cn/gtubmrpafr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtsvxojoak.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gtidmoindc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtxtefsjvr.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtymcvjbpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.52xcode.cn/gtgvhwtspy.html

[S22] C：字符串转数字
来源：http://hz.bjfxy.top/gtlnocfwvi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtosviiecv.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gtjlegmwzv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.9152youxi.cn/gtwqawykfc.html

[S24] C：获取本地时间
来源：http://hz.pycfn.com/gtupvcgmij.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.dianchejie.cn/gtjjftdmno.html

[S25] C：内存拷贝
来源：http://hz.gotoacloud.top/gtloghmdaq.html

memcpy(dst, src, n);
来源：http://hz.hammf.cn/gtgztfnzdv.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtpjmstjgh.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtttlriylp.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtasukrmhl.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtmyjsgzqh.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gtfpvzxgpw.html

static int counter = 0;
来源：http://hz.yuxming.cn/gtzrnmaael.html

[S29] C：变参函数
来源：http://hz.daria6918.cn/gtfctruzfj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zdqjudy.top/gtlfsijkzi.html

[S30] C：头文件保护
来源：http://hz.jiagoushi.top/gteutozzcl.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtgafbxfwn.html

#define X_H
来源：http://hz.jinqigufen.top/gtpixmyexv.html

#endif
来源：http://hz.c1oappe.top/gtjzotstzg.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtrzhbkqiw.html

#include <iostream>
来源：http://hz.cheryme.top/gtcifctgoj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtcucmbqxk.html

[S32] C++：字符串
来源：http://hz.gaohongyu789.top/gtqekqwazt.html

std::string s = "hi";  s += "!";
来源：http://hz.gaohongyu789.top/gtefibojzw.html

[S33] C++：vector 增删
来源：http://hz.hysaishi.cn/gtjzukmryj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tian-w.cn/gtkddjbgev.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gteyjwcmpq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtygznwxvh.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtwwyxnokh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhixingplan.top/gtaatpvnky.html

[S36] C++：unordered_map
来源：http://hz.guannengcc.top/gtbpsxiuwn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ydjk.org.cn/gtgdvyhicu.html

[S37] C++：set
来源：http://hz.feifeiyinyue.top/gtkfmzosen.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gtptwnulcf.html

[S38] C++：排序
来源：http://hz.wangshuangyany.cn/gtilnbudgw.html

std::sort(v.begin(), v.end());
来源：http://hz.sxryk.cn/gtowoxnxnt.html

[S39] C++：自定义比较器排序
来源：http://hz.ydzc1.top/gtbicsfose.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gogol.net.cn/gtmzkvmmby.html

[S40] C++：查找元素
来源：http://hz.feifeiyinyue.top/gtirxvkaul.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xuanzx.com/gtyralqnxl.html

[S41] C++：类与构造函数
来源：http://hz.quarkkingdee.top/gttauuaomu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ivvv.top/gtqpgaizze.html

[S42] C++：继承与虚函数
来源：http://hz.dianchejie.cn/gtbxoldtpk.html

class B : public Base { public: void f() override {} };
来源：http://hz.nanxuanxn.top/gtstqvpbtz.html

[S43] C++：智能指针
来源：http://hz.hysaishi.cn/gtjtikupzz.html

auto p = std::make_unique<int>(5);
来源：http://hz.daxiang520.top/gttpryfbxw.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gtkplclayb.html

void inc(int &x) { ++x; }
来源：http://hz.pycfn.com/gtjvlrggmg.html

[S45] C++：lambda
来源：http://hz.yj20258.top/gtxqberbqx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gtkcrtbehl.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtkdfcciap.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yvedp.cn/gttpctbeeo.html

[S47] C++：结构化绑定遍历
来源：http://hz.zhixingplan.top/gthbofbnxo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nwbrower.top/gtqlfwecne.html

[S48] C++：逐行读文件
来源：http://hz.ppjwa.cn/gtlnshlrne.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtqaqrgasf.html

while (std::getline(in, line)) { }
来源：http://hz.kuanghao11.cn/gtspyiyrnd.html

[S49] C++：写文件
来源：http://hz.0kj1m.cn/gtqyppnkfn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nwbrower.top/gtpaespxgq.html

[S50] C++：格式化数字
来源：http://hz.zycfv.cn/gticpgmonf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.fzhhl.top/gtjaseklzm.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtxbasltyo.html

static_cast<double>(a) / b
来源：http://hz.yj202588.top/gtyvnmduxh.html

[S52] C++：const 与 noexcept
来源：http://hz.pycfn.com/gtfdjtcwyr.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gtpxwbrdal.html

[S53] C++：移动语义
来源：http://hz.xuetiantiany.cn/gttgelklpw.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtherukgtf.html

[S54] C++：异常处理
来源：http://hz.dianchejie.cn/gtlsuofndg.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinghuilouyu.cn/gtcpilgyrc.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtqjtuldir.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.chenzaomai.com/gtrmruzkfc.html

[S56] C++：optional
来源：http://hz.fengsongda.top/gtrhblomug.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinghuilouyu.cn/gtqdtkeyxo.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gtjyzuxody.html

constexpr int N = 10;
来源：http://hz.zhiwuduotai.top/gtcohlpkjd.html

[S58] C++：命名空间
来源：http://hz.ehwqpu.com/gtynkwjvgq.html

namespace ns { int f() { return 1; } }
来源：http://hz.daxiang520.top/gtsgjlsbic.html

[S59] C++：静态断言
来源：http://hz.52xcode.cn/gtdtyusmfg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenlongwang.top/gtfojflhdv.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtodbnxuud.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenlongwang.top/gtpvrorvjr.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtelzegnnk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guowangkeji.top/gtszcoxqnq.html

================================================================================
来源：http://hz.guannengcc.top/gtpuyzucgz.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258888.top/gttkvpdeou.html

println("Hello")
来源：http://hz.cheryme.top/gtpqkxbmhn.html

[T02] Kotlin：变量
来源：http://hz.zhengqikj.top/gtocatmvkz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.c1oappe.top/gtdiyctbyi.html

[T03] Kotlin：字符串模板
来源：http://hz.vqdsnc.cn/gtxtpayoii.html

"值: $b"
来源：http://hz.andypj.xyz/gttazawonl.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtxoidbgqo.html

val n: String? = null;  n?.length
来源：http://hz.aibaodan.cn/gtjykihkds.html

[T05] Kotlin：when 表达式
来源：http://hz.pengpengdd.cyou/gttnrxzdkh.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuxming.cn/gtybvfpkzd.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gthszknkzk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.ehwqpu.com/gtrhvugkej.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtcwvttmgj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yongpay.top/gtpzbkihyb.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtpsymlrbv.html

data class User(val name: String, val age: Int)
来源：http://hz.tanke756.top/gtlwysfsne.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gthrdwoaek.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gtavewsuuv.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtygynswho.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtbyjprnaa.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtwgrkepjl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtxhbrnaxh.html

[T12] Kotlin：解构声明
来源：http://hz.yangfankeji.com/gtzhhzvpmq.html

val (a, b) = Pair(1, 2)
来源：http://hz.gzhubu.top/gtslvvfykc.html

[T13] Kotlin：只读 Map
来源：http://hz.hywenlv.cn/gtxzmxfqdd.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtpqzkquam.html

[T14] Kotlin：循环
来源：http://hz.cucudq.cn/gtrylwslem.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gthqxkwczi.html

[T15] Kotlin：接口
来源：http://hz.gaohongyu789.top/gtnwmfetfm.html

interface Shape { fun area(): Double }
来源：http://hz.tian-w.cn/gtsmqinfit.html

[T16] Swift：Hello World
来源：http://hz.cheryme.top/gtaaejiolp.html

print("Hello")
来源：http://hz.sweek.top/gtkeofbhyr.html

[T17] Swift：变量与常量
来源：http://hz.guowangkeji.top/gtzmcwofif.html

var a = 1;  let b = 2
来源：http://hz.chenlongwang.top/gtmrukfvvh.html

[T18] Swift：字符串插值
来源：http://hz.zhixingplan.top/gtifgykurb.html

"值: \(b)"
来源：http://hz.xinyue.icu/gtngxawgzs.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtntwszkuj.html

if let n = opt { print(n) }
来源：http://hz.chenzaomai.com/gtssvsazcp.html

[T20] Swift：数组操作
来源：http://hz.sxryk.cn/gtgnrwmmpi.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.daria6918.cn/gtzwfppzry.html

[T21] Swift：遍历
来源：http://hz.yj20258888.top/gtrfpswewz.html

for x in a { print(x) }
来源：http://hz.sxryk.cn/gtfywaygam.html

[T22] Swift：字典
来源：http://hz.zhijiandao.cn/gtsxdmfjgz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.chenzaomai.com/gttfffsmit.html

[T23] Swift：函数
来源：http://hz.jyoumei.cn/gtawecmccf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.c1oappe.top/gtcjirzpfe.html

[T24] Swift：闭包
来源：http://hz.xziqi.cn/gtmczkpuxh.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.chenlongwang.top/gtioiltaee.html

[T25] Swift：结构体
来源：http://hz.zhiwuduotai.top/gtgnbitmeb.html

struct P { var x: Int }
来源：http://hz.nwbrower.top/gtpthivloj.html

[T26] Swift：类与重写
来源：http://hz.jyoumei.cn/gtaanyyzay.html

class A: Base { override func f() {} }
来源：http://hz.yj20258.top/gtiibtckxg.html

[T27] Swift：错误处理
来源：http://hz.ehwqpu.com/gtigotopte.html

do { try f() } catch { print(error) }
来源：http://hz.snrcjt.cn/gtfiqwyvsv.html

[T28] Swift：枚举
来源：http://hz.hnqzz.top/gtpiuorktl.html

enum Color { case red, green }
来源：http://hz.daria6918.cn/gtjgrxgtxl.html

[T29] Swift：guard 提前返回
来源：http://hz.yj202588.top/gtonvenybw.html

guard let x = opt else { return }
来源：http://hz.xylfe.cn/gtrfifzner.html

[T30] Swift：协议
来源：http://hz.cashguo.top/gtiuwwordn.html

protocol Shape { func area() -> Double }
来源：http://hz.jinqigfzy.top/gtsmegjfiv.html

[T31] Lua：Hello World
来源：http://hz.feifeiyinyue.top/gtuwdiwdao.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtfhacuoza.html

[T32] Lua：局部变量
来源：http://hz.cheryme.top/gtzuojywhr.html

local a = 1
来源：http://hz.hfpthk.cn/gtxrxsfsrq.html

[T33] Lua：表（数组）
来源：http://hz.zycfv.cn/gtjdohkqyl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.yj20258.top/gtgfgqolph.html

[T34] Lua：遍历表
来源：http://hz.yuxming.cn/gtxdzaslbh.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.meibo888.top/gtkkyhswno.html

[T35] Lua：字典表
来源：http://hz.zhongyouzk.top/gtponlpohv.html

local d = { a = 1 };  d.b = 2
来源：http://hz.aibaodan.cn/gtkzyelbcr.html

[T36] Lua：函数
来源：http://hz.tanke756.top/gthgychlih.html

function add(a, b) return a + b end
来源：http://hz.cheryme.top/gtbtepolji.html

[T37] Lua：字符串拼接
来源：http://hz.tian-w.cn/gtljikgemm.html

"a" .. "b"
来源：http://hz.xingfuxueyuan.xyz/gtkdvhdobt.html

[T38] Lua：条件
来源：http://hz.vqdsnc.cn/gtdtmpzqlu.html

if x > 0 then print("正") end
来源：http://hz.sysykeji.top/gtabnjmihj.html

[T39] Lua：模式匹配
来源：http://hz.dashuyun.cn/gtnjjzjhfo.html

string.find(s, "%d+")
来源：http://hz.chenlongwang.top/gtlpwynsqs.html

[T40] Lua：元表
来源：http://hz.gotoacloud.top/gtulwahnyr.html

setmetatable({}, { __index = base })
来源：http://hz.pengpengdd.cyou/gtaqyolvrr.html


<!-- 参考信息 -->