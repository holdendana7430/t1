代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtmhiqcojs.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gttwgdbufz.html

echo "scale=2; 10/3" | bc
来源：http://hz.vqdsnc.cn/gtzxnswium.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gtupjxkeuf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cdnleiting.top/gtkqesslyh.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtgrygqsmf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtyeiljlxb.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtafarxacw.html

f() { local x=1; echo "$x"; }
来源：http://hz.xziqi.cn/gtsiryortm.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtzbhjyiee.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtqlnfciwm.html

[R33] 捕获错误并提示行号
来源：http://hz.aizwys.cn/gtcmixpeie.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gtvrcuqtwz.html

[R34] 退出时清理
来源：http://hz.pycfn.com/gtnxvurzyk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gttsyprkop.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtstmxjtxw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtassprcfz.html

[R36] 并发执行多个任务
来源：http://hz.wangshuangyany.cn/gthsxgkumx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.redwolf501.top/gttyptokzs.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gtwjokzcwq.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtmeetyttk.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtfsviakat.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtbimaxndz.html

[R39] 重定向标准输出与错误
来源：http://hz.hfpthk.cn/gtovtiefzv.html

cmd > out.log 2>&1
来源：http://hz.hysaishi.cn/gtnvsxkwvy.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtavshknmq.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtnuzhuuei.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtepxhqgau.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigufen.top/gtidxxhtly.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtggtdlrxh.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtqxguxlne.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtlrwmnbcr.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtdfkoqmyu.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtpnmrwjql.html

find . -mtime -7 -type f
来源：http://hz.iojbl.cn/gtlwebtokz.html

[R45] 批量删除
来源：http://hz.yj202588.top/gthpvepams.html

find . -name "*.tmp" -delete
来源：http://hz.aibaodan.cn/gtizckculz.html

[R46] 递归替换文件内容
来源：http://hz.hnqzz.top/gtnlmsaxjh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gotoacloud.top/gtazwtlvmi.html

[R47] sed 单行替换
来源：http://hz.yueranfly.top/gtjmdzpqip.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtobdhtzft.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtravmlmyz.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtemseirsm.html

[R49] awk 带条件
来源：http://hz.pycfn.com/gtavbvtncz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hywenlv.cn/gtalyyuwzm.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtldshbhmx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.redwolf501.top/gteannseof.html

[R51] 排序去重取前几
来源：http://hz.9152youxi.cn/gtiiacamyu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daria6918.cn/gtkpzhophe.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtstxaspzq.html

wc -l a.txt
来源：http://hz.sxryk.cn/gtfrbwoeaa.html

[R53] 查看文件头与实时尾
来源：http://hz.meibo888.top/gtvrmdihim.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dashuyun.cn/gtxgrazoxx.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtyblodftr.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtfoddhuyj.html

[R55] 压缩与解压
来源：http://hz.yj20258888.top/gtbxunmdhq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtyldzopna.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gtnuksjtwl.html

scp file user@host:/path/
来源：http://hz.yangfankeji.com/gtjnbhjpdw.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtorxmxfni.html

ssh user@host 'uptime'
来源：http://hz.zhaomingkeji.xyz/gtmoplgkko.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtanczlnpa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtdtgsqopd.html

[R59] 发 POST JSON
来源：http://hz.sufxvd.cn/gtzplorrcr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gttitbmkms.html

[R60] 只看 HTTP 状态码
来源：http://hz.xziqi.cn/gtdinqwifr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hammf.cn/gteocmrnpe.html

[R61] 磁盘占用
来源：http://hz.guowangkeji.top/gttqjzmlvi.html

df -h;  du -sh *
来源：http://hz.hfpthk.cn/gtdyuodiyc.html

[R62] 找最占空间的文件
来源：http://hz.dashuyun.cn/gtqrsrmyur.html

du -ah . | sort -rh | head -10
来源：http://hz.shuidangran.top/gtntylpoka.html

[R63] 内存与进程
来源：http://hz.jianghu66.top/gtgltyalyt.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtvmegxtea.html

[R64] 结束进程
来源：http://hz.yueranfly.top/gtwruriptq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gthzfwtgej.html

[R65] 查看端口占用
来源：http://hz.yuxming.cn/gtvlmcxcno.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cqqwz.cn/gtannkoxzh.html

[R66] 定时任务
来源：http://hz.hammf.cn/gtnwxvwkds.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtfgievpve.html

[R67] 生成随机十六进制串
来源：http://hz.52xcode.cn/gtpfqkwpcv.html

openssl rand -hex 16
来源：http://hz.zhoulong.xyz/gteodxnyld.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtncwegxcd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.9152youxi.cn/gtiogfqxch.html

[R69] 生成随机密码
来源：http://hz.haohaochexian.top/gtjxvlvdxx.html

head -c 16 /dev/urandom | base64
来源：http://hz.guannengcc.top/gtfbmsdllf.html

[R70] 时间戳与互转
来源：http://hz.sysykeji.top/gtstmqxbro.html

date +%s;  date -d @1700000000
来源：http://hz.hfpthk.cn/gtbtvtlkyf.html

[R71] 日期格式化
来源：http://hz.guowangkeji.top/gtzmqgxhge.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.andypj.xyz/gtkbnvlbsx.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gthvghpkhm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yueranfly.top/gtrgvryorz.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gttjsdjetg.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtwljvzmaj.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gtzgnbnxdn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtkmhtwxyx.html

[R75] 导出环境变量
来源：http://hz.xylfe.cn/gtlhsbqvgs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.smart0.xyz/gtoaqgogbj.html

[R76] 使用临时文件
来源：http://hz.gaohongyu789.top/gtgydpwfiq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtpkzreruj.html

[R77] 读取用户输入
来源：http://hz.gaohongyu789.top/gtssgaztep.html

read -rp "请输入: " ans
来源：http://hz.hysaishi.cn/gtjmhijqpa.html

[R78] 交互式菜单
来源：http://hz.zhiwuduotai.top/gthezsbllh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtiowkuzgl.html

[R79] 解析命令行选项
来源：http://hz.yvedp.cn/gtrkvwtshs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtdyappzqs.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtkrquoryf.html

time ./run.sh
来源：http://hz.shuidangran.top/gtnpilbnay.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtncnxheos.html

S. C / C++ 专题
来源：http://hz.c1oappe.top/gtebrxiddd.html

================================================================================
来源：http://hz.daria6918.cn/gtylzizkwi.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtgjcfqdxm.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtpiwlnmpl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtjejbidpb.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtshlagsik.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhoulong.xyz/gtcphcnigp.html

[S03] C：读入整数
来源：http://hz.sysykeji.top/gtmixtmakd.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtfguadrbo.html

[S04] C：字符串复制
来源：http://hz.redwolf501.top/gtighqgyml.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtopnnjvok.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtdxfzsrvs.html

strlen(s)
来源：http://hz.9152youxi.cn/gteukfbtzg.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtntenckop.html

strcmp(a, b) == 0
来源：http://hz.birdmap.top/gtrapjeexp.html

[S07] C：数组遍历求和
来源：http://hz.gogol.net.cn/gtczxafwhe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dashuyun.cn/gtiiysgzks.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gtziaftood.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.redwolf501.top/gtlxbzjpbl.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtttzsbrkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuxming.cn/gtnhvfegdv.html

[S10] C：指针与解引用
来源：http://hz.kuanghao11.cn/gtmcdumqbx.html

int *p = &a;  *p = 5;
来源：http://hz.sufxvd.cn/gtlteowhid.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtnhisazti.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.havefunace.top/gtjygyrpwr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtrunscilg.html

fclose(f);
来源：http://hz.cucudq.cn/gtmkvwvevy.html

[S12] C：写文件
来源：http://hz.yuanzhike.top/gtcagvbafn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cucudq.cn/gthiiskhpb.html

[S13] C：宏定义
来源：http://hz.ydzc1.top/gtukcvnwbz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtenvnhvpo.html

[S14] C：枚举
来源：http://hz.havefunace.top/gtdozmhatl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuanzx.com/gtaevrvqrd.html

[S15] C：类型转换
来源：http://hz.zhengqikj.top/gtgeaivdwm.html

(double) a / b
来源：http://hz.sxryk.cn/gtkpixhysw.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtuhmhiqad.html

x |= (1 << 3);
来源：http://hz.yangfankeji.com/gtjxzzykzp.html

[S17] C：安全拼接字符串
来源：http://hz.hongshengwenyu.top/gtmxnohcji.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gthrukokxz.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gtqjymphvu.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtrhzxeqed.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gthyiaxjph.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtnxsuzqud.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtbrfvwfbz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtthzyjmka.html

[S21] C：字符类别判断
来源：http://hz.chenjidiqi.icu/gtxosmlocq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jiagoushi.top/gtegraukzt.html

[S22] C：字符串转数字
来源：http://hz.yj20258888.top/gtqkhjaqag.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.pycfn.com/gtctzmbqhs.html

[S23] C：随机数
来源：http://hz.haohaochexian.top/gtxenprqkf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hysaishi.cn/gttwbbmtxp.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtutytydld.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.smart0.xyz/gtvwipcljn.html

[S25] C：内存拷贝
来源：http://hz.aizwys.cn/gtcvijsysn.html

memcpy(dst, src, n);
来源：http://hz.zycfv.cn/gtkbtbpiwm.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtupjvjeej.html

memset(a, 0, sizeof a);
来源：http://hz.jyoumei.cn/gtysowrpxf.html

[S27] C：定义常量
来源：http://hz.jiagoushi.top/gtedyadubt.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gtljezpanh.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtqbbraowz.html

static int counter = 0;
来源：http://hz.shzxlz.cn/gtxllvicjs.html

[S29] C：变参函数
来源：http://hz.ydzc1.top/gtmixptpjl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.aibaodan.cn/gtuzaulopa.html

[S30] C：头文件保护
来源：http://hz.ivvv.top/gtocrmdbtw.html

#ifndef X_H
来源：http://hz.hammf.cn/gtnlpitcsz.html

#define X_H
来源：http://hz.hnqzz.top/gtagroxnio.html

#endif
来源：http://hz.52xcode.cn/gtowudukzu.html

[S31] C++：Hello World
来源：http://hz.snrcjt.cn/gtrqqttwjn.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtspltzibn.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xingfuxueyuan.xyz/gtkghhrwou.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gttglsbpec.html

std::string s = "hi";  s += "!";
来源：http://hz.jianghu66.top/gtijoziwlp.html

[S33] C++：vector 增删
来源：http://hz.tian-w.cn/gtpwchgize.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.bjfxy.top/gtylzyexiv.html

[S34] C++：遍历 vector
来源：http://hz.cheryme.top/gtussicivm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.meibo888.top/gtrvmshebz.html

[S35] C++：map
来源：http://hz.redwolf501.top/gtodmoozfr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenzaomai.com/gttnnzkatx.html

[S36] C++：unordered_map
来源：http://hz.aibaodan.cn/gtfaxegncy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ehwqpu.com/gtobyrqnmp.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtxfdpkpzv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.hfpthk.cn/gtowngbnru.html

[S38] C++：排序
来源：http://hz.ywan-chungtsiang.top/gtvhviuigw.html

std::sort(v.begin(), v.end());
来源：http://hz.cashguo.top/gtlsqghzpr.html

[S39] C++：自定义比较器排序
来源：http://hz.jyoumei.cn/gtmemkytvc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daxiang520.top/gtikqsojrz.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtgitqqtvj.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtekrdgfne.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtkplualvi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yongpay.top/gtxnwszpyf.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gtkxxynvcn.html

class B : public Base { public: void f() override {} };
来源：http://hz.ehwqpu.com/gtpnfnugev.html

[S43] C++：智能指针
来源：http://hz.dianchejie.cn/gtwlzffzkk.html

auto p = std::make_unique<int>(5);
来源：http://hz.sufxvd.cn/gtpczfgevr.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gtjzsgpnrl.html

void inc(int &x) { ++x; }
来源：http://hz.vqdsnc.cn/gtskjbeiaw.html

[S45] C++：lambda
来源：http://hz.shanyushiyangkeji.top/gtccmhwwee.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yongpay.top/gthxekopze.html

[S46] C++：函数模板
来源：http://hz.kuanghao11.cn/gtftirtayb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jlsjyb.cn/gtmycwpqfy.html

[S47] C++：结构化绑定遍历
来源：http://hz.xuanzx.com/gtccmwdidg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gthbdufjbh.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtouxeqbgd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jinqigufen.top/gtecbldslb.html

while (std::getline(in, line)) { }
来源：http://hz.jyoumei.cn/gtimqjzprb.html

[S49] C++：写文件
来源：http://hz.yonumen.top/gtytndnlqw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.andypj.xyz/gtxydvkxce.html

[S50] C++：格式化数字
来源：http://hz.sysykeji.top/gtrfyhtgyz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gtwsspjfmd.html

[S51] C++：显式类型转换
来源：http://hz.svipenyu.cn/gtseqbihvg.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtbymczhlj.html

[S52] C++：const 与 noexcept
来源：http://hz.nanxuanxn.top/gtjcekbiod.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtmiantcgk.html

[S53] C++：移动语义
来源：http://hz.cashguo.top/gtmuyuhhmi.html

std::vector<int> w = std::move(v);
来源：http://hz.kuanghao11.cn/gtsevcnbfs.html

[S54] C++：异常处理
来源：http://hz.mhx1999.top/gtydsmzkgi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jiagoushi.top/gtnmvpbfpf.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gticewqcjf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gtgbhfvjry.html

[S56] C++：optional
来源：http://hz.sxryk.cn/gtkgunflpq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenzaomai.com/gtjfdabtmc.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtexvferbw.html

constexpr int N = 10;
来源：http://hz.chenjidiqi.icu/gtlzyeauhe.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtzevgwtrg.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtsssnbslu.html

[S59] C++：静态断言
来源：http://hz.smart0.xyz/gtjptrpbkj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gaohongyu789.top/gtsuurcuhu.html

[S60] C++：遍历并删除元素
来源：http://hz.c1oappe.top/gtozmmtouc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtyikrouus.html

================================================================================
来源：http://hz.wangdashe.top/gtovjfmebn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yonumen.top/gtbsyccsxm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpoynxqsq.html

[T01] Kotlin：Hello World
来源：http://hz.wangdashe.top/gtaccxkywn.html

println("Hello")
来源：http://hz.nwbrower.top/gtrczrmpem.html

[T02] Kotlin：变量
来源：http://hz.aizwys.cn/gtkwjlhkqq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.xinyue.icu/gttexeytop.html

[T03] Kotlin：字符串模板
来源：http://hz.hysaishi.cn/gtuyckxzzy.html

"值: $b"
来源：http://hz.jiagoushi.top/gtsbskmvjw.html

[T04] Kotlin：空安全
来源：http://hz.hammf.cn/gtbvoxilhe.html

val n: String? = null;  n?.length
来源：http://hz.shuidangran.top/gtjlxhqqmi.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gtbkjadmqf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.wangdashe.top/gttyxwknys.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtviywajsv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yanxiufei.cn/gtdkmtixua.html

[T07] Kotlin：集合过滤
来源：http://hz.cqqwz.cn/gtoatppvyz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj20258888.top/gtpffrhyuf.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtjawugnpb.html

data class User(val name: String, val age: Int)
来源：http://hz.daxiang520.top/gtcbomkzih.html

[T09] Kotlin：扩展函数
来源：http://hz.ywan-chungtsiang.top/gtpzimeeyd.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gttfinghzo.html

[T10] Kotlin：默认参数
来源：http://hz.xingfuxueyuan.xyz/gtopmsnttu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.haohaochexian.top/gtvoscjdex.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtyacqkjbr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydjk.org.cn/gtemelpxyz.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gtvpihwqde.html

val (a, b) = Pair(1, 2)
来源：http://hz.xuanzx.com/gteauxxakq.html

[T13] Kotlin：只读 Map
来源：http://hz.yuxming.cn/gtevxpsght.html

val m = mapOf("a" to 1)
来源：http://hz.havefunace.top/gtxoggyaem.html

[T14] Kotlin：循环
来源：http://hz.aibaodan.cn/gtoyyoqzlu.html

for (i in 1..10) println(i)
来源：http://hz.birdmap.top/gtkejucsgz.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtkxzdwjmu.html

interface Shape { fun area(): Double }
来源：http://hz.jqgfzy.top/gtopxmjqlf.html

[T16] Swift：Hello World
来源：http://hz.xingfuxueyuan.xyz/gttmyitapm.html

print("Hello")
来源：http://hz.fzhhl.top/gtltxlmywe.html

[T17] Swift：变量与常量
来源：http://hz.gzhubu.top/gtifarampv.html

var a = 1;  let b = 2
来源：http://hz.wangshuangyany.cn/gtcysxlntt.html

[T18] Swift：字符串插值
来源：http://hz.snrcjt.cn/gthopwelaj.html

"值: \(b)"
来源：http://hz.yuxming.cn/gtugtvgxcs.html

[T19] Swift：可选绑定
来源：http://hz.ehwqpu.com/gtpbahwpkp.html

if let n = opt { print(n) }
来源：http://hz.sufxvd.cn/gtfexdzsur.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtroybtwdz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tanke756.top/gtwobcevvg.html

[T21] Swift：遍历
来源：http://hz.gaohongyu789.top/gtycaehnaa.html

for x in a { print(x) }
来源：http://hz.jinyuanbaomall.cn/gtdglpteke.html

[T22] Swift：字典
来源：http://hz.tianlin.xyz/gtnahwpeny.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.xinyue.icu/gtfvxhgfii.html

[T23] Swift：函数
来源：http://hz.redwolf501.top/gtohmbtlfo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jyoumei.cn/gtpkqrvgdm.html

[T24] Swift：闭包
来源：http://hz.mhx1999.top/gtfnrowcqo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhijiandao.cn/gtcnpmumll.html

[T25] Swift：结构体
来源：http://hz.wangdashe.top/gtbqfvkmqj.html

struct P { var x: Int }
来源：http://hz.cqqwz.cn/gtuyhczjcw.html

[T26] Swift：类与重写
来源：http://hz.xinyue.icu/gtkdqmwqti.html

class A: Base { override func f() {} }
来源：http://hz.fengsongda.top/gtiucvahyk.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtdzljykmr.html

do { try f() } catch { print(error) }
来源：http://hz.xuanzx.com/gtdxctjjcw.html

[T28] Swift：枚举
来源：http://hz.jinqigufen.top/gtzbysjjue.html

enum Color { case red, green }
来源：http://hz.jyoumei.cn/gtagatfjhm.html

[T29] Swift：guard 提前返回
来源：http://hz.guowangkeji.top/gtkltzfsez.html

guard let x = opt else { return }
来源：http://hz.dianchejie.cn/gtvlwdcruh.html

[T30] Swift：协议
来源：http://hz.yuxming.cn/gtlgwzbzsd.html

protocol Shape { func area() -> Double }
来源：http://hz.gzhubu.top/gtphrwxfaf.html


<!-- 参考信息 -->