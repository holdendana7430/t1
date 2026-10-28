代发 wailian999

files=$(ls -1)
来源：http://hz.birdmap.top/gtkwebtnap.html

[R38] 管道串联
来源：http://hz.zhaomingkeji.xyz/gtzbwarfpo.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtoymvsnsp.html

[R39] 重定向标准输出与错误
来源：http://hz.zdqjudy.top/gthrmlibay.html

cmd > out.log 2>&1
来源：http://hz.tanke756.top/gttinmpspl.html

[R40] 追加写日志
来源：http://hz.xylfe.cn/gtszqzisex.html

echo "log" >> out.log
来源：http://hz.yongpay.top/gtfmudwyma.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtersyydri.html

cmd >/dev/null 2>&1
来源：http://hz.52xcode.cn/gtdoayzpim.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtcdidaihi.html

wc -l < a.txt
来源：http://hz.316326.xyz/gtjfncfajm.html

[R43] 按名字查找文件
来源：http://hz.dianchejie.cn/gtcivqrncq.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtcqbdxyka.html

[R44] 按修改时间查找
来源：http://hz.ydzc1.top/gtzpxcgetc.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtoljtzweh.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtpgyzxzxg.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtiiiyyadr.html

[R46] 递归替换文件内容
来源：http://hz.jinqigufen.top/gtmlbfvach.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.daxiang520.top/gtzvqgvoxt.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gtvnxtpfts.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinyuanbaomall.cn/gtakibaspj.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gttkpfegsp.html

awk '{print $1, $3}' a.txt
来源：http://hz.9152youxi.cn/gtnthofvll.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtdzjuvdzo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gtqvpacckf.html

[R50] awk 求和
来源：http://hz.zhoulong.xyz/gtlgqrokko.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.quarkkingdee.top/gtmeizcbhm.html

[R51] 排序去重取前几
来源：http://hz.hysaishi.cn/gtbaylpyhl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cqqwz.cn/gtehknbapu.html

[R52] 统计行数
来源：http://hz.cqqwz.cn/gtdynxccgj.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtqwpwznug.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtfkgsceks.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinghuilouyu.cn/gtaevzxquq.html

[R54] 比较两个文件
来源：http://hz.zhiwuduotai.top/gtmlmlnavk.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gtaxjhtnrx.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtyjzwbkmh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtdnrugbah.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtkobqzqzp.html

scp file user@host:/path/
来源：http://hz.smart0.xyz/gtuwfulgcz.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtazodnsut.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtxlldglmu.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtldmndtau.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtwvkawbqp.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtvghnvche.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cqqwz.cn/gtqjwnljpj.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtjauteufw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yonumen.top/gtaenbyvop.html

[R61] 磁盘占用
来源：http://hz.pengpengdd.cyou/gtbcsovhul.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtvmefysed.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtbdwmkrqi.html

du -ah . | sort -rh | head -10
来源：http://hz.gaohongyu789.top/gtokymqfrz.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gttvctmlrb.html

free -h;  ps aux | grep nginx
来源：http://hz.iojbl.cn/gtgeuymced.html

[R64] 结束进程
来源：http://hz.sufxvd.cn/gtoifrzrnl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtneomvgrz.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtvfvqwepe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtqjedobza.html

[R66] 定时任务
来源：http://hz.jinyuanbaomall.cn/gtajplbfnf.html

crontab -e;  crontab -l
来源：http://hz.daria6918.cn/gtletdmukg.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gtkcxdbnff.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gteeuuypkt.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtwnjkwpod.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtyffnizxi.html

[R69] 生成随机密码
来源：http://hz.yvedp.cn/gtmysvtqhl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yueranfly.top/gtnxxffshs.html

[R70] 时间戳与互转
来源：http://hz.jinghuilouyu.cn/gtorxmkubz.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtzpdcjmks.html

[R71] 日期格式化
来源：http://hz.jyoumei.cn/gtqieiostf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.316326.xyz/gtekwokwma.html

[R72] 等待端口就绪
来源：http://hz.tianlin.xyz/gtgcvlrgfs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.iojbl.cn/gtvvgfgtpi.html

[R73] 分割大日志
来源：http://hz.xingfuxueyuan.xyz/gtgprlurtn.html

split -l 1000 big.log part_
来源：http://hz.jqgfzy.top/gtshirxnuz.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtwcfrgjvb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtknnyblqv.html

[R75] 导出环境变量
来源：http://hz.wangshuangyany.cn/gtymynfxij.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xylfe.cn/gtexedcafl.html

[R76] 使用临时文件
来源：http://hz.aizwys.cn/gtbohgpmdk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtuexymmvy.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gtulbwvnjy.html

read -rp "请输入: " ans
来源：http://hz.snrcjt.cn/gtwuismwei.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtpghvatzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtzttqtxas.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gtqdyouzea.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gtpiwseqeg.html

[R80] 查看脚本执行耗时
来源：http://hz.aizwys.cn/gtwzbcegjr.html

time ./run.sh
来源：http://hz.redwolf501.top/gttllasqoe.html

================================================================================
来源：http://hz.meibo888.top/gtweastxnx.html

S. C / C++ 专题
来源：http://hz.cdnleiting.top/gtnesroknt.html

================================================================================
来源：http://hz.bjfxy.top/gtmvbckoem.html

[S01] C：Hello World
来源：http://hz.zhoulong.xyz/gtujvtjmdy.html

#include <stdio.h>
来源：http://hz.fengsongda.top/gtzlgmkqlq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ywan-chungtsiang.top/gtzhabmita.html

[S02] C：变量与格式化输出
来源：http://hz.meibo888.top/gtzmucwley.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinyuanbaomall.cn/gtwsdjysju.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gteqsztqpk.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gthbhsjorr.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gtdsvsitoj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hongshengwenyu.top/gtofuxzsgj.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtxqdbmaui.html

strlen(s)
来源：http://hz.sufxvd.cn/gtnsahupew.html

[S06] C：字符串比较
来源：http://hz.aizwys.cn/gtcosigurz.html

strcmp(a, b) == 0
来源：http://hz.pycfn.com/gtthiteetb.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtyopakaej.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtkopmnolb.html

[S08] C：动态内存分配与释放
来源：http://hz.xziqi.cn/gtbigwhdju.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtghbetxee.html

[S09] C：结构体定义与初始化
来源：http://hz.jinyuanbaomall.cn/gtttnkuynl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.fzhhl.top/gtrconppin.html

[S10] C：指针与解引用
来源：http://hz.quarkkingdee.top/gtzjmvvljq.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gttulzsxrt.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtjctoowbc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shuidangran.top/gthemgysyg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtojvzqqfk.html

fclose(f);
来源：http://hz.chenlongwang.top/gtpjjqabox.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtlouutxok.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtuqgoigex.html

[S13] C：宏定义
来源：http://hz.yj20258.top/gtxwvoifbu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jqgfzy.top/gtagdvplci.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gttsrhnzfx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hywenlv.cn/gtupzernqx.html

[S15] C：类型转换
来源：http://hz.cheryme.top/gtfjarqwrh.html

(double) a / b
来源：http://hz.meibo888.top/gtfqawatqs.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtcyqnmjza.html

x |= (1 << 3);
来源：http://hz.ivvv.top/gtsmqnsvun.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtxmbjwnjb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtlqycgrol.html

[S18] C：命令行参数
来源：http://hz.0kj1m.cn/gtcvhayosi.html

int main(int argc, char **argv)
来源：http://hz.hnxiangtu.top/gtklcafynp.html

[S19] C：快速排序
来源：http://hz.yongpay.top/gtawnsluha.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtlncetteb.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtyijyhhle.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtbkdwdvaf.html

[S21] C：字符类别判断
来源：http://hz.guannengcc.top/gtbescveei.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.gogol.net.cn/gtatpdnymx.html

[S22] C：字符串转数字
来源：http://hz.hongshengwenyu.top/gtnbjwclkp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxinkj.top/gtrmfiiydl.html

[S23] C：随机数
来源：http://hz.jinqigufen.top/gtqonhubes.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gtzdkahhml.html

[S24] C：获取本地时间
来源：http://hz.zdqjudy.top/gtybyvtcwy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gtcjdibamn.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtwtreznke.html

memcpy(dst, src, n);
来源：http://hz.aizwys.cn/gtmeyeflxg.html

[S26] C：内存清零
来源：http://hz.wangdashe.top/gtrubjbclv.html

memset(a, 0, sizeof a);
来源：http://hz.shuidangran.top/gtyhfriqib.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtlzcyufzz.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtluikgwge.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtixvdrwty.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtevrhvukx.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtjpgxudht.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hywenlv.cn/gtibltbkls.html

[S30] C：头文件保护
来源：http://hz.0kj1m.cn/gtedbyuqqy.html

#ifndef X_H
来源：http://hz.aibaodan.cn/gtjnoewqev.html

#define X_H
来源：http://hz.nanxinkj.top/gtptvvncqz.html

#endif
来源：http://hz.yueranfly.top/gtxagupcaz.html

[S31] C++：Hello World
来源：http://hz.zhoulong.xyz/gthvoqyvso.html

#include <iostream>
来源：http://hz.andypj.xyz/gtdrmsinzu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sweek.top/gtrhkbejum.html

[S32] C++：字符串
来源：http://hz.jiagoushi.top/gtkykbgxid.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gtvqchrvyc.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtgqaavrsc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.aibaodan.cn/gthbpkjbdc.html

[S34] C++：遍历 vector
来源：http://hz.zdqjudy.top/gtbiqagtut.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenlongwang.top/gtybeyzwkv.html

[S35] C++：map
来源：http://hz.havefunace.top/gtznyuukjd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtjmmajudk.html

[S36] C++：unordered_map
来源：http://hz.svipenyu.cn/gtqxongzmu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtdgmtwyre.html

[S37] C++：set
来源：http://hz.gotoacloud.top/gtmzqfvuvc.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenlongwang.top/gtbaxxuocw.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtltjadgdv.html

std::sort(v.begin(), v.end());
来源：http://hz.vqdsnc.cn/gtqdilpizz.html

[S39] C++：自定义比较器排序
来源：http://hz.kuanghao11.cn/gtnukdfsxb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnxiangtu.top/gtfgacmwyu.html

[S40] C++：查找元素
来源：http://hz.tanke756.top/gteatctqne.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgufenzy.top/gtzfsffoaa.html

[S41] C++：类与构造函数
来源：http://hz.havefunace.top/gtyhenofwt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtcpgcxvsg.html

[S42] C++：继承与虚函数
来源：http://hz.svipenyu.cn/gtxjtzucxu.html

class B : public Base { public: void f() override {} };
来源：http://hz.fzhhl.top/gtpvcuskur.html

[S43] C++：智能指针
来源：http://hz.gotoacloud.top/gtlkobjmma.html

auto p = std::make_unique<int>(5);
来源：http://hz.jianghu66.top/gtjhyhgeia.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gteekkyixd.html

void inc(int &x) { ++x; }
来源：http://hz.gaohongyu789.top/gtceirsgrr.html

[S45] C++：lambda
来源：http://hz.kuanghao11.cn/gtpwommzzy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.havefunace.top/gtkwbkadot.html

[S46] C++：函数模板
来源：http://hz.hfpthk.cn/gtwrfhwtss.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtgvxqcdpo.html

[S47] C++：结构化绑定遍历
来源：http://hz.shangyingyoupin.top/gtskqmsoji.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hongshengwenyu.top/gtqmmzquda.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gttppslixn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yongpay.top/gtxrpgfmyt.html

while (std::getline(in, line)) { }
来源：http://hz.cucudq.cn/gtvgmuytbb.html

[S49] C++：写文件
来源：http://hz.kuanghao11.cn/gtqhvydizc.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhixingplan.top/gtlsirxevc.html

[S50] C++：格式化数字
来源：http://hz.yongpay.top/gtzbwhrvle.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.316326.xyz/gtpblyhxvf.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtpnbiltdu.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtrbwfiejh.html

[S52] C++：const 与 noexcept
来源：http://hz.andypj.xyz/gttsasqxpp.html

int size() const noexcept { return n_; }
来源：http://hz.nanxinkj.top/gtrywxkqda.html

[S53] C++：移动语义
来源：http://hz.pengpengdd.cyou/gtcziupdys.html

std::vector<int> w = std::move(v);
来源：http://hz.gaohongyu789.top/gtocejafhh.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtojwsyaie.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.daria6918.cn/gttecmosjv.html

[S55] C++：结构化绑定
来源：http://hz.xuetiantiany.cn/gtnamjyzbd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.redwolf501.top/gtcjnptxzp.html

[S56] C++：optional
来源：http://hz.hnxiangtu.top/gttrakkrvk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.nanxuanxn.top/gtylpnvpss.html

[S57] C++：编译期常量
来源：http://hz.aibaodan.cn/gtpivnwwbp.html

constexpr int N = 10;
来源：http://hz.zhoulong.xyz/gtwyxbxijl.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtwzlfgmuu.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtqgtvgndr.html

[S59] C++：静态断言
来源：http://hz.birdmap.top/gtliubickb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.fzhhl.top/gtzmclwvmm.html

[S60] C++：遍历并删除元素
来源：http://hz.jinqigfzy.top/gtjzkttguu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhoulong.xyz/gtxmtnriyt.html

================================================================================
来源：http://hz.kuanghao11.cn/gtixvnjthz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.52xcode.cn/gtlscqxvpm.html

================================================================================
来源：http://hz.c1oappe.top/gtnkwbtubb.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtwqogrzem.html

println("Hello")
来源：http://hz.nanxinkj.top/gtxloxorsv.html

[T02] Kotlin：变量
来源：http://hz.iojbl.cn/gtdaumjyji.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhaomingkeji.xyz/gtmhjwjpgk.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258.top/gtpqdieyvn.html

"值: $b"
来源：http://hz.yj20258.top/gtzhdyjnep.html

[T04] Kotlin：空安全
来源：http://hz.dashuyun.cn/gtvagpqjvy.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtjgpayxbp.html

[T05] Kotlin：when 表达式
来源：http://hz.jinyuanbaomall.cn/gtpyvnqdnr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ppjwa.cn/gtzxyugcla.html

[T06] Kotlin：集合映射
来源：http://hz.gzhubu.top/gtcthyxluz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hywenlv.cn/gtjkgjjmcp.html

[T07] Kotlin：集合过滤
来源：http://hz.daria6918.cn/gtrofalhxe.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tian-w.cn/gtzwwizmez.html

[T08] Kotlin：数据类
来源：http://hz.vqdsnc.cn/gtidqlybkc.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtbargcspd.html

[T09] Kotlin：扩展函数
来源：http://hz.hywenlv.cn/gtaqphrxuf.html

fun String.exclaim() = this + "!"
来源：http://hz.jqgfzy.top/gtpswmwtgq.html

[T10] Kotlin：默认参数
来源：http://hz.aizwys.cn/gtnbrykqns.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yueranfly.top/gtexctydsw.html

[T11] Kotlin：协程
来源：http://hz.yvedp.cn/gtbhdyiips.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jiagoushi.top/gtfzoijltx.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258.top/gtvjqajcrj.html

val (a, b) = Pair(1, 2)
来源：http://hz.kuanghao11.cn/gtizfwuyop.html

[T13] Kotlin：只读 Map
来源：http://hz.pycfn.com/gtwstqyddf.html

val m = mapOf("a" to 1)
来源：http://hz.svipenyu.cn/gtzccxjfat.html

[T14] Kotlin：循环
来源：http://hz.zhaomingkeji.xyz/gtaacyaxpv.html

for (i in 1..10) println(i)
来源：http://hz.xziqi.cn/gtdeuqxdev.html

[T15] Kotlin：接口
来源：http://hz.cdnleiting.top/gttnkntnrp.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtzzquodqs.html

[T16] Swift：Hello World
来源：http://hz.dashuyun.cn/gtntxhvvjy.html

print("Hello")
来源：http://hz.ydzc1.top/gtxthfqvyt.html

[T17] Swift：变量与常量
来源：http://hz.jqgufenzy.top/gtugxihuyx.html

var a = 1;  let b = 2
来源：http://hz.jinqigfzy.top/gtzxxpvsnw.html

[T18] Swift：字符串插值
来源：http://hz.yangfankeji.com/gtvqlijfic.html

"值: \(b)"
来源：http://hz.zhixingplan.top/gtzsmvnfhg.html

[T19] Swift：可选绑定
来源：http://hz.gaohongyu789.top/gtbylmwfyt.html

if let n = opt { print(n) }
来源：http://hz.tanke756.top/gtvwzrtmog.html

[T20] Swift：数组操作
来源：http://hz.yuxming.cn/gtuhiwqxgg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinghuilouyu.cn/gtgmnshnct.html

[T21] Swift：遍历
来源：http://hz.zhongyouzk.top/gtwrtbaiwp.html

for x in a { print(x) }
来源：http://hz.nwbrower.top/gthuegdymf.html

[T22] Swift：字典
来源：http://hz.xziqi.cn/gtdqvkhbha.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.kuanghao11.cn/gthinecwxi.html

[T23] Swift：函数
来源：http://hz.jinghuilouyu.cn/gtpnjuccya.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtowrotbwx.html

[T24] Swift：闭包
来源：http://hz.hysaishi.cn/gtbyofildr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cheryme.top/gtartmarrr.html

[T25] Swift：结构体
来源：http://hz.jinghuilouyu.cn/gtkzcoymmp.html

struct P { var x: Int }
来源：http://hz.feifeiyinyue.top/gtwtjvsbcv.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gthaddosfl.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gtqklfwxfv.html

[T27] Swift：错误处理
来源：http://hz.yj20258.top/gtmpxdxnwu.html

do { try f() } catch { print(error) }
来源：http://hz.gogol.net.cn/gtlojqgxki.html

[T28] Swift：枚举
来源：http://hz.zhengqikj.top/gtqzlfvqtl.html

enum Color { case red, green }
来源：http://hz.havefunace.top/gtjrpwkkpy.html

[T29] Swift：guard 提前返回
来源：http://hz.sufxvd.cn/gtjozirtld.html

guard let x = opt else { return }
来源：http://hz.52xcode.cn/gtowlcqnvj.html

[T30] Swift：协议
来源：http://hz.zdqjudy.top/gtgwmoanoc.html

protocol Shape { func area() -> Double }
来源：http://hz.zdqjudy.top/gtviiddrzm.html

[T31] Lua：Hello World
来源：http://hz.hnqzz.top/gtjtxghtxx.html

print("Hello")
来源：http://hz.cucudq.cn/gtqbskwxsf.html

[T32] Lua：局部变量
来源：http://hz.kuanghao11.cn/gtwqxmyvqq.html

local a = 1
来源：http://hz.xuanzx.com/gtbdnjjiiu.html

[T33] Lua：表（数组）
来源：http://hz.chenlongwang.top/gtjikvyjes.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtkdicdmuh.html

[T34] Lua：遍历表
来源：http://hz.tianlin.xyz/gtkgpygrad.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.feifeiyinyue.top/gtqmcdwopb.html

[T35] Lua：字典表
来源：http://hz.9152youxi.cn/gtvlvvnnmk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.ywan-chungtsiang.top/gtoxanqoqf.html

[T36] Lua：函数
来源：http://hz.nwbrower.top/gtreaqpaur.html

function add(a, b) return a + b end
来源：http://hz.sysykeji.top/gtmlzyucec.html

[T37] Lua：字符串拼接
来源：http://hz.zhoulong.xyz/gtrrlrahqw.html

"a" .. "b"
来源：http://hz.kuanghao11.cn/gtywpsnfbx.html

[T38] Lua：条件
来源：http://hz.gaohongyu789.top/gtduygzkii.html

if x > 0 then print("正") end
来源：http://hz.jlsjyb.cn/gtazbnagqs.html

[T39] Lua：模式匹配
来源：http://hz.havefunace.top/gtjxncbyiw.html

string.find(s, "%d+")
来源：http://hz.c1oappe.top/gtwdusifju.html

[T40] Lua：元表
来源：http://hz.mhx1999.top/gtiaexortw.html

setmetatable({}, { __index = base })
来源：http://hz.andypj.xyz/gtuzltfwhp.html


<!-- 参考信息 -->